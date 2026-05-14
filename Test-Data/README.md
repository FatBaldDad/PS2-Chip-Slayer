# Test Data

## Introduction

This directory contains testing information, validation notes, console observations, and experimental data related to the ChipSlayer project.

The purpose of this section is to document:

- hardware behavior
- compatibility observations
- startup behavior
- revision comparisons
- signal measurements
- installation differences
- troubleshooting observations

Because ChipSlayer is still experimental, maintaining organized test records is an important part of the development process.

---

## Purpose of This Directory

The Test-Data section exists to:

- preserve validation history
- compare hardware revisions
- document console-specific behavior
- track known issues
- archive scope captures
- compare startup behavior
- improve repeatability between tests

---

## Directory Structure

The Test-Data folder is organized into several sections:

    Test-Data/
    ├── Console-Test-Logs/
    ├── Scope-Captures/
    ├── PS2Ident-Reports/
    └── Boot-Behavior-Notes/

Additional folders may be added as testing expands.

---

## Console-Test-Logs

### Purpose

This folder contains written observations and test results collected during hardware validation.

### Example Content

Possible contents include:

- startup observations
- compatibility notes
- installation comparisons
- revision-specific behavior
- troubleshooting notes
- console-specific anomalies

### Suggested File Naming

Examples:

    SCPH-70012-v0.2-TestLog.txt
    SCPH-75001-v0.3-Observations.txt
    SCPH-77001-BootBehavior.txt

---

## Scope-Captures

### Purpose

This folder stores oscilloscope captures and signal-analysis data.

### Typical Signals

Signals that may be analyzed include:

- reset-line behavior
- startup timing
- voltage transitions
- switch control behavior
- power sequencing
- signal ringing
- leakage observations

### Example File Types

Possible file types include:

- PNG images
- CSV waveform exports
- oscilloscope session files
- annotated screenshots

### Suggested File Naming

Examples:

    ResetLine-ColdBoot-v0.2.png
    StartupTiming-SCPH70012.csv
    AnalogSwitch-Test.png

---

## PS2Ident-Reports

### Purpose

This folder contains PS2Ident logs collected during testing.

### Typical Uses

PS2Ident reports may help compare:

- modchip enabled vs disabled
- ChipSlayer active vs bypassed
- motherboard revision behavior
- startup-state differences

### Suggested File Naming

Examples:

    SCPH-70012-ModBo-On.txt
    SCPH-70012-ModBo-Off.txt
    SCPH-70012-ChipSlayer-Enabled.txt
    SCPH-70012-ChipSlayer-Bypassed.txt

---

## Boot-Behavior-Notes

### Purpose

This folder stores startup observations and boot-behavior comparisons.

### Example Content

Possible contents include:

- cold boot observations
- warm reset behavior
- standby-to-power behavior
- inconsistent startup reports
- revision comparison notes
- troubleshooting observations

### Suggested File Naming

Examples:

    SCPH-75001-ColdBootNotes.txt
    SCPH-77001-WarmResetTest.txt
    v0.3-StartupComparison.txt

---

## Recommended Testing Information

When documenting a test, the following information is recommended:

| Field | Description |
|---|---|
| Console model | Example: SCPH-70012 |
| Motherboard revision | Example: GH-032-xx |
| Modchip type | Example: ModBo 5.0 |
| ChipSlayer revision | Example: v0.2 |
| Installation type | Prototype, permanent, test platform |
| Power conditions | OEM PSU, bench supply, USB-C PD |
| Test conditions | Enabled, disabled, bypassed |
| Results | Startup behavior and observations |
| Scope captures | If available |
| Additional notes | Anything unusual observed |

---

## Testing Philosophy

The project prioritizes:

- real-world testing
- repeated validation
- cross-revision comparison
- signal analysis
- installation repeatability

The goal is not simply to confirm functionality, but to better understand how PlayStation 2 hardware reacts under different electrical conditions.

---

## Important Notes

Not all consoles behave identically.

Observed behavior may vary due to:

- motherboard revision
- modchip revision
- installation quality
- signal integrity
- grounding
- power quality
- wiring length
- existing console damage

Testing results should always be interpreted carefully.

---

## Experimental Nature

Much of the data in this directory may involve:

- prototype hardware
- incomplete revisions
- temporary wiring
- experimental configurations
- partially validated concepts

Some findings may later be revised or disproven as testing continues.

---

## Suggested Future Expansion

Future additions to this directory may include:

- automated test procedures
- revision comparison charts
- long-term reliability data
- thermal observations
- additional console coverage
- alternate modchip testing
- startup timing analysis

---

## Repository Role

The Test-Data section is one of the most important parts of the ChipSlayer repository.

It serves as:

- a research archive
- a validation history
- a troubleshooting reference
- a compatibility reference
- a hardware development record

---

## Final Notes

Testing and validation are ongoing.

As the project evolves, this directory should continue expanding with additional observations, comparisons, and technical analysis.
