# Load test plan

Next round of bench tests for the AP63201 board. Blank cells are not measured yet.

## Setup

- Input: GW Instek GPS-4303 bench supply at 12.0 V, with the current limit set above the expected input current.
- Load: DC electronic load on J2 in constant-current mode.
- Measurements: Agilent 34405A DMM for Vout; supply readout (or a second meter) for Vin and Iin; Rohde & Schwarz RTC1002 for ripple.
- Before testing: recheck continuity between J1 GND and J2 GND.

## Load and efficiency

Efficiency η = (Vout × Iout) / (Vin × Iin)

| Iout (A) | Vin (V) | Iin (A) | Vout (V) | Pout (W) | Pin (W) | η (%) |
|---|---|---|---|---|---|---|
| 0.5 | | | | | | |
| 1.0 | | | | | | |
| 2.0 | | | | | | |

## Output ripple at 2 A

- Probe the output capacitor directly with the ground-spring tip (no long ground lead), with 20 MHz bandwidth limit on.
- Calculated expectation: about 3–7 mV peak-to-peak.

| Condition | Ripple (mV p-p) |
|---|---|
| 12 V in, 2 A out | |

## Temperature at 2 A

| Condition | U1 temperature after 10 min (°C) | Ambient (°C) |
|---|---|---|
| 12 V in, 2 A out | | |

Design estimate: about 45 °C rise at the IC.
