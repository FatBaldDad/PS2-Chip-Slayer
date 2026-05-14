# Installation Examples

## Introduction

This document provides general installation examples, observations, and layout concepts for the ChipSlayer project.

Because PlayStation 2 motherboard revisions, modchip installs, and wiring quality can vary significantly, these examples should be treated as reference material rather than strict installation instructions.

ChipSlayer installations are still considered experimental.

---

# Important Disclaimer

ChipSlayer installation requires:

- Fine-pitch soldering
- PlayStation 2 motherboard modification
- Understanding of modchip wiring
- Understanding of signal integrity considerations

Improper installation may damage:
- the console
- the modchip
- motherboard traces
- surrounding components

Use at your own risk.

---

# General Installation Philosophy

The overall goal of ChipSlayer installation is to:

- Keep wiring clean
- Minimize signal interference
- Reduce wire length where possible
- Avoid unnecessary loading on console signals
- Preserve serviceability
- Maintain repeatable installation behavior

---

# Typical Installation Location

Current prototype installations are generally placed near:

- the installed modchip
- reset-line access points
- convenient ground reference points

Placement may vary depending on:
- console revision
- modchip type
- internal modifications
- available physical space

---

# Common Installation Styles

## Inline Reset Switching

One installation method places ChipSlayer inline with the modchip reset connection.

### Purpose

This allows controlled isolation of the modchip reset behavior from the console.

### Typical Goals

- Reduce reset-line interference
- Allow controlled modchip disabling
- Maintain cleaner startup behavior

---

## Ground Isolation Approach

Some revisions of ChipSlayer also experiment with selective modchip ground isolation.

### Purpose

This testing investigates whether removing ground reference paths reduces unwanted interaction between the modchip and the console.

### Notes

Ground isolation behavior may vary significantly depending on:
- modchip design
- console revision
- signal leakage paths
- installation quality

---

# Example Installation Concepts

## Example 1 — Compact Slim Install

### Console

- SCPH-700xx

### Modchip

- ModBo 5.0

### Goals

- Minimal added wiring
- Compact installation
- Easy serviceability

### Notes

This configuration focuses primarily on reset-line isolation while keeping the board physically close to the modchip installation.

---

## Example 2 — Testing Platform Install

### Console

- SCPH-750xx

### Goals

- Rapid testing access
- Easy probing
- Scope capture support

### Notes

This style of installation may intentionally prioritize accessibility over appearance.

Additional wiring may be exposed for testing purposes.

---

## Example 3 — Integrated Build

### Console

- SCPH-770xx

### Goals

- Permanent internal installation
- Compact routing
- Reduced visible wiring

### Notes

Integrated builds may combine ChipSlayer with:

- HDMI modifications
- BlueRetro installs
- SD2PSX integration
- custom internal layouts

---

# Wiring Considerations

## Keep Wires Short

Excessively long wires may increase:

- noise pickup
- ringing
- startup instability
- signal integrity problems

---

## Avoid Excessive Heat

PlayStation 2 motherboard pads can lift easily if overheated.

Use proper soldering technique and avoid prolonged heat exposure.

---

## Maintain Good Grounding

Reliable ground connections are important for stable operation.

Poor grounding may produce:
- unstable behavior
- inconsistent startup
- false triggering
- intermittent operation

---

## Route Carefully

Avoid routing wires:
- over sharp edges
- under pressure points
- near moving components
- near high-noise areas when possible

---

# Testing During Installation

It is recommended to test the console at multiple stages during installation.

---

## Suggested Testing Flow

| Stage | Recommended Test |
|---|---|
| Before installation | Verify console operation |
| After modchip install | Confirm normal boot behavior |
| After ChipSlayer install | Confirm console still boots |
| After wiring cleanup | Repeat boot testing |
| Final assembly | Long-duration testing |

---

# Boot Testing

Repeated boot testing is strongly recommended.

Suggested tests include:

- Cold boots
- Warm resets
- Rapid power cycles
- Modchip enabled operation
- Modchip disabled operation

---

# Physical Mounting

Current prototype boards may be mounted using:

- Kapton tape
- double-sided foam tape
- custom brackets
- insulated adhesive methods

Mounting methods should:
- avoid shorts
- prevent movement
- allow future servicing

---

# Prototype Installations

Prototype installations may differ significantly from future production hardware.

Current development revisions may include:

- exposed test points
- temporary wiring
- bodge wires
- alternate switching methods
- hand-modified traces

This is expected during active development.

---

# Photos and Reference Images

Reference images may eventually be added to:

```text
Images/
├── Install-Examples/
├── Prototype-Revisions/
└── Board-Photos/
