# 01 — Nitrogen Liquefaction Using Linde Cycle
**Author:** Eze Chukwuemeka Ephraim
**Institute:** University of Lagos

## Overview
Simulation of nitrogen liquefaction using the
Linde cycle implemented in DWSIM 9.0.

## Process Description
- Feed: Gaseous N2 at 300 K, 1 atm
- Compression to 25 atm (50% adiabatic efficiency)
- Cooling train to 85 K
- Isenthalpic expansion to 1 atm
- Gas-Liquid separation
- Liquid yield: ~917.6 kg/h from 1,000 kg/h feed

![Flowsheet](flowsheet_screenshot.png)
## Key Results
| Stream | Temp (K) | Pressure (atm) | Mass Flow (kg/h) |
|---|---|---|---|
| Feed (Mixed N2) | 300 | 1 | 1,000 |
| Compressed N2 | 1,145 | 25 | 1,000 |
| Cooled N2-S3 | 85 | 25 | 1,000 |
| Liquified N2 | 77.35 | 1 | 917.6 |

## Equipment Summary
| Unit | Type | Key Setting |
|---|---|---|
| Compressor | Adiabatic | 50% efficiency, 25 atm outlet |
| CL-1 | Cooler | Outlet 300 K |
| HX-1 | Heat Exchanger | LMTD 88.24 K |
| Cooler | Cooler | Outlet 85 K |
| VALVE-1 | Isenthalpic Valve | 1 atm outlet |
| V-1 | Gas-Liquid Separator | 1 atm, 77.35 K |

## Software
- DWSIM v9.0
- Property Package: Peng-Robinson

## How to Run
1. Install [DWSIM](https://dwsim.org)
2. Open `MySimulation_43.dwxml`
3. Press F5 to solve
