# Known Issues

## Introduction

This document tracks known issues, observed behaviors, limitations, and areas that require additional testing for the ChipSlayer project.

ChipSlayer is still considered experimental hardware. Some issues may be caused by the board design, while others may be caused by console revision differences, modchip behavior, wiring quality, or unrelated console faults.

---

## Issue Status Key

| Status | Meaning |
|---|---|
| Open | Issue is known and still being investigated |
| Testing | Possible solution or workaround is being tested |
| Resolved | Issue appears corrected in a later revision |
| Not Reproducible | Issue was seen once or reported, but has not been repeated |
| By Design | Behavior is expected based on the current design |

---

## Known Issue Summary

| Issue | Status | Notes |
|---|---|---|
| Console does not start when reset line is connected | Open | Reset-line loading or switching behavior may be involved |
| Reset line appears pulled high or held in an unexpected state | Open | Needs additional scope testing |
| Behavior changes between motherboard revisions | Open | Expected due to PS2 hardware differences |
| Modchip may still influence console behavior when partially disabled | Open | Isolation method may need revision-specific validation |
| Ground isolation behavior is not fully characterized | Testing | Results may vary by modchip and install |
| Long wire runs may cause unstable behavior | By Design | Installation quality and routing matter |
| Deckard compatibility is unknown | Open | Not currently a primary target |

---

## Console Does Not Start When Reset Line Is Connected

### Status

Open

### Description

In some test configurations, the console may fail to start when ChipSlayer is connected to the modchip reset input or reset-related wiring.

This may appear as:

- no startup
- delayed startup
- inconsistent power-on behavior
- console only starting after the reset connection is removed

### Possible Causes

Possible causes include:

- reset-line loading
- incorrect pull-up or pull-down behavior
- analog switch interaction
- floating control input
- modchip input leakage
- incorrect wiring
- motherboard revision sensitivity

### Current Notes

This issue is one of the main reasons continued testing is needed.

Reset behavior on PlayStation 2 Slim consoles can be sensitive, and small electrical changes may affect startup behavior.

### Suggested Testing

Recommended checks include:

- verify reset wiring
- confirm no solder bridges
- measure reset-line voltage during standby and startup
- scope the reset line during power-on
- test with the modchip disconnected
- test with ChipSlayer bypassed
- compare enabled and disabled states

---

## Reset Line Appears Pulled High or Held Unexpectedly

### Status

Open

### Description

Some test behavior suggests that the reset line or reset-related input may be held in a state that affects normal startup.

This may be caused by interaction between:

- console reset circuitry
- modchip reset input
- ChipSlayer switching circuit
- pull-up resistors
- leakage paths

### Possible Symptoms

- console fails to boot
- console behaves differently with ChipSlayer connected
- reset input does not return to expected idle state
- reset behavior changes depending on switch position

### Suggested Testing

Recommended checks include:

- measure reset-line idle voltage
- check reset-line behavior during power-on
- compare connected and disconnected states
- test different pull-up values if applicable
- verify switch control logic
- inspect for unintended continuity paths

---

## Analog Switch Interaction

### Status

Testing

### Description

Some revisions may use an analog switch or signal switch to isolate reset-related connections.

The switching device itself may introduce:

- on-resistance
- off-state leakage
- input capacitance
- control-input sensitivity
- startup-state uncertainty

### Possible Symptoms

- console starts inconsistently
- reset line does not behave as expected
- switch state affects console boot behavior
- behavior changes when control input is floating or weakly held

### Suggested Testing

Recommended checks include:

- confirm control pin is never floating
- verify switch enable logic
- verify switch power rail
- measure voltage on both sides of the switched signal
- test with the switch bypassed
- compare behavior with direct wiring

---

## Ground Isolation Behavior Is Not Fully Characterized

### Status

Testing

### Description

Ground isolation has been explored as part of ChipSlayer development, but behavior may vary depending on the modchip and console revision.

Some modchips may still interact with the console through signal lines even when their ground or reset behavior is modified.

### Possible Variables

- modchip design
- signal-line protection diodes
- backfeed paths
- reset wiring
- power wiring
- motherboard revision

### Current Notes

Ground isolation should be treated as experimental until more testing is completed.

---

## Behavior Changes Between Motherboard Revisions

