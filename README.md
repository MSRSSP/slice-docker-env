# Core slicing prototype
This tutorial will walk you through building and executing two versions of our core slicing prototype: one with desired security properties in RISC-V, and another for performance evaluation in x86.

## RISC-V prototype

### :rocket: Quick start

Jump to :point_right: [quick-start](quick-start.md) if you do not want to compile from source code.

### :hourglass: :wrench: Build from source
Follow :point_right: [build tutorial](build.md) to build from source code.

### :-1: Limitations
There are some limitations of using QEMU-based emulation, such as: 
* :alarm_clock: Timestamp from log is not useful since it is under QEMU.
* :construction: Slice cache will always show zero value for cache controller registers since the cache emulation is unimplemented.
* :tv: UART-0 is assigned to slice-0, UART-1 is reserved for normal harts to use before they are locked into a slice, UART-2 is used by hart1 and hart2, UART2 is used by hart 3 and hart4.

## Core slicing x86 prototype

Jump to :point_right: [slice-x86](https://github.com/MSRSSP/sliceloader-x64#readme) for x86 tutorials. You need a machine with SR-IO support NIC.

Jump to :point_right: [slice-x86-exp](x86-exp/README.md)
