# Study Notes

## SoC vs SiP

SoC:
multiple system functions integrated on one semiconductor die.

SiP:
multiple dies / components integrated within one package.

The project examines both because wearable products can combine die-level integration and package-level heterogeneous integration.

## AFE

Analog Front-End is the first circuit block that receives weak sensor signals.

For biosignals, low input-referred noise, high input impedance, CMRR, and PSRR can be more important than raw computational throughput.

## Always-On Domain

A low-power always-on domain remains active while high-power blocks sleep.

Its role is to monitor sensor events and decide when the main system should wake.

## Static vs Dynamic Power

Static:
leakage-related power even when switching activity is low.

Dynamic:
switching energy, often modeled approximately with C·V²·f.

## High-k

High dielectric constant material such as HfO₂ can support a thicker physical dielectric while maintaining a small EOT, helping reduce direct tunneling leakage.

## GAA

Gate-All-Around improves electrostatic channel control compared with structures where the gate surrounds fewer channel surfaces.

## TIM

Thermal Interface Material reduces thermal resistance between heat-generating die/package structures and the heat-spreading path.

## Mechanical Interface

Wearable sensor reliability also depends on the interface between rigid electronics and soft human skin, motivating flexible substrate and electrode materials.
