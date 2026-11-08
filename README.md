<p align="center">🌻🧟</p>

<h1 align="center">Plants vs. Zombies Fusion | Multi-Language Translation</h1>

<p align="center">The community multi-language translation for <b>Plants vs. Zombies: Fusion</b> | translation files, translated textures, the Translator mod, and the official PC and Android download links, all in one place.</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-PC%20%C2%B7%20Android-558B2F" alt="Platform: PC · Android">
  <a href="https://github.com/c12n/PVZF-Translation/releases/latest"><img src="https://img.shields.io/github/v/release/c12n/PVZF-Translation?label=Latest%20release&color=33691E" alt="Latest release"></a>
  <a href="https://github.com/c12n/PVZF-Translation/releases"><img src="https://img.shields.io/github/downloads/c12n/PVZF-Translation/total?label=Downloads&color=33691E" alt="Downloads"></a>
  <img src="https://img.shields.io/badge/License-CC%20BY--NC%204.0-33691E" alt="License: CC BY-NC 4.0">
</p>

<p align="center">
  📥 <a href="https://github.com/c12n/PVZF-Translation/releases/latest"><b>Download the latest release</b></a> · 🔗 <a href="https://github.com/Teyliu/PVZF-Translation"><b>Upstream repo</b></a> · 🐛 <a href="https://github.com/Teyliu/PVZF-Translation/issues"><b>Report an issue</b></a>
</p>

`4.0.5.2 Alpha` · Multi-Language build for PC | base game 4.0.5, translation support for base game 3.9 and earlier.

