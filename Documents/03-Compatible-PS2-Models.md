# Compatible PS2 Models

## Introduction

ChipSlayer development has primarily focused on PlayStation 2 Slim consoles using commonly installed aftermarket modchips.

This document tracks known compatibility observations, testing status, and important notes regarding different PlayStation 2 motherboard revisions.

Because PlayStation 2 hardware revisions can vary significantly, compatibility should always be considered experimental unless specifically validated.

---

# Important Notes

Compatibility depends on several factors, including:

- Console motherboard revision
- Modchip type
- Modchip firmware
- Installation quality
- Existing console modifications
- Signal integrity
- Power stability
- Reset-line behavior

Even consoles within the same model family may behave differently.

---

# Current Testing Focus

Current development has primarily focused on:

| Console Family | Status |
|---|---|
| SCPH-700xx | Primary development target |
| SCPH-750xx | Active testing |
| SCPH-770xx | Active testing |

---

# Compatibility Table

| Console Model | Board Family | Status | Notes |
|---|---|---|---|
| SCPH-700xx | Early Slim | Active Testing | Primary development platform |
| SCPH-750xx | Slim | Active Testing | Reset behavior differs from some 70K units |
| SCPH-770xx | Slim | Active Testing | Additional validation ongoing |
| SCPH-790xx | Late Slim | Limited Testing | Future testing planned |
| SCPH-900xx | Deckard Slim | Unknown | Not currently targeted |
| PS2 Fat Models | Various | Not Tested | Future evaluation possible |

---

# SCPH-700xx

## Current Status

The SCPH-700xx series has been one of the primary development targets for ChipSlayer.

These consoles are commonly modified and have shown several interesting reset and modchip interaction behaviors during testing.

---

## Observations

Observed behaviors on some 700xx systems include:

- Reset sensitivity
- Modchip interaction during startup
- Boot behavior changes depending on reset loading
- Differences between modchip enabled and disabled states

---

## Notes

Some 700xx systems appear more sensitive to:

- Pull-up resistor values
- Leakage current
- Reset timing
- High-impedance switching behavior

These systems remain one of the most important testing platforms for the project.

---

# SCPH-750xx

## Current Status

The SCPH-750xx family is under active testing.

These systems may behave differently than some earlier Slim revisions regarding reset behavior and startup timing.

---

## Observations

Current testing suggests:

- Some reset interactions differ from early Slim models
- Startup behavior may be less tolerant of loading conditions
- Certain modchip configurations behave differently compared to 700xx systems

Additional testing is ongoing.

---

# SCPH-770xx

## Current Status

Testing is ongoing on SCPH-770xx systems.

These consoles remain important because they represent later non-Deckard Slim hardware.

---

## Observations

Current observations include:

- Similar behavior to some 750xx systems
- Possible differences in reset-line tolerance
- Additional testing required for long-term stability validation

---

# SCPH-790xx

## Current Status

Limited testing has been performed.

The SCPH-790xx family is of interest because of its lower power consumption and popularity in highly modified systems.

---

## Future Goals

Future testing may focus on:

- Boot stability
- Modchip compatibility
- Reset-line interaction
- High-impedance switching behavior

---

# SCPH-900xx (Deckard)

## Current Status

Deckard systems are not currently a primary development target.

These systems use significantly different hardware architecture compared to earlier Slim revisions.

---

## Important Notes

Compatibility should currently be considered unknown.

Additional research is required before official support can be claimed.

---

# PS2 Fat Consoles

## Current Status

Fat PlayStation 2 systems have not yet been fully evaluated.

---

## Possible Future Support

Future testing may include:

- SCPH-300xx
- SCPH-390xx
- SCPH-500xx

Compatibility is currently unknown.

---

# Modchip Compatibility

ChipSlayer development has primarily focused on commonly installed PS2 modchips.

Current testing has mainly involved:

| Modchip | Status |
|---|---|
| ModBo 5.0 | Primary testing target |
| Matrix-derived clones | Partial testing |
| Other modchips | Unknown |

---

# Installation Variables

Several installation variables can strongly affect compatibility:

## Wire Length

Longer wires may increase signal integrity issues.

## Ground Quality

Poor grounding can introduce instability.

## Reset Wiring

Reset-line routing and loading are especially critical.

## Power Stability

Unstable power rails may produce inconsistent results.

## Existing Console Damage

Damaged traces or poor prior installs can affect testing outcomes.

---

# Known Unknowns

Several areas still require additional research:

- Full Deckard compatibility
- Cross-region motherboard behavior
- Differences between modchip firmware revisions
- Long-term stability across all Slim revisions
- Behavior under unusual boot conditions

---

# Testing Methodology

Compatibility testing generally includes:

- Cold boot testing
- Warm reset testing
- Modchip enable/disable testing
- Repeated boot-cycle validation
- Long-duration stability observation
- Signal integrity analysis
- Console behavior comparison

Additional documentation may be included elsewhere within this repository.

---

# Reporting Compatibility Results

As testing expands, compatibility findings may be added to:

- Revision notes
- Testing logs
- Installation examples
- Scope captures
- Known issues documentation

---

# Community Feedback

Community testing and observations may eventually help expand compatibility knowledge.

However, all unofficial testing should be treated as informational until validated internally.

---

# Disclaimer

Compatibility information in this document reflects ongoing experimental development and testing.

No compatibility guarantees are currently provided.

Use at your own risk.
