# BoardRunner

**Building the foundations for scalable firmware rehosting and cyber-physical systems simulation.**

Embedded firmware depends on more than a processor. It interacts with peripherals, sensors, actuators, and the physical environment. Running that firmware outside its original board requires reproducing those interactions.

BoardRunner brings together research and tools for connecting firmware execution, peripheral models, virtual I/O, and real hardware. Our goal is to make embedded systems easier to run, inspect, test, and analyze.

## Research direction

We focus on three connected challenges:

- **Firmware rehosting:** Run embedded firmware outside its original hardware while preserving the peripheral interactions it relies on.
- **Efficient simulation:** Accelerate execution and connect firmware to models of its environment.
- **Reusable infrastructure:** Share interfaces and components across emulators, device models, and hardware experiments.

These capabilities support firmware testing, vulnerability discovery, and the study of cyber-physical behavior.

## Projects

| Project | Purpose |
| --- | --- |
| [BoardRunner](https://github.com/boardrunner2049/BoardRunner) | Firmware rehosting system. Public implementation not yet available. |
| [FastDyn](https://github.com/boardrunner2049/FastDyn) | Execution engine for the BoardRunner ecosystem. Public implementation not yet available. |
| [LibVIO](https://github.com/boardrunner2049/LibVIO) | Standalone C library connecting emulated peripherals to virtual I/O, including terminals, files, networking, signals, DMA, ADC, and SPI/I2C buses with pluggable devices. |
| [libhw](https://github.com/boardrunner2049/libhw) | Hardware access library providing a common interface for memory operations and flash programming through ST-Link, OpenOCD, and a mock backend, with Python bindings. |
| [QEMU](https://github.com/boardrunner2049/qemu) | The organization’s QEMU fork. |

## Getting started

The supporting libraries can be used independently:

- **Building device models?** Start with [LibVIO](https://github.com/boardrunner2049/LibVIO) and its [API guide](https://github.com/boardrunner2049/LibVIO/blob/main/docs/API.md). It builds without FastDyn or QEMU.
- **Working with physical boards?** Start with [libhw](https://github.com/boardrunner2049/libhw) for hardware access, flash programming, and Python integration.

See each repository for build instructions, dependencies, documentation, and licensing.

## Community

We welcome researchers and developers working on firmware rehosting, emulation, embedded systems, and CPS security.

**[Join our Discord community](https://discord.gg/wYFbUQT5y)** to ask questions, discuss ideas, share use cases, and connect with the project.

For reproducible bugs and concrete feature requests, open an issue in the relevant repository where issue tracking is enabled.
