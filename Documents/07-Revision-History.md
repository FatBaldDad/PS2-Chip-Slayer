# Revision History

## Introduction

This document tracks the development history, hardware revisions, testing milestones, and major design changes for the ChipSlayer project.

Because ChipSlayer is still under active development, revision tracking is important for:

- identifying design changes
- comparing test results
- documenting hardware evolution
- tracking known issues
- validating improvements between revisions

This document should evolve as additional hardware revisions are produced and tested.

---

## Revision Naming Convention

ChipSlayer revisions currently follow a simple versioning format:

| Revision Type | Example |
|---|---|
| Early concept revision | v0.1 |
| Prototype revision | v0.2 |
| Experimental revision | v0.3 |
| Pre-production revision | v0.9 |
| Production candidate | v1.0 |

Revision numbering may evolve as the project matures.

---

## Revision Status Key

| Status | Meaning |
|---|---|
| Concept | Initial design or theory stage |
| Prototype | Physical hardware produced |
| Testing | Active validation and troubleshooting |
| Stable | Working consistently in testing |
| Retired | No longer actively used |
| Experimental | Used only for testing new ideas |

---

# Revision Timeline

| Revision | Status | Summary |
|---|---|---|
| v0.1 | Retired | Initial concept revision |
| v0.2 | Testing | Early reset isolation testing |
| v0.3 | Experimental | Alternate switching behavior testing |
| v0.4 | Experimental | High-impedance refinement testing |
| v1.0 | Planned | Future production candidate |

---

# Revision Details

## v0.1 — Initial Concept Revision

### Status

Retired

### Purpose

The first revision focused on validating the core concept of selectively isolating modchip behavior from the PlayStation 2 console.

### Main Goals

- prove the switching concept
- test reset-line interaction
- evaluate console startup behavior
- determine whether selective isolation was practical

### Characteristics

- hand-built prototype style
- simple routing
- minimal optimization
- heavy use of test wiring
- focused on experimentation rather than appearance

### Observations

Initial testing confirmed:

- reset behavior strongly affects startup
- some consoles are highly sensitive to loading
- partial modchip isolation changes console behavior
- motherboard revisions behave differently

### Outcome

The revision successfully validated the general project direction but required additional refinement.

---

## v0.2 — Early Reset Isolation Revision

### Status

Testing

### Purpose

This revision focused more heavily on reset-line isolation and switching behavior.

### Main Goals

- improve startup consistency
- reduce reset-line loading
- test cleaner switching methods
- improve repeatability between installs

### Design Changes

Possible changes included:

- alternate resistor values
- revised switching topology
- cleaner signal routing
- improved grounding layout
- revised control logic

### Observations

Testing suggested:

- some consoles remained highly sensitive
- startup behavior improved in certain cases
- wiring quality still strongly affected results
- reset-line behavior remained one of the largest variables

### Current Notes

This revision remains important for comparison testing.

---

## v0.3 — Alternate Switching Revision

### Status

Experimental

### Purpose

This revision explored alternate switching approaches intended to improve high-impedance behavior and reduce unintended interaction with the reset line.

### Main Goals

- reduce leakage paths
- improve switch isolation
- reduce electrical loading
- refine startup-state behavior

### Areas of Investigation

- analog switching
- transistor switching
- buffered logic
- pull-up optimization
- control-state stability

### Observations

Some improvements were observed, but additional testing is still required.

Behavior continued to vary between motherboard revisions.

---

## v0.4 — High-Impedance Refinement Revision

### Status

Experimental

### Purpose

This revision focused on improving inactive-state electrical behavior.

### Main Goals

- minimize line loading
- improve idle-state behavior
- reduce unintended interaction
- improve reset-line stability

### Areas of Investigation

- open-drain behavior
- high-impedance switching
- floating-state control
- startup control timing
- reduced leakage current

### Current Notes

This revision remains under evaluation.

---

## v1.0 — Planned Production Candidate

### Status

Planned

### Goals

The future v1.0 revision is intended to represent a more stable and production-ready version of ChipSlayer.

### Planned Focus Areas

- stable startup behavior
- improved compatibility
- simplified installation
- compact layout
- improved documentation
- repeatable installation quality
- refined switching behavior

### Notes

Features and design details may change significantly before reaching production status.

---

# Hardware Evolution

The project has evolved through several major areas of investigation.

---

## Reset-Line Isolation

One of the largest development areas has involved understanding and refining reset-line interaction.

Testing has shown:

- some consoles are extremely sensitive
- small electrical loads matter
- startup timing varies between revisions
- different switching methods behave differently

---

## High-Impedance Switching

Several revisions focused on improving inactive-state electrical behavior.

Goals included:

- minimizing leakage
- reducing loading
- improving compatibility
- reducing startup interference

---

## Ground Isolation Testing

Ground isolation experiments were explored to determine whether unwanted interaction could be reduced further.

Results remain mixed and may depend heavily on:

- console revision
- modchip design
- signal paths
- installation quality

---

## Installation Refinement

As revisions progressed, installation goals expanded to include:

- cleaner routing
- reduced wire count
- improved physical fitment
- better serviceability
- improved repeatability

---

# Testing Progression

Testing evolved alongside hardware revisions.

---

## Early Testing

Focused on:

- proving the concept
- observing startup behavior
- identifying signal sensitivity

---

## Mid-Stage Testing

Focused on:

- switch behavior
- high-impedance performance
- resistor optimization
- comparative boot testing

---

## Current Testing

Current work focuses on:

- cross-revision compatibility
- startup reliability
- installation consistency
- signal integrity refinement
- long-term behavior observation

---

# Revision Documentation

Each revision may eventually include:

| Item | Description |
|---|---|
| Board photos | Top and bottom images |
| Schematics | Revision-specific diagrams |
| Testing notes | Boot behavior and observations |
| Scope captures | Signal measurements |
| Known issues | Revision-specific problems |
| Installation notes | Wiring and layout changes |

---

# Suggested Repository Organization

Revision-specific material may eventually be organized like this:

    Hardware/
    ├── Revision-v0.1/
    ├── Revision-v0.2/
    ├── Revision-v0.3/
    └── Revision-v1.0/

Each revision folder may contain:

- schematics
- photos
- notes
- test results
- installation examples

---

# Future Revision Goals

Future revisions may explore:

- simplified switching logic
- reduced component count
- alternate switch devices
- improved startup-state control
- additional motherboard compatibility
- diagnostic indicators
- alternate installation methods

---

# Development Philosophy

ChipSlayer development prioritizes:

- real-world testing
- electrical behavior analysis
- repeatability
- serviceability
- careful revision tracking

The project intentionally evolves slowly to better understand how different PlayStation 2 revisions respond to the hardware.

---

# Final Notes

Revision tracking is one of the most important parts of the ChipSlayer project.

As testing expands, this document should continue evolving alongside the hardware itself.
