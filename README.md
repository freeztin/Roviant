<p align="right"><a href="README.ru.md">РУССКИЙ</a> &nbsp; / &nbsp; <strong>ENGLISH</strong></p>

<img src=".github/assets/cover.svg" width="100%" alt="Roviant. Independent Linux launcher. Rust, GTK4 and libadwaita. Roblox on Linux. Arch Linux, CachyOS, Hyprland and Wayland.">

### A launcher for the Linux desktop.

Roviant is an independent project for launching Roblox on **Arch Linux** and **CachyOS**, written in **Rust** with **GTK4 / libadwaita**. Its focus is **Hyprland and Wayland**: the environment you already use, with a native desktop interface.

The launcher brings together system diagnostics, runtime state management and a defined connection to the game environment.

<br>

<img src=".github/assets/field-notes.svg" width="100%" alt="Three areas of development: diagnostics to inspect the system, runtime management to track states and launch, and integration to connect the game environment through a defined boundary.">

### Before the game starts.

Roviant is designed to show whether the system and runtime are ready, what is happening during launch, and where a failure occurred. Diagnostics and runtime states belong in the launcher, where you can see them.

<br>

<img src=".github/assets/architecture.svg" width="100%" alt="Proposed architecture: GTK4/libadwaita interface → Rust core → runtime → Roblox. System diagnostics feed the core; the runtime connects to the game environment through a defined integration boundary.">

### Under the hood.

The architecture separates the interface, system diagnostics, runtime lifecycle and game integration. The runtime connection has its own boundary, so the core can manage states without mixing launch logic into the interface.

This is the project’s design direction. Application source code and builds have not been published in this repository yet; installation instructions will follow a runnable release.

---

[Report an issue](https://github.com/freeztin/Roviant/issues) &nbsp; ↗ &nbsp; [Releases](https://github.com/freeztin/Roviant/releases) &nbsp; ↗ &nbsp; [По-русски](README.ru.md)

<sub>Roviant is an independent project, not affiliated with Roblox Corporation. Launch compatibility depends on the game runtime.</sub>
