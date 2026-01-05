# Custom Embedded Operating System and GUI

This repository contains a custom embedded Operating System and GUI
developed from scratch during my work in video software R&D.
<br>
The system was designed to explore portable OS concepts under real
execution constraints rather than to serve as a general-purpose platform.

## System overview
The OS was initially implemented on AVR 8-bit MCUs and later ported across
multiple architectures:<br>
- AVR 8-bit<br>
- Toshiba 8-bit<br>
- Renesas R8C 16-bit<br>
- ARM9 32-bit<br>

Portability was achieved by isolating architecture-specific mechanisms
such as context switching, interrupt handling, and ABI boundaries,
allowing the core scheduling and system logic to remain largely unchanged.

## GUI subsystem
A lightweight GUI was implemented on the ARM9 platform with direct LCD
control. The focus was deterministic execution and minimal abstraction,
rather than feature richness.

## Design intent

This project emphasizes:<br>
- separation of policy and mechanism<br>
- explicit control over execution and memory<br>
- deterministic behavior under constrained environments<br>
- clarity at hardware–software boundaries<br>

The code reflects real-world constraints typical of deeply embedded systems
rather than modern convenience abstractions.

## Project status

Development paused due to a major personal life event, after which my
professional focus shifted toward applied systems engineering.<br>

The project is preserved here as an engineering artifact and learning
reference.<br>

Future work may include adapting the OS to boot directly on x86 hardware
from SPI flash, without reliance on external storage.<br>

#### Sourcecode

[OS src](https://github.com/sinfu98android/Custom-Embedded-OS-and-GUI/blob/main/PolOS.rar)  <br>
[GUI src](https://github.com/sinfu98android/Custom-Embedded-OS-and-GUI/blob/main/PolGUI.rar)

<br>
The archive format reflects the original development environment and
tooling used at the time.<br>

This repository is shared for educational and exploratory purposes.<br>
