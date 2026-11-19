# Argus

[![GitHub tag (with filter)](https://img.shields.io/github/v/tag/PanBabinicz/argus?style=plastic&label=latest)](https://github.com/PanBabinicz/argus/releases/latest)

> **Argus** is a tiny keylogger built around the [CH32V003](https://www.wch-ic.com/products/CH32V003.html),
> a low-cost 32-bit RISC-V microcontroller. It captures keystrokes and discreetly
> logs them to flash, all from a minimal footprint built on bare-metal firmware
> and a custom PCB.

> [!NOTE]
> **Please bear in mind that the workspace was primarily created for enjoyment
> and educational endeavors.**

## ✨ Features

- Inline USB tap — wires into the cable's physical D+/D− lines, sitting between keyboard and host.
- Captures keystrokes by sniffing the USB data lines and logs them to on-chip flash.
- Runs on a bare-metal [CH32V003](https://www.wch-ic.com/products/CH32V003.html) 32-bit RISC-V MCU clocked by a 24 MHz crystal.
- Powered straight from the USB +5 V rail — no battery needed.
- Replays the captured keystrokes back to the user on a chosen key combination.
- On-board button for reset.
- Tiny two-layer PCB that hides inside a cable or connector shell.

## 📂 Repository Layout

```
argus/
├── hardware/          # KiCad project, Gerbers, and board renders
│   ├── argus/         # Schematic, PCB layout, and fab-ready gerber/
│   └── screenshots/   # 3D views of the board
├── software/          # CH32V003 firmware
├── LICENSE
└── README.md
```

## License

Released under the [MIT License](LICENSE). Copyright (c) 2026 km1t4h.
