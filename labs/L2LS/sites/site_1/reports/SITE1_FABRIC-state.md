# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed | Total Tests Skipped |
| ----------- | ------------------ | ------------------ | ------------------- |
| 29 | 23 | 2 | 4 |

### Summary Totals Device Under Test

| Device Under Test | Total Tests | Tests Passed | Tests Failed | Tests Skipped | Categories Failed | Categories Skipped |
| ------------------| ----------- | ------------ | ------------ | ------------- | ----------------- | ------------------ |
| s1-spine1 | 29 | 23 | 2 | 4 | Interfaces | Hardware |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed | Tests Skipped |
| ------------- | ----------- | ------------ | ------------ | ------------- |
| Connectivity | 6 | 6 | 0 | 0 |
| Hardware | 4 | 0 | 0 | 4 |
| Interfaces | 16 | 14 | 2 | 0 |
| MLAG | 1 | 1 | 0 | 0 |
| System | 2 | 2 | 0 | 0 |

## Failed Test Results Summary

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 17 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet7 - P2P_WANCORE_Ethernet2 = 'up' | FAIL | Ethernet7 - Expected: up/up, Actual: down/down |
| 18 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet8 - P2P_WANCORE_Ethernet2 = 'up' | FAIL | Ethernet8 - Expected: up/up, Actual: down/down |

## All Test Results

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 1 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s1-spine2 Ethernet1 | PASS | - |
| 2 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s1-leaf1 Ethernet2 | PASS | - |
| 3 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s1-leaf2 Ethernet2 | PASS | - |
| 4 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: s1-leaf3 Ethernet2 | PASS | - |
| 5 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: s1-leaf4 Ethernet2 | PASS | - |
| 6 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s1-spine2 Ethernet6 | PASS | - |
| 7 | s1-spine1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 8 | s1-spine1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 9 | s1-spine1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 10 | s1-spine1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 11 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s1-spine2_Ethernet1 = 'up' | PASS | - |
| 12 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - L2_s1-leaf1_Ethernet2 = 'up' | PASS | - |
| 13 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - L2_s1-leaf2_Ethernet2 = 'up' | PASS | - |
| 14 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - L2_s1-leaf3_Ethernet2 = 'up' | PASS | - |
| 15 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - L2_s1-leaf4_Ethernet2 = 'up' | PASS | - |
| 16 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s1-spine2_Ethernet6 = 'up' | PASS | - |
| 17 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet7 - P2P_WANCORE_Ethernet2 = 'up' | FAIL | Ethernet7 - Expected: up/up, Actual: down/down |
| 18 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet8 - P2P_WANCORE_Ethernet2 = 'up' | FAIL | Ethernet8 - Expected: up/up, Actual: down/down |
| 19 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 20 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s1-spine2_Port-Channel1 = 'up' | PASS | - |
| 21 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel2 - L2_RACK1_Port-Channel2 = 'up' | PASS | - |
| 22 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - L2_RACK2_Port-Channel2 = 'up' | PASS | - |
| 23 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 24 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 25 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 26 | s1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 27 | s1-spine1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 28 | s1-spine1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 29 | s1-spine1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
