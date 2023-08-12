# Start and Shutdown Procedures

## Introduction
- **Boot** and **Shutdown** procedures: Sequences guiding a computer from power-on to off.
- Needed during system power cycles, maintenance, or software updates.

## System Start

### 1. What's a Bootloader?
- Small program in system's firmware or primary storage.
- Purpose: Load the operating system into main memory.

### 2. Booting Process

#### MBR (Master Boot Record) Booting
1. **BIOS** initializes hardware.
2. Control handed to the **MBR** on the boot device.
3. MBR loads the **primary bootloader** (e.g., GRUB).

#### UEFI (Unified Extensible Firmware Interface) Booting
1. **UEFI firmware** initializes hardware.
2. Firmware reads boot entries, loads specified **EFI application**.
3. Bootloader (e.g., GRUB) is loaded from **EFI system partition**.

### 3. Kernel Loading
- Bootloader loads the **OS kernel**.
- In Linux: often `vmlinuz`.
- Kernel initializes hardware, mounts filesystem, starts `init` process.

### 4. Boot Flags
- Flags/parameters passed to the kernel at boot.
- Can include device configurations, disabling features, etc.

### 5. Init Messages and Procedures
- `init` starts post-kernel load.
- Messages during boot: `init` starting services, checking system states.

## System Shutdown

### 1. Importance
- Proper shutdown: Save data, finish processes, stabilize peripherals.

### 2. Pre-shutdown Checks
- Check for running critical tasks.
- Ensure no active data writes.
- Ensure no active users.

### 3. Killing Processes and User Sessions
- Signal processes to terminate orderly.
- Terminate user sessions, logging out users.

### 4. Commands
- **Shutdown** (Linux): `shutdown -h now`
- **Reboot** (Linux): `shutdown -r now` or `reboot`
- **Forcefully Kill Processes**: Use `kill` or `pkill`.
- **Logout Users**: Use `logout`.

## Conclusion
- Starting & shutting down ensures a correct operating environment.
- Procedures vary slightly based on the OS.
