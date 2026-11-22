# Argus Software

Firmware for the Argus keylogger, running bare-metal on the CH32V003 RISC-V MCU.
It sniffs the tapped USB data lines, decodes keystrokes, logs them to flash, and
replays them to the user on a chosen key combination.

## Overview

_TODO: short description of the firmware and its responsibilities._

## How It Works

The firmware pipeline, end to end:

1. **Capture** — sample the USB D+/D− lines tapped inline on the cable.
2. **Decode** — reconstruct USB HID reports into keystrokes.
3. **Log** — append captured keys to on-chip flash.
4. **Replay** — on a trigger key combination, play the stored keys back to the user.

_TODO: fill in the details of each stage._

## Build

_TODO: how to compile the firmware._

## Flash

_TODO: how to program the board over single-wire debug (DBG / SWIO pad)._

## Configuration

_TODO: where the trigger key combination and flash-layout constants are defined._

## Memory Constraints

The CH32V003 provides only **16 KB flash** and **2 KB SRAM**, which bounds how
much can be logged and how the capture buffer is sized.

_TODO: notes on flash budget and log capacity._

## Project Layout

_TODO: source tree map once the firmware sources are in place._
