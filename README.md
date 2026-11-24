<p align="center">
  <img src="program_info/org.prismlauncher.PrismLauncher.logo.svg" alt="Prism Launcher Logo" width="128"/>
</p>

<h1 align="center">Prism Launcher</h1>

<p align="center">
  A custom launcher for Minecraft that allows you to easily manage multiple installations of Minecraft at once.<br/>
  <sub>Community build with standalone local profile support • <a href="https://github.com">skretchati</a></sub>
</p>

<p align="center">
  <a href="https://github.com/PrismLauncher/releases/latest">
    <img src="https://shields.io" alt="Download Latest Release"/>
  </a>
  <a href="https://github.com/PrismLauncher/blob/develop/LICENSE">
    <img src="https://shields.io" alt="License"/>
  </a>
</p>

---

## About

Prism Launcher is a free, open-source launcher for Minecraft (forked from PolyMC). It allows you to have multiple, cleanly separated instances of Minecraft (each with their own mods, resource packs, saves, etc.) and helps you manage them and their associated options with a simple and powerful interface.

### Build Notes
* Standalone Local Profiles: This build enables creating and launching local (offline) player profiles directly without requiring an external Microsoft account entitlement check. Designed for local testing, LAN sessions, and private servers with custom authentication.
* Pre-built Binaries: Ready-to-use Windows (x64 MSVC) installer and portable builds are available on the [Releases](https://github.com/PrismLauncher/releases/latest) page.
* Updates: Please skip built-in update prompts if they appear, as upstream updates will replace this binary with the standard upstream release.

---

## Features

* Isolated Instances: Keep different Minecraft versions, modloaders, configurations, and worlds completely separate.
* Integrated Mod & Modpack Browser: Search, download, and update mods, modpacks, resource packs, and shader packs directly from Modrinth and CurseForge.
* Modloader Support: Built-in installation for Fabric, Forge, NeoForge, Quilt, and LiteLoader.
* Java Management: Automatic detection of local Java installations with per-instance memory and JVM argument settings.
* Customization: Support for custom themes, icon packs, and background cats.

---

## Installation (Windows)

1. Open the [Latest Release](https://github.com/PrismLauncher/releases/latest) page.
2. Download either:
   * **Setup.exe** — standard Windows installer.
   * **Portable.zip** — portable archive (extract with 7-Zip or WinRAR).
3. First Run: Because this build is not signed with a commercial code-signing certificate, Windows SmartScreen may display an *"Unrecognized app"* warning on first launch. Click More info → Run anyway to continue.

---

## Building

For general compilation steps and dependencies (CMake, Qt 6, JDK 17+), refer to the [Build Instructions](https://prismlauncher.org).

git clone --recursive https://github.com/PrismLauncher.git
cd PrismLauncher
cmake -B build -DCMAKE_BUILD_TYPE=Release
cmake --build build --config Release
---

## License

This project is licensed under the GNU General Public License v3.0 — see the [LICENSE](LICENSE) file for details.

*Minecraft is a trademark of Mojang Synergies AB. This project is not affiliated with or endorsed by Mojang or Microsoft.*
