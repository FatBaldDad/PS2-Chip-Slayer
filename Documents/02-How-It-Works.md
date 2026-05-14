# How ChipSlayer Works

## Introduction

ChipSlayer is designed to control how a PlayStation 2 modchip interacts with the console by selectively isolating portions of the modchip circuitry from the system.

The project was developed after observing that many PS2 modchips continue to influence console behavior even when partially disconnected or "disabled." Simply removing power from the modchip was not always enough to completely eliminate interaction with the console.

ChipSlayer attempts to provide a cleaner and more controlled method of isolating the modchip while preserving installation simplicity.

---

# Core Concept

The main idea behind ChipSlayer is:

> Allow the modchip to remain physically installed while electronically reducing or removing its influence on the console.

This is accomplished by controlling critical connections between the modchip and the PlayStation 2 motherboard.

---

# Why This Matters

During testing, several important behaviors were observed:

- Some consoles would fail to boot properly if certain modchip lines remained connected
- Some modchips continued to partially interact with the console even when their main power was removed
- Reset-line behavior could interfere with normal startup timing
- Different motherboard revisions behaved differently
- Some installs became unstable depending on pull-up and pull-down interactions

ChipSlayer was developed to help manage these interactions in a more predictable way.

---

# Signals of Interest

Current development has primarily focused on controlling:

## Modchip Reset

The reset connection between the modchip and the console can strongly influence startup behavior.

ChipSlayer can isolate or switch the reset interaction so the modchip no longer affects the console when disabled.

---

## Modchip Ground

Ground isolation testing was performed because some modchips still influenced console behavior through signal lines even when reset or power conditions changed.

ChipSlayer experiments with selective ground isolation behavior to reduce unwanted interaction.

---

## Signal Integrity

Special attention has been given to:

- Pull-up resistance
- Leakage current
- Floating states
- High-impedance behavior
- Startup timing
- Logic-level interaction

The project attempts to avoid placing unnecessary electrical load on critical PlayStation 2 signals.

---

# Reset-Line Considerations

One important discovery during development was that reset behavior on PlayStation 2 consoles can be extremely sensitive.

The reset signal used by the modchip is tied into the console supervisory circuitry.

Depending on the motherboard revision:

- Older consoles may route reset behavior through SysCon circuitry
- Newer consoles route behavior through MechaCon circuitry
- Timing and electrical behavior can vary between revisions

Because of this, ChipSlayer development has focused heavily on preventing unintended loading or pull conditions on the reset line.

---

# High-Impedance Switching

A major design goal of ChipSlayer is maintaining a high-impedance state whenever possible.

This helps:

- Reduce loading on console signals
- Prevent unwanted pull-down behavior
- Improve compatibility between board revisions
- Minimize signal interference
- Allow the console to behave more normally when the modchip is disabled

Several switching methods and logic approaches have been explored during development.

---

# Switching Methods

Multiple hardware approaches have been investigated during development, including:

- Transistor-based switching
- Open-drain logic
- Analog switching
- MOSFET isolation
- Buffered logic control

Different revisions of ChipSlayer may use different methods depending on testing results and hardware goals.

---

# Modchip Behavior

ChipSlayer does not modify modchip firmware.

Instead, it works externally by controlling how the installed modchip electrically interacts with the PlayStation 2 motherboard.

This means behavior may vary depending on:

- Modchip model
- Firmware revision
- Installation quality
- Console motherboard revision
- Console condition

---

# Console Compatibility

Testing has primarily focused on PS2 Slim consoles, especially:

| Model Family | Status |
|---|---|
| SCPH-700xx | Active testing |
| SCPH-750xx | Active testing |
| SCPH-770xx | Active testing |

Additional testing may expand into other revisions over time.

---

# Experimental Nature

ChipSlayer remains an experimental hardware project.

Not all motherboard revisions behave identically.

Some observed behaviors include:

- Boot instability
- Delayed startup
- Reset sensitivity
- Different behavior between consoles with the same model number
- Variations between modchip revisions

Because of this, extensive testing and revision tracking are maintained throughout this repository.

---

# Design Priorities

Current development priorities include:

## Stability

Ensuring the console boots consistently with the modchip enabled or disabled.

## Low Signal Impact

Reducing electrical influence on console circuitry.

## Compact Installation

Keeping the board small and practical for internal installation.

## Repeatability

Making installation behavior more predictable across consoles.

## Documentation

Tracking revisions, testing results, and compatibility observations.

---

# Current Development Direction

Current work is focused on:

- Refining reset isolation behavior
- Improving high-impedance switching characteristics
- Reducing unintended leakage paths
- Improving compatibility across PS2 Slim revisions
- Documenting real-world installation behavior

---

# Future Possibilities

Potential future development may include:

- Additional switching modes
- Enhanced diagnostic capability
- Integrated status indication
- Advanced logic control
- Expanded motherboard compatibility
- Combined functionality with other PS2 hardware projects

---

# Important Notes

ChipSlayer is not intended to bypass repair or troubleshooting procedures.

If a console has:
- damaged traces
- poor soldering
- failing capacitors
- unstable power rails
- damaged modchip installs

ChipSlayer may not resolve those underlying issues.

Proper console servicing and installation quality remain critical.

---

# Disclaimer

This project is experimental and intended for hobbyist hardware development and research purposes.

Installation requires modification of PlayStation 2 hardware and should only be performed by individuals comfortable working with fine-pitch electronics and console repair.
