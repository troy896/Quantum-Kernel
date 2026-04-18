# Quantum-Kernel

<p align="center">
  <img src="https://img.shields.io/badge/Base-Sultan-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Wild%20KSU-Built--In-6f42c1?style=for-the-badge" />
  <img src="https://img.shields.io/badge/SUSFS-v2.0.0-1f883d?style=for-the-badge" />
  <img src="https://img.shields.io/badge/SELinux-Enforcing-success?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Android-16-3ddc84?style=for-the-badge" />
</p>

<p align="center">
  <b>Quantum-Kernel</b> is a <b>Sultan-based kernel</b> for <b>Pixel Tensor devices</b>, focused on stability, clean integration, and practical daily use.
</p>

---

## Overview

Quantum-Kernel keeps the strong Sultan kernel base while adding project-specific integration work, packaging, release automation, and optional support for **Wild KSU** and **SUSFS**.

This project is meant to stay clean, usable, and reliable.

It is not designed to be a random collection of questionable tweaks. The goal is to provide a solid **Sultan-based kernel** with a proper **stock** option and a modern **root-ready** option for users who want **Wild KSU** and **SUSFS**.

---

## Variants

### `stock`
Pure Quantum-Kernel base build with no Wild KSU or SUSFS integration.

### `wksu-susfs`
Quantum-Kernel with:
- **Wild KSU** built in
- **SUSFS v2.0.0**
- **Inline hook mode**
- Project-specific integration and config changes

---

## Current Validation

Current public validation includes:

- **Android 16 stock**
- **SELinux Enforcing**
- **Wild KSU built-in working**
- **SUSFS inline mode working**
- Successful boot confirmation on tested device(s)

---

## Build Targets

The current workflow produces builds for:

- `gs201`
- `zuma`
- `zumapro`

Runtime testing may vary depending on device, firmware version, and setup.

---

## Downloads

### Releases
- [Latest Release](https://github.com/Drizzy07x/Quantum-Kernel/releases/latest)
- [All Releases](https://github.com/Drizzy07x/Quantum-Kernel/releases)

### Source
- [Quantum-Kernel Repository](https://github.com/Drizzy07x/Quantum-Kernel)

---

## Installation

Flash the correct **AnyKernel3** package for your device and chosen variant.

### Example artifact names
- `kernel-gs201-stock`
- `kernel-gs201-wksu-susfs`
- `kernel-zuma-stock`
- `kernel-zuma-wksu-susfs`
- `kernel-zumapro-stock`
- `kernel-zumapro-wksu-susfs`

---

## Notes

- Always flash the correct build for your device codename
- Keep a known working boot image or recovery path before testing a new kernel
- The `wksu-susfs` variant is intended for users who specifically want **Wild KSU + SUSFS**
- First public validation has been done on **Android 16 stock**

---

## Credits

Quantum-Kernel would not exist without the work of the people and projects below.

- **[Sultan / kerneltoast](https://github.com/kerneltoast/android_kernel_google_tensynos)** — for the Sultan kernel base used by this project
- **[WildKernels](https://github.com/WildKernels/Wild_KSU)** — for **Wild KSU**
- **[simonpunk](https://gitlab.com/simonpunk/susfs4ksu)** — for **SUSFS / susfs4ksu**
- **[sidex15](https://github.com/sidex15/ksu_module_susfs)** — for the **ksu_module_susfs** ecosystem
- **[TheWildJames](https://github.com/TheWildJames)** — for packaging and workflow resources used in this project, including **AnyKernel3** branches and related patch resources
- Everyone contributing to the wider **KernelSU**, **SUSFS**, **Pixel kernel**, and Android kernel modding community

---

## Disclaimer

You are responsible for what you flash.

Always make sure you are using the correct build for your device and keep a recovery path available in case something goes wrong.
