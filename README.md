# Rainmeter Setup Guide

> Empower your workspace with dynamic, lightweight skins and seamless customization.

## Table of Contents

1. [Introduction](#introduction)
2. [Download Rainmeter](#download-rainmeter)
3. [Installation](#installation)
4. [Folder Structure & Default Paths](#folder-structure--default-paths)
5. [Basic Usage](#basic-usage)
6. [Skin Management Tips](#skin-management-tips)
7. [Advanced Configuration](#advanced-configuration)
8. [Troubleshooting & Logs](#troubleshooting--logs)
9. [Additional Resources](#additional-resources)
10. [License](#license)

---

## 1. Introduction

Rainmeter is an open-source platform that empowers you to transform your Windows desktop into a robust, fully customizable dashboard. Whether you want real‑time system stats, weather reports, or slick media controls, Rainmeter synergizes performance and aesthetics in one modular package.

## 2. Download Rainmeter

Download the latest stable release from the official site:

* **URL:** [https://www.rainmeter.net/](https://www.rainmeter.net/)
* **Installer (64-bit):** [https://download.rainmeter.net/Rainmeter-4.5.15-64bit.exe](https://download.rainmeter.net/Rainmeter-4.5.15-64bit.exe)
* **Portable ZIP (optional):** [https://download.rainmeter.net/Rainmeter-4.5.15-Portable.zip](https://download.rainmeter.net/Rainmeter-4.5.15-Portable.zip)

> *Pro Tip:* Always grab your release from the official domain to stay secure and up-to-date.

## 3. Installation

1. Run the `.exe` installer or extract the portable ZIP.
2. Follow the wizard: accept the EULA, choose install type (Standard vs. Portable), and select your target folder.
3. Launch Rainmeter via Start Menu or `Rainmeter.exe` in the install root.

## 4. Folder Structure & Default Paths

Streamline your workflow by understanding where Rainmeter keeps its assets and configs.

### A. Installation Directory (Program Files Mode)

```
C:\Program Files\Rainmeter\
├─ Rainmeter.exe
├─ Rainmeter.dll
├─ Skins\        # Default bundled skins
└─ Plugins\      # Core plugins (.dll)
```

### B. Portable Mode

```
D:\PortableApps\Rainmeter\    # Mirrors the standard install tree
```

### C. User Configuration & Skins (Documents)

```
C:\Users\<YourUser>\Documents\Rainmeter\
├─ Skins\        # Your custom skins
│  └─ MySkin\     # Example: MySkin.ini + resources
├─ Layouts\      # Saved layouts (.rmskinlayout)
├─ AutoLoad\     # Skins to auto-start on login (.rmskin)
└─ Rainmeter.ini  # Personal global settings
```

### D. Roaming Config & Cache (AppData)

```
C:\Users\<YourUser>\AppData\Roaming\Rainmeter\
├─ Rainmeter.ini  # Global settings
├─ Cache\        # Measurement caches
└─ Logs\         # rainmeter.log for debug
```

## 5. Basic Usage

* **Manage Skins:** Right-click the tray icon → Manage.
* **Load/Unload:** Browse your `Documents\Rainmeter\Skins` tree and toggle skins.
* **Position & Snap:** Drag skins anywhere; use `Ctrl` + Drag to snap to grid.
* **Save Layout:** Click `Layouts` → `Save` to capture current setup.

## 6. Skin Management Tips

* Use `@Resources` variables to standardize paths.
* Bundle assets (images, fonts) in a dedicated `@Resources` folder.
* Leverage Git for version control under `Documents\Rainmeter\Skins`.
* Modularize skins with include files (`.inc`).

## 7. Advanced Configuration

* **Global Tweaks:** Edit `AppData\Roaming\Rainmeter\Rainmeter.ini` for startup parameters.
* **Custom Plugins:** Drop `.dll` files into `Plugins\` under Program Files or portable root.
* **AutoStart:** Add skins to `AutoLoad` for auto-launch on Windows login.

## 8. Troubleshooting & Logs

* **Log File:** `%AppData%\Rainmeter\Logs\rainmeter.log` captures errors and warnings.
* **Configuration Reload:** Right-click tray icon → `Refresh All` to apply changes instantly.
* **Safe Mode:** Launch `Rainmeter.exe /SafeMode` to disable third-party plugins.

## 9. Additional Resources

* **Official Docs:** [https://docs.rainmeter.net/](https://docs.rainmeter.net/)
* **Community Forum:** [https://forum.rainmeter.net/](https://forum.rainmeter.net/)
* **DeviantArt Skins:** [https://www.deviantart.com/rainmeter](https://www.deviantart.com/rainmeter)
* **GitHub Repo:** [https://github.com/rainmeter/rainmeter](https://github.com/rainmeter/rainmeter)

## 10. License

Rainmeter is licensed under [GPLv2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html).
