# Related Projects

## Introduction

This document lists projects, hardware, tools, research efforts, and community work related to the ChipSlayer project.

These references are included for:

- historical context
- technical research
- compatibility understanding
- hardware comparison
- installation reference
- general PlayStation 2 development knowledge

Inclusion here does not necessarily imply endorsement, affiliation, or compatibility.

---

# PlayStation 2 Modchips

## ModBo 5.0

### Overview

The ModBo 5.0 is one of the primary modchips used during ChipSlayer testing and development.

It is a Matrix-derived clone modchip commonly installed in PlayStation 2 consoles.

### Relevance to ChipSlayer

ChipSlayer development heavily focuses on how ModBo-style chips interact with:

- reset circuitry
- startup timing
- signal loading
- console boot behavior

### Notes

Different ModBo revisions and clone variations may behave differently.

---

## Matrix Infinity

### Overview

The Matrix Infinity is one of the most influential PlayStation 2 modchip designs.

Many later clone chips are derived from Matrix-style hardware or firmware concepts.

### Relevance to ChipSlayer

ChipSlayer testing may eventually expand to additional Matrix-derived hardware.

---

## Other PS2 Modchips

Additional modchips may eventually be evaluated, including:

- clone variants
- legacy modchips
- rare regional hardware
- custom firmware variants

Compatibility is currently unknown for many of these devices.

---

# PS2 Homebrew Projects

## Open PS2 Loader (OPL)

### Overview

OPL is one of the most widely used PlayStation 2 homebrew applications.

It allows games and applications to be loaded from:

- SMB/network
- HDD
- USB
- MX4SIO
- SD2PSX-related setups

### Relevance to ChipSlayer

Many ChipSlayer test systems also use OPL-based configurations.

---

## PS2Ident

### Overview

PS2Ident is a hardware identification and diagnostic utility for PlayStation 2 consoles.

### Relevance to ChipSlayer

PS2Ident may be used during testing to compare console behavior between:

- modchip enabled
- modchip disabled
- ChipSlayer enabled
- ChipSlayer bypassed

### Notes

PS2Ident logs may help document console revision differences and startup behavior observations.

---

## wLaunchELF (uLaunchELF)

### Overview

wLaunchELF is a widely used PS2 utility and file-management environment.

### Relevance to ChipSlayer

Many test consoles use wLaunchELF during validation and troubleshooting procedures.

---

# Related Hardware Projects

## BlueRetro

### Overview

BlueRetro is an open-source wireless controller adapter project.

### Relevance to ChipSlayer

Some test consoles combine:

- ChipSlayer
- BlueRetro
- internal HDMI modifications
- custom power-management systems

### Notes

Complex internal builds may create additional variables during testing.

---

## SD2PSX / MMCE Projects

### Overview

SD2PSX-style projects provide advanced memory card and storage functionality for PlayStation 2 systems.

### Relevance to ChipSlayer

Some integrated test builds combine ChipSlayer with internal MMCE-based hardware setups.

---

## Internal HDMI Modifications

### Overview

Many modern PS2 builds include internal HDMI modifications.

### Relevance to ChipSlayer

Additional internal hardware may affect:

- internal layout
- grounding
- thermal behavior
- wiring complexity
- signal routing

These variables may influence testing observations.

---

# Related Technical Areas

## Reset Supervisor Circuits

### Overview

PlayStation 2 consoles use supervisory reset circuitry to manage startup behavior.

### Relevance to ChipSlayer

ChipSlayer development heavily investigates interaction with reset-related signals and startup timing.

---

## High-Impedance Switching

### Overview

High-impedance switching techniques are important for minimizing electrical influence on sensitive console signals.

### Relevance to ChipSlayer

A major project goal is reducing electrical loading while maintaining predictable behavior.

---

## Signal Integrity

### Overview

Signal integrity strongly affects console startup and stability behavior.

### Relevance to ChipSlayer

Areas of concern include:

- wire length
- leakage current
- pull-up interaction
- ringing
- startup timing
- floating states

---

# Development Tools

## KiCad

### Overview

KiCad is the primary PCB design software used during development.

### Relevance to ChipSlayer

Used for:

- schematic capture
- PCB layout
- revision tracking
- prototype generation

---

## Oscilloscope Testing

### Overview

Oscilloscope analysis is used extensively during validation.

### Relevance to ChipSlayer

Used for observing:

- reset-line behavior
- startup timing
- voltage transitions
- switching behavior
- signal integrity

---

## Logic Analysis

### Overview

Logic analysis tools may be used to observe digital signal behavior during startup and operation.

### Relevance to ChipSlayer

May assist in identifying:

- unexpected transitions
- startup-state behavior
- timing anomalies

---

# Community Research

## PS2 Modding Communities

### Overview

Many important observations related to PlayStation 2 hardware behavior originate from community experimentation and shared research.

### Relevance to ChipSlayer

Community testing and discussion may help:

- identify unusual behavior
- compare motherboard revisions
- validate installation methods
- identify compatibility trends

---

# Hardware Manufacturers and Components

## Texas Instruments

### Overview

Several switching and logic components evaluated during development originate from Texas Instruments.

### Relevance to ChipSlayer

Certain analog switches and logic devices may be evaluated for reset-line isolation behavior.

---

## MOSFET and Logic Device Research

### Overview

Various MOSFETs, buffers, and analog switches may be explored during development.

### Relevance to ChipSlayer

Areas of investigation include:

- leakage current
- startup state behavior
- high-impedance switching
- logic compatibility

---

# Important Notes

This document is intended only as a research and reference index.

Projects listed here:

- remain property of their respective owners
- may use different licenses
- may not be compatible with ChipSlayer
- may evolve independently

Always consult original project documentation when applicable.

---

# Future Expansion

This document may eventually expand to include:

- technical papers
- developer notes
- forum references
- historical modchip information
- component references
- diagnostic utilities
- related hardware experiments

---

# Final Notes

ChipSlayer development exists within a much larger ecosystem of PlayStation 2 hardware experimentation, repair, preservation, and homebrew development.

Understanding related projects and technologies is an important part of understanding how PlayStation 2 hardware behaves under modification.