### Status

Open

### Description

Different PlayStation 2 motherboard revisions may respond differently to the same ChipSlayer hardware revision.

This is expected because PS2 Slim hardware changed across model families.

### Affected Areas

Possible areas of difference include:

- reset behavior
- startup timing
- MechaCon/SysCon behavior
- modchip interaction
- power sequencing
- signal tolerance

### Current Notes

Compatibility must be validated on real consoles and not assumed based only on model number.

---

## Modchip Still Influences Console When Disabled

### Status

Open

### Description

A modchip may still influence console behavior even when it appears to be disabled.

This can happen if the modchip remains electrically connected through:

- signal wires
- protection diodes
- ground paths
- power leakage paths
- reset wiring
- BIOS or controller lines

### Possible Symptoms

- console does not behave like a fully stock console
- boot behavior changes with the chip physically installed
- disabling only one signal is not enough
- behavior depends on the modchip model

### Current Notes

ChipSlayer attempts to reduce this behavior, but complete electrical isolation may not always be possible without disconnecting more signals.

---

## Long Wire Runs May Cause Instability

### Status

By Design

### Description

Long wires may introduce signal integrity problems.

This is especially important for reset-related wiring and any signal that affects startup behavior.

### Possible Symptoms

- inconsistent startup
- random boot failure
- noise pickup
- ringing
- sensitivity to wire placement

### Recommended Practice

Keep wiring:

- short
- clean
- routed away from noisy areas
- mechanically secured
- free from unnecessary loops

---

## Poor Installation Quality Can Mimic Board Issues

### Status

By Design

### Description

Installation quality strongly affects test results.

A poor solder joint, lifted pad, bridged pin, or weak ground connection may look like a ChipSlayer design issue.

### Common Installation Problems

- cold solder joints
- solder bridges
- lifted pads
- broken vias
- damaged modchip wiring
- weak ground points
- stressed wires

### Recommended Practice

Before assuming a design issue, verify:

- continuity
- no shorts
- clean solder joints
- correct wire routing
- stable power
- correct switch behavior

---

## Deckard Compatibility Unknown

### Status

Open

### Description

SCPH-900xx Deckard Slim consoles are not currently a primary development target.

Deckard consoles use different internal architecture compared to earlier PS2 Slim models.

### Current Status

Compatibility is unknown.

### Notes

Deckard testing should not be assumed until specific validation is completed.

---

## PS2 Fat Compatibility Unknown

### Status

Open

### Description

ChipSlayer has not yet been fully validated on PS2 Fat consoles.

### Possible Future Targets

Future testing may include:

- SCPH-300xx
- SCPH-390xx
- SCPH-500xx

### Current Status

Compatibility is unknown.

---

## Known Limitations

Current known limitations include:

- limited motherboard coverage
- limited modchip variety
- incomplete long-term testing
- incomplete Deckard testing
- no guarantee of full stock-console behavior when disabled
- installation-sensitive behavior

---

## Troubleshooting Checklist

If an issue occurs, check the following:

- confirm console worked before installation
- confirm modchip worked before ChipSlayer installation
- inspect all solder joints
- check for solder bridges
- verify reset wiring
- verify ground wiring
- verify switch position
- verify power rails
- test with ChipSlayer bypassed
- test with modchip reset disconnected
- compare behavior between enabled and disabled states

---

## Reporting Issues

When documenting a new issue, include:

| Field | Information |
|---|---|
| Console model | Example: SCPH-70012 |
| Motherboard revision | Example: GH-032-xx |
| Modchip | Example: ModBo 5.0 |
| ChipSlayer revision | Example: v0.2 |
| Install type | Prototype, permanent, test platform |
| Symptoms | What happened |
| Test conditions | Enabled, disabled, bypassed, cold boot, warm boot |
| Measurements | Voltage readings or scope captures if available |
| Photos | Install photos if useful |
| Status | Open, testing, resolved, not reproducible |

---

## Future Work

Future revisions may focus on:

- improved reset isolation
- reduced leakage paths
- simplified wiring
- better startup-state control
- expanded motherboard testing
- improved diagnostic test points
- clearer installation documentation

---

## Final Notes

Known issues are expected during active hardware development.

This document should be updated as testing continues and new hardware revisions are evaluated.
