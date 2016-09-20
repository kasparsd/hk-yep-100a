# Hobbyking YEP 100A

Here is an overview of the [Hobbyking YEP 100A ESC](http://www.hobbyking.com/hobbyking/store/__20695__Hobbyking_YEP_100A_2_6S_SBEC_Brushless_Speed_Controller.html) which is a clone of [YGE 90 LV](http://www.yge.de/pages/pup.php).

## Hardware

- Atmel Mega 168PA (AU 1451) microcontroller
- Intersil ISL6700 (L423FKW) half-bridge drivers
- ON Semiconductor LM2931 (PFJZ5) voltage regulator (40V input continuous)
- TOSHIBA TPCA8060-H N-Channel MOSFETS


## ATmega168PA Connections

- PD1: PWM throttle input
- PD3: LED negative
- PB6, PB7 XTAL
- PB0: Phase A Hi
- PB1: Phase C Hi
- PB2: Phase B Hi
- PB3: Phase A Li
- PB4: Phase C Li
- PB5: Phase B Li
- PC0: Vbat through 18.2kOhm and 2kOhm voltage divider
- PC1: Unknown ADC


## MOSFET board connections

HO, LO and HS are connections to ISL6700. From top (DC input) to bottom (Phase output):

- GND
- GND
- Vbat
- Vbat
- Not connected?
- Phase C HO
- Phase C LO
- Phase B HO
- Phase B LO
- Phase A HO
- Phase A LO
- Unknown ADC
- Phase C HS
- Phase B HS
- Phase A HS


## Specification

- Max continuous current: 100A
- Max burst current: 120A for 10 seconds
- Input voltage: 2-6 cells li-XX or 6-16 Ni-MH/Ni-Cd battery
- BEC: 5.5V/6A Switching BEC
- PWM: 8~16 KHz
- Max RPM: 240,000rpm for 2 Poles Brushless Motor
- PCB size: 50x30mm
- Weight: 81g (including wires)


## Features

- Powerful 5.5V/6A Switching BEC
- Optional programming card for convenient setup
- Super fine throttle resolution provides first-rate and highly accurate linearity
- Super smooth adjustable start-up mode
- Constant RPM mode (governor mode)
- Adjustable F3A brake.
- 3 steps adjustable normal EMF brake
- High anti-interference capability
- Low voltage cut-off protection with automatic adjustment for NiCd/NiMH/Li-Ion/LiPo/LiFePO4
- Soft cut-off option at low voltage, slows motor RPM gradual rather than hard cutoff (LVC)
- Low voltage cut-off can be disabled
- Variable cut-off voltage / cell
- Active free-wheeling circuit allows for unlimited "partial load" capability
- LED status display
- Adjustable motor timing from 0° to 30°
- Blocked rotation protection (senses a jammed motor and stops motor rotation)
- Motor reversing from ESC (no need to change ESC/motor wires)
- Over-temperature protection and overload alarm
- Anti sparking circuit: reduces connection sparks (for HV ESC)
- Throttle signal lose protection. If the signal is lost for 3 seconds, the power will automatically cut-off.
- Safe power-on. (Motor will not start until throttle is returned to lowest position)
