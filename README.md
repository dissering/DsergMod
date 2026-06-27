# DsergMod

![Minecraft](https://img.shields.io/badge/Minecraft-1.21.11-brightgreen) ![Loader](https://img.shields.io/badge/Fabric-Loader%20%E2%89%A50.19.3-blue) ![License](https://img.shields.io/badge/License-LGPL--3.0-orange)

DsergMod is a client-side Fabric mod for visual clarity and quality-of-life tweaks. It injects all behavior changes through **Mixins**, which means there is no server-side component.
It works out of the box on any compatible Fabric installation.

> **Supported version:** Minecraft **1.21.11** · **Fabric Loader ≥ 0.19.3** · **Java 25+** · requires **Fabric API**

## ⬇️ Download

Grab the latest `dsergmod-<version>.jar` from the [**Releases**](https://github.com/dissering/DsergMod/releases/latest) page and drop it in your `mods/` folder.

## ✨ Features

| Feature                         | Description                                                                                           |
|---------------------------------|-------------------------------------------------------------------------------------------------------|
| 🌟 **Fullbright**               | Scales in-game brightness via a configurable multiplier.                                              |
| 👁️ **Night vision cleanup**    | Suppresses the night vision effect.                                                                   |
| 🎃 **Pumpkin blur toggle**      | Disables the carved-pumpkin overlay blur.                                                             |
| 🔥 **Low fire**                 | Configurable first-person fire overlay offset.                                                        |
| 🛡️ **Low shield**              | Configurable first-person shield render offset.                                                       |
| 🗺️ **Boat map visibility**     | Keep filled maps visible while moving in boats.                                                       |
| 🌫️ **Fog controls**            | Toggle lava, powder snow, blindness, darkness, water, and atmospheric fog.                            |
| 📐 **Item scaling**             | Scale individual items (totems, potions, food, etc.) in first-person view via a dedicated sub-screen. |
| 🌊 **Riptide + shield fix**     | Corrects shield rendering position during riptide use.                                                |
| 🎮 **No-OP gamemode switcher**  | Enables the debug gamemode-switch screen without OP-level checks.                                     |
| 🕶️ **Vignette control**         | Toggle the dark vignette around screen corners.                                                       |
| 🔍 **Spyglass overlay toggle**  | Toggle the black spyglass overlay while keeping zoom.                                                 |
| ✈️ **Auto third person elytra** | Automatically switch to third person during Elytra flight.                                             |
| 📋 **Scoreboard visibility**    | Toggle display of the scoreboard sidebar.                                                            |
| 👥 **Entity shadows**           | Toggle entity shadows for an FPS boost.                                                               |
| 🌧️ **Weather rendering**        | Toggle rain and snow client-side for performance improvement.                                        |
| 🤕 **Hurt camera shake**        | Toggle camera tilt/shake effect when taking damage.                                                   |
| 💣 **TNT Explosion Timer**      | Displays a 3D countdown timer above primed TNT entities.                                              |
| 🛡️ **Durability Text Overlay**   | Displays precise colored durability text overlay on tools/armor in inventory and hotbar.               |

## ⚙️ Configuration

dsergmod settings are generated from config annotations and can be changed in-game.

| Method | Description |
| --- | --- |
| **ModMenu** *(preferred)* | Config entry inside ModMenu (if installed). |
| **Credits screen** *(fallback)* | Injected "dsergmod Settings" button in `CreditsAndAttributionScreen`. |
| **Config file** | `<gameDir>/config/dsergmod.json` — JSON, editable by hand. |

**Main options:**

`gammaMultiplier` · `nightVision` · `pumpkinBlur` · `fireOffset` · `shieldOffset` · `blindnessFog` · `darknessFog` · `lavaFog` · `powderSnowFog` · `waterFog` · `atmosphericFog` · `showMapWhileInBoat` · `fixShieldRiptideTrident` · `ignoreOpGamemodeSwitcher` · `vignette` · `spyglassOverlay` · `autoThirdPersonElytra` · `showScoreboard` · `viewmodelXOffset` · `viewmodelYOffset` · `viewmodelZOffset` · `viewmodelScale` · `entityShadows` · `showWeather` · `hurtTilt` · `tntTimer` · `armorDurabilityText`

**Item scaling** factors (totems, potions, food, shields, etc.) are configured in a separate sub-screen accessible from the main settings screen.

## 📦 Installation

1. Install **Fabric Loader** for **Minecraft 1.21.11**.
2. Place the dsergmod `.jar` into your Minecraft `mods/` folder.
3. Ensure **Fabric API** is installed.
4. Launch Minecraft with the Fabric profile.

## 🛠️ Building from source

This repository ships the compiled mod only. The full source is available upstream:

- Upstream source: [Codeberg → Bactrosaurus/dsergmod](https://codeberg.org/Bactrosaurus/dsergmod)

```bash
./gradlew build       # produces build/libs/dsergmod-<version>.jar
./gradlew runClient   # launches a dev Minecraft instance under run/
```

> **Java 25+ JDK required** on the build PATH (`options.release = 25` in `build.gradle.kts`).

## 📸 Screenshots

![](https://i.imgur.com/CIdyeb7.png)

![](https://i.imgur.com/07NFlrz.png)

---

<div align="center">

Licensed under **LGPL-3.0-only** · Source on [Codeberg](https://codeberg.org/Bactrosaurus/dsergmod)

</div>
