# Project Overview

## Introduction

ChipSlayer is a PlayStation 2 hardware interface board developed to provide controlled enable/disable functionality for installed modchips while minimizing interference with normal console operation.

The project was created during experimentation with PS2 Slim modchip behavior, particularly surrounding reset-line interaction, boot consistency, and the ability to temporarily isolate a modchip without physically removing wiring from the console.

Rather than simply disconnecting power to the modchip, ChipSlayer focuses on controlling the modchip reset and ground behavior in a cleaner and more repeatable way.

This repository serves as the primary documentation, testing, validation, and revision-tracking hub for the ChipSlayer project.

---

# Project Goals

The primary goals of ChipSlayer are:

- Provide a reliable method for enabling or disabling a PS2 modchip
- Minimize interference with normal console operation
- Improve repeatability compared to manually disconnecting wires
- Allow testing of console behavior with and without the modchip active
- Document hardware revisions and testing results
- Create a clean and compact installation method suitable for long-term installs

---

# Purpose of the Repository

This repository is intended to document the project and preserve development history.

The repository currently focuses on:

- Hardware revision tracking
- Installation notes
- Console compatibility testing
- Scope captures and electrical observations
- Research and development notes
- Board photos and prototype comparisons
- Known issues and limitations
- General project documentation

This repository is **not currently intended to be a full open-source hardware release**.

Production-ready manufacturing files, Gerbers, and complete production schematics may not be publicly released at this time while development and commercial testing continue.

---

# Background

During testing of PlayStation 2 Slim consoles with installed modchips, several behaviors were observed:

- Some consoles behaved differently depending on whether the modchip reset line was connected
- Simply removing power from the modchip was not always sufficient
- Certain modchip connections could still influence console behavior even when "disabled"
- Reset-line behavior varied between motherboard revisions
- Ground isolation and reset isolation both played important roles

ChipSlayer was developed as an experimental hardware solution intended to better isolate the modchip from the console when desired.

---

# Design Philosophy

ChipSlayer is designed around several core ideas:

## Minimal Invasiveness

The design attempts to work with existing modchip installs while minimizing additional wiring and complexity.

## Controlled Isolation

Rather than physically removing or rewiring the modchip, ChipSlayer attempts to electronically isolate key signals in a controlled manner.

## Revision Tracking

Different PlayStation 2 motherboard revisions can behave differently. Development and testing are tracked carefully to document compatibility and observed behavior.

## Serviceability

The project is intended to remain understandable, testable, and repairable by hobbyists and hardware developers.

---

# Hardware Focus

Current development has primarily focused on PlayStation 2 Slim consoles, particularly:

- SCPH-700xx
- SCPH-750xx
- SCPH-770xx

Testing may eventually expand further into additional motherboard revisions and hardware configurations.

---

# Current Status

ChipSlayer has moved beyond the initial concept phase.

Prototype hardware revisions have been:
- Designed
- Manufactured
- Installed
- Tested on real hardware

The project is still considered experimental and under active development.

---

# Compatibility Notes

Compatibility can vary depending on:

- Console motherboard revision
- Modchip type
- Installation quality
- Existing console modifications
- Power conditions
- Reset-line behavior
- Signal integrity

Additional compatibility information is documented elsewhere within this repository.

---

# Repository Structure

This repository is organized into several major sections:

| Folder | Purpose |
|---|---|
| `Documents/` | Project documentation and technical notes |
| `Hardware/` | PCB revisions, schematics, and board references |
| `Images/` | Board photos, installation examples, and captures |
| `Test-Data/` | Console logs, testing results, and observations |
| `References/` | Datasheets, research notes, and related information |

---

# Important Disclaimer

ChipSlayer is an experimental hardware modification project.

Installation requires soldering and modification of PlayStation 2 hardware.

Improper installation or misuse may damage hardware.

This project is intended for:
- Research
- Hardware experimentation
- Console repair
- Hobbyist development
- Educational purposes

Use at your own risk.

---

# Author

Developed and documented by:

**Fat Bald Dad (FBD Retro Game)**

Additional collaborators, testers, and contributors may be credited throughout the repository as development continues.
