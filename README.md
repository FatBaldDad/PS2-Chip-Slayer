# FBD PS2 ChipSlayer

## Introduction

ChipSlayer is an experimental PlayStation 2 hardware interface board designed to better control how installed modchips interact with the console.

The project was created after observing that many PlayStation 2 modchips continue influencing console behavior even when partially disabled or disconnected. Simply removing power from the modchip was not always enough to fully isolate it from the system.

ChipSlayer focuses primarily on:

- reset-line interaction
- modchip isolation behavior
- startup consistency
- high-impedance switching
- minimizing electrical loading on sensitive console signals

This repository serves as the primary:

- documentation hub
- testing archive
- revision tracker
- research reference
- compatibility database

for the ChipSlayer project.

---

# Project Status

ChipSlayer is currently considered:

| Status | Meaning |
|---|---|
| Experimental | Active hardware development and testing |
| Prototype Hardware Exists | Physical revisions have been manufactured and tested |
| Under Active Investigation | Compatibility and behavior still being explored |
| Not Fully Open Hardware | Production files are not currently publicly released |

---

# Project Goals

The primary goals of ChipSlayer are:

- provide cleaner modchip enable/disable behavior
- reduce unintended modchip interaction
- improve startup consistency
- minimize reset-line loading
- improve repeatability between installations
- document console behavior across revisions
- maintain a research archive of findings and testing

---

# Core Concept

ChipSlayer is designed around the idea that:

> A modchip may continue influencing console behavior even when partially disabled.

Rather than simply removing power, ChipSlayer investigates more controlled methods of electrically isolating modchip behavior from the console.

Current development focuses heavily on:

- reset-line behavior
- startup-state interaction
- high-impedance switching
- signal integrity
- grounding interaction

---

# Primary Testing Platforms

Current development has primarily focused on PlayStation 2 Slim systems.

| Console Family | Status |
|---|---|
| SCPH-700xx | Primary development platform |
| SCPH-750xx | Active testing |
| SCPH-770xx | Active testing |
| SCPH-790xx | Limited testing |
| SCPH-900xx | Future investigation |
| PS2 Fat Models | Future investigation |

---

# Modchip Focus

Current testing has primarily involved:

| Modchip | Status |
|---|---|
| ModBo 5.0 | Primary testing target |
| Matrix-derived clones | Partial testing |

Additional modchip support may be explored later.

---

# Repository Structure

The repository is organized into several primary sections:

    .
    ├── Documents/
    ├── Hardware/
    ├── Images/
    ├── References/
    ├── Store-Links/
    ├── Test-Data/
    ├── CHANGELOG.md
    ├── LICENSE
    └── README.md

---

# Documentation Sections

## Documents/

Contains project documentation including:

- project overview
- hardware concepts
- compatibility notes
- installation examples
- testing methodology
- known issues
- revision history
- future development plans

---

## Hardware/

Contains hardware-related files and references.

Possible contents may include:

- schematics
- PCB revisions
- prototype layouts
- BOM references
- board photos

Some production manufacturing files may not be publicly released.

---

## Images/

Contains project-related images such as:

- board photos
- installation examples
- prototype revisions
- scope captures
- testing setups

---

## References/

Contains supporting technical information and related research including:

- datasheets
- hardware notes
- related projects
- signal research
- component references

---

## Test-Data/

Contains validation and testing information including:

- console logs
- startup observations
- PS2Ident reports
- scope captures
- troubleshooting notes

---

# Important Development Areas

Current areas of investigation include:

| Area | Focus |
|---|---|
| Reset-line behavior | Startup consistency |
| High-impedance switching | Reduced loading |
| Ground isolation | Reduced unwanted interaction |
| Signal integrity | Improved stability |
| Cross-revision testing | Broader compatibility |
| Installation refinement | Cleaner installs |

---

# Important Notes

Different PlayStation 2 revisions may behave differently.

Observed behavior can vary due to:

- motherboard revision
- modchip revision
- installation quality
- wiring length
- grounding quality
- power conditions
- signal integrity
- existing console damage

Testing on one console does not guarantee identical behavior on another.

---

# Experimental Nature

ChipSlayer remains an experimental hardware project.

Some revisions shown within this repository may include:

- temporary wiring
- bodge modifications
- incomplete layouts
- prototype-only features
- experimental switching methods

Behavior may evolve significantly as testing continues.

---

# Hardware Availability

This repository currently exists primarily for:

- documentation
- research
- revision tracking
- compatibility analysis
- testing history

ChipSlayer hardware is not currently intended to be fully open-source hardware.

Production-ready manufacturing files and commercial production data may not be publicly released at this time.

---

# Official Links

## FBD Retro Game Website

https://retrogame.fatbalddad.com/

## Etsy Store

https://www.etsy.com/shop/FBDRetroGame

## eBay Store

https://www.ebay.com/usr/fatbalddad

---

# Related Projects

ChipSlayer development exists within a broader PlayStation 2 hardware ecosystem including:

- modchip development
- BlueRetro
- OPL
- PS2Ident
- HDMI modifications
- SD2PSX/MMCE projects
- custom power-management systems
- console preservation efforts

Additional related information can be found in:

    References/
    └── Related-Projects.md

---

# Current Known Issues

Current known issues and areas still under investigation include:

- reset-line sensitivity
- startup inconsistency on some revisions
- incomplete Deckard testing
- incomplete cross-modchip validation
- ground isolation behavior
- high-impedance refinement

Additional information is documented in:

    Documents/
    └── 06-Known-Issues.md

---

# Future Development

Future work may include:

- improved switching behavior
- reduced component count
- simplified installation
- expanded compatibility testing
- diagnostic features
- improved miniaturization
- alternate isolation methods

Additional details are documented in:

    Documents/
    └── 08-Future-Development.md

---

# Disclaimer

ChipSlayer is an experimental hardware modification project.

Installation requires modification of PlayStation 2 hardware and should only be attempted by individuals familiar with:

- fine-pitch soldering
- console repair
- electronics troubleshooting
- signal integrity considerations

No guarantees are provided regarding:

- compatibility
- reliability
- functionality
- long-term stability

Use at your own risk.

---

# Credits

Developed and documented by:

**Fat Bald Dad (FBD Retro Game)**

Additional contributors, testers, and collaborators may be credited throughout the repository as development continues.

---

# Final Notes

ChipSlayer is as much a research and documentation effort as it is a hardware project.

The long-term goal is to better understand how PlayStation 2 modchips interact with console hardware and to develop cleaner, more controlled methods of managing that interaction.
