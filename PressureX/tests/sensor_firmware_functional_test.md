# PressureX Sensor – Firmware Functional Test Plan

**Version:** 1.0  
**Date:** 2025-05-17  
**Author:** B. W. Design  
**Target Audience:** Firmware Engineers, QA Engineers, Hardware Test Technicians

---

## Objective

Validate that the embedded firmware reliably:

- Initializes hardware correctly  
- Measures and transmits pressure data  
- Handles faults and recoverable failures  
- Maintains timing, communication, and accuracy across edge cases  

---

## Test Environment

| Component              | Version/Model          |
|------------------------|------------------------|
| MCU Board              | STM32F303K8T6 (Flight Rev) |
| Firmware Build System  | PlatformIO 6.1.5        |
| Host Interface         | USB-UART Adapter @115200 |
| Logging Tool           | SerialLog v1.2          |
| Power Supply           | 3.3V regulated @0.5A    |

---

## Test Categories

### A. Boot & Initialization

- Power-on reset test
- Warm boot (soft reset via command)
- Cold boot (full power cycle)
- EEPROM check
- Sensor handshake success

✅ **Pass:** No boot hangs, config values correctly loaded.

---

### B. Pressure Data Acquisition

- Confirm default sampling rate (10Hz)
- Validate correct pressure unit output (Pa)
- Inject known test pressure via simulator
- Compare sensor output vs known input

✅ **Pass:** Output matches input ±2% FS across full range

---

### C. Communication & Uplink

- Confirm command-response interface over UART
- Issue `STATUS`, `CALIBRATE`, `RESET` commands
- Simulate dropped packets
- Validate recovery and retransmission

✅ **Pass:** No freeze, watchdog triggers on stall, CRC errors logged but handled.

---

### D. Fault Injection

- Induce overvoltage (simulate 3.6V spike)
- Disable I2C mid-stream
- Remove pressure element during runtime
- Trigger watchdog intentionally

✅ **Pass:** Fault state entered, logged, and recovery attempted if safe.

---

### E. Power Cycling Robustness

- Repeated power cycles (100x @ 5 sec interval)
- Memory persistence test (EEPROM save/load validation)

✅ **Pass:** No memory corruption or bootlock

---

## Output Validation

All output should be logged to `/logs/firmware_test/` directory.  
Sample CSV fields:

```csv
timestamp,pressure_reading_Pa,cmd_response,crc_status,event_flags
2025-05-17T10:12:03Z,101325,OK,CRC_OK,NONE