> [!NOTE]
> **Unofficial fan project.** This is a fork of [Teyliu/PVZF-Translation](https://github.com/Teyliu/PVZF-Translation) for layout and reference. It is not affiliated with or endorsed by EA, PopCap, or the original Fusion team (LanPiaoPiaoFly / Blue Fly). All translation credit belongs to the upstream contributors listed under Credits.

---

## 🌟 Features

| **Multi-language game text**<br>Almanac and in-game string translations for English, Chinese (Simplified), Indonesian, French, Spanish, Vietnamese, Japanese, Ukrainian, Romanian and Korean. Some languages are complete to older base versions and update gradually. | **Translator mod included**<br>`PvZ_Fusion_Translator.dll` plus `AudioImportLib.dll` and `Blooms_QOL.dll` at the repo root, ready to drop into a MelonLoader install. The mod reads the JSON translation files in this repo. |
| :--- | :--- |
| **Translated textures**<br>Translated menu, almanac, seed packet and selector textures under `PvZ_Fusion_Translator/`, including the default texture set that ships with the mod. | **Plant and zombie IDs**<br>`PlantsAndZombiesIDs/` holds the plant and zombie ID lists used by translators, level makers and the almanac. |
| **Translator scripts**<br>Four Python helpers in `Useful Scripts`: convert between JSON, CSV and XLSX, and compare almanac or string files between languages. See How to Use below. | **Online English Almanac**<br>A web almanac by CarrotD1scrd, linked in the upstream README. It updates slowly, so the in-game text in this repo is the current source. |

---

## 🚀 Installation

### PC | Pre-patched (recommended)

1. Download `PvZ.Fusion.Multi-lang.4.0.5.2.Alpha.by.Blooms.zip` from the [latest release](https://github.com/c12n/PVZF-Translation/releases/latest) into a **new folder**. Do not install over an older version.
2. Extract it to a path with no special or non-ASCII characters, and not inside Downloads, Documents, Desktop, OneDrive or MEGA folders.
3. Run the game through `Launch Game.bat` or `PlantsVsZombiesRH.exe`.
4. If the game closes instantly, install the .NET 6.0 Desktop Runtime and everything in the Redist download linked in the upstream README, then try again.

### PC | Manual MelonLoader install (optional)

1. Get the base game from the original developers (Bilibili link in the upstream README).
2. Install MelonLoader 0.7.1 and patch the game via Add Game Manually, selecting `PlantsVsZombiesRH.exe`.
3. Download the source code ZIP of this repo and extract it into the `Mods` folder in your game folder.

### Android

1. Download an Android release APK from the [Releases page](https://github.com/Teyliu/PVZF-Translation/releases) (English Android builds are listed there, for example 3.6.1 and 3.5).
2. Install the APK over your previous installation. **Do not delete your previous installation first, or you will lose your progress.**

### iOS

> [!IMPORTANT]
> **There is no native iOS version, and no IPA can be built from this repo.** This repo contains translation JSON files, textures and compiled Windows mod DLLs for MelonLoader. It contains no Unity project and no Xcode project, and the original Fusion team ships the game for PC and Android only. Sites advertising a "PvZ Fusion IPA download" are not offering a real build from this project. A real iOS build would need the original Unity project from the Fusion team, built with the Unity iOS target.

---

## 📖 How to Use

**Playing:** install as above, pick your language in game, and your saves carry over when you update the PC build (delete the old PC install folder first, into a new folder each time).

**Translating:** all four scripts in `Useful Scripts` read files from the folder the script is in.

1. `csver.py` converts `*.json` translation files to `*.csv` for spreadsheet editing.
2. `jsonifier.py` converts a finished `*.xlsx` spreadsheet back into the `*.json` files the mod reads. Copy them to `Mods/PvZ_Fusion_Translator/Localization/<Language>/Almanac` or `Strings` in your game folder.
3. `almanac_json_comparer.py` and `strings_json_comparer.py` compare your language against English, keeping your entries and appending untranslated English entries at the bottom.

---

## 🗺️ Roadmap

This fork tracks upstream. Upstream status from the latest release notes:

- Gods: Evolved almanac, Super Level Editor guide and Custom Online Levels translation support are **not** currently planned upstream.
- Language coverage varies by base version: English and Korean are the most current, other languages update gradually through the online system.

---

## ⚠️ Known Issues

- **iOS:** not available, in any form, from this project. See the iOS note under Installation.
- **Mods:** the Multi-Language PC build is MelonLoader only and is **not** compatible with mods that require the BepInEx ecosystem.
- **Paths:** the PC build fails or closes on paths containing special characters, or when extracted into user folders such as Downloads or Desktop.

---

## ❓ FAQ

**Is it free?**
Yes | free, no ads, no in-app purchases, non-commercial under CC BY-NC 4.0.

**Is this the game itself?**
The Releases on this repo bundle the pre-patched PC game with the translation for convenience. This repo itself is the translation files and mod artifacts, not the game source code.

**Where is the Translator mod source code?**
The upstream README notes the mod source is in a separate repo, and asks developers to reach out by email or Discord if they need it. You do not need to build from source to play.

**Can I play it on iPhone or iPad?**
No. There is no native iOS build and none has been announced by the Fusion team. See the iOS note under Installation.

**Where do I get help with install errors?**
The upstream Discord server linked in the upstream README, in its FAQ | Errors channel.

---

## 🔒 Privacy

This repo is translation files, textures and mod DLLs. It adds no accounts and no analytics of its own. The fork changes presentation only.

---

## 🏗️ Built With

- **Game:** Unity, by LanPiaoPiaoFly / Blue Fly and team (PC and Android only)
- **Mod loader:** MelonLoader 0.7.1, .NET 6.0
- **This repo:** JSON localization files, PNG textures, compiled mod DLLs, Python helper scripts

## 🛠️ Build It Yourself

There is nothing to compile here to play the game. Download a Release above instead.

If you are a translator or developer:

```sh
git clone https://github.com/c12n/PVZF-Translation.git
cd PVZF-Translation
# Translation files: PvZ_Fusion_Translator/
# Helper scripts: "Useful Scripts" (Python 3, run in place)
# Mod DLLs: repo root (PvZ_Fusion_Translator.dll and friends)
```

### GitHub Actions

| Workflow | Runs when | What it does |
| --- | --- | --- |
| **Keyword moderator** | On issues and comments | Upstream moderation workflow, the only workflow in this repo. There is no build workflow, because there is no app or game project here to build. |

<details>
<summary><b>Project layout</b></summary>

- `PvZ_Fusion_Translator/` | translation JSON files, dumps and textures, by language
- `PlantsAndZombiesIDs/` | `plantID.json` and `zombieID.json`
- `Useful Scripts/` | the four Python converter and comparer scripts
- `ConsolManager/` | console manager notes
- `Docs/` | contributor documentation, including the French team reports
- Repo root DLLs | `PvZ_Fusion_Translator.dll`, `AudioImportLib.dll`, `Blooms_QOL.dll`
- `CURRENT_GAME_VER` | the base game version the translations currently target

</details>

---

## Credits

| **LanPiaoPiaoFly's Team** | Original Developers |
| --- | --- |
| Program, Director | LanPiaoPiaoFly (Blue Fly) |
| Animation | LanPiaoPiaoFly, JiYu |
| Artist, Visual Director | LanPiaoPiaoFly |
| Video Editor | LanPiaoPiaoFly, MengLuo |
| Animation Helper | JiYu, LanDie |
| Art Helper | LanDie |

### Translation Credits

| Person / People | Contribution |
| --- | --- |
| **Mamoru-kun** | Main Translator |
| **NaKune** | OG Translation Mod Creator |
| **Climeron** | Coding Help |
| **Teyliu, Cassidy, JustNull, Dakosha** | Coding |
| **TrevTV** | Audio Changing Implementation |
| **Rollerlhite** | New Main Menu Music |
| **Cassidy** | English PvZ Fusion Logo |
| **Roaoming, Shel** | Custom Textures |
| **flexyj, CarrotD1scord** | Translation Textures |
| **Xabdi** | Translation Textures, New In-Game Music |
| **The Blooms Community** | Translation ideas and assistance |

Full language team lists are in the [upstream README](https://github.com/Teyliu/PVZF-Translation#language-teams).

---

## Disclaimer

This is an unofficial fan translation project and is not affiliated with, authorized, or endorsed by EA, PopCap, or the original Plants vs. Zombies: Fusion team. Provided "as is", without warranty of any kind.

- This project is **free** and non-commercial. If a third party charged you for it, you may have been misled.
- No user data is collected by this repository.

## 📄 License

Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0) | the upstream project's license. See [LICENSE](LICENSE). Commercial use is not permitted.

> [!TIP]
> **Star the upstream repo** ([Teyliu/PVZF-Translation](https://github.com/Teyliu/PVZF-Translation)) to support the translators and get notified about new releases directly from GitHub.
