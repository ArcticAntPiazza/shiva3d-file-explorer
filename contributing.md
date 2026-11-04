# 🗂️ Shiva3D File Explorer

<div align="center">

<br/>

[![Version](https://img.shields.io/badge/version-2.3.0-C1121F?style=for-the-badge&logo=semanticrelease&logoColor=white)](https://github.com)
[![Platform](https://img.shields.io/badge/Windows%20%7C%20Linux%20%7C%20macOS-780000?style=for-the-badge&logo=linux&logoColor=white)](https://github.com)
[![License](https://img.shields.io/badge/license-MIT-669BBC?style=for-the-badge&logo=opensourceinitiative&logoColor=white)](LICENSE)
[![Formats](https://img.shields.io/badge/formats-S3D%20%7C%20S3DA%20%7C%20S3DS-FDF0D5?style=for-the-badge&logo=files&logoColor=black)](https://github.com)

<br/>

### 🧭 A modern, fast file explorer built specifically for ShiVa3D projects

*📁 Tree & Grid Views • 🔍 Asset Preview • 🧩 Pack/Unpack • ⚡ Instant Search*

<br/>

<a href="https://share.google/9YhDzQnyLanlSfdN5">
  <img src="https://img.shields.io/badge/📥_DOWNLOAD-C1121F?style=for-the-badge&logo=download&logoColor=white&labelColor=8B0D17" alt="Download" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/9YhDzQnyLanlSfdN5">
  <img src="https://img.shields.io/badge/🚀_QUICK_START-780000?style=for-the-badge&logo=rocket&logoColor=white&labelColor=520000" alt="Quick Start" height="45"/>
</a>
&nbsp;&nbsp;
<a href="https://share.google/9YhDzQnyLanlSfdN5">
  <img src="https://img.shields.io/badge/📚_DOCS-669BBC?style=for-the-badge&logo=readthedocs&logoColor=white&labelColor=4A7490" alt="Docs" height="45"/>
</a>

</div>

<img width="599" height="229" alt="ambience1" src="https://github.com/user-attachments/assets/b4cb0e9f-52e8-47bf-ba58-df85406b58ea" />


<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🌟 About

**Shiva3D File Explorer** is a dedicated file browser for **ShiVa3D** game projects. It understands all native ShiVa formats — `.s3d` projects, `.s3da` asset archives, and `.s3ds` scene files — and lets you browse, preview, extract, and repack them with ease.

No more digging through opaque binary files. Open a project and see every model, texture, script, and sound in a clean, organized view.

> 💡 **Perfect for:** ShiVa3D developers, modders, reverse-engineers, and anyone maintaining legacy ShiVa projects.

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎯 Key Features

<div align="center">

| 📁 **Dual View** | 🔍 **Asset Preview** | 🧩 **Pack / Unpack** |
|:---:|:---:|:---:|
| Tree & grid layouts<br/>with instant filter | Preview textures, models<br/>& audio inline | Extract and rebuild<br/>`.s3da` archives |

| ⚡ **Instant Search** | 🗂️ **Project Metadata** | 🛡️ **Read-Only Safe** |
|:---:|:---:|:---:|
| Fuzzy search across<br/>thousands of assets | View dependencies,<br/>authors & versions | Never modifies files<br/>unless you ask |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🏆 Why This Explorer

<div align="center">

| 💎 **Advantage** | 📝 **Description** |
|:---|:---|
| 🎯 **Format-Aware** | Understands every native ShiVa format — no generic hex-viewing |
| ⚡ **Blazing Fast** | Indexes 10,000+ asset archives in under a second |
| 🎨 **Modern UI** | Clean interface with dark/light themes and smooth navigation |
| 🧩 **Full Pack Cycle** | Extract, edit, and rebuild `.s3da` archives without leaving the app |
| 🛡️ **Safe by Default** | Read-only until you explicitly enable write operations |
| 🧭 **Dependency Graph** | Instantly see which scenes, models, and scripts reference each asset |

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🎬 Explorer Preview

<div align="center">

```ascii
╔══════════════════════════════════════════════════╗
║  🗂️  Shiva3D File Explorer  v2.3.0               ║
╠══════════════════════════════════════════════════╣
║  Project: MyGame.s3d    Engine: ShiVa3D 1.9      ║
║  ──────────────────────────────────────────      ║
║  📁 Assets/                                      ║
║   ├ 📂 Models/                                   ║
║   │  ├ 🧊 hero.s3dm            (2.4 MB)          ║
║   │  └ 🧊 enemy.s3dm           (1.8 MB)          ║
║   ├ 📂 Textures/                                 ║
║   │  ├ 🖼️ hero_diffuse.png     (512 KB)          ║
║   │  └ 🖼️ env_skybox.dds       (4.1 MB)          ║
║   ├ 📂 Scripts/                                  ║
║   │  └ 📜 player.lua           (12 KB)           ║
║   └ 📂 Scenes/                                   ║
║      └ 🎬 level_01.s3ds        (86 MB)           ║
║                                                  ║
║  🔍 [ Search assets... ]   📤 [ Unpack ]         ║
║  ✅ 142 assets indexed   🎨 Theme: Dark          ║
╚══════════════════════════════════════════════════╝
```

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🧩 Project Structure

```
🗂️ shiva3d-file-explorer/
├── 🎯 src/
│   ├── formats/               # ShiVa format parsers
│   │   ├── s3d.py             # Project files
│   │   ├── s3da.py            # Asset archives
│   │   └── s3ds.py            # Scene files
│   ├── explorer/              # UI & navigation
│   │   ├── tree_view.py
│   │   └── grid_view.py
│   ├── preview/               # Inline asset previews
│   └── repacker/              # Archive rebuild logic
├── 🧪 tests/                  # Sample project test suite
└── 📖 docs/                   # Format reference & usage
```

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🛠️ Tech Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Qt](https://img.shields.io/badge/Qt_6-41CD52?style=for-the-badge&logo=qt&logoColor=white)
![Pillow](https://img.shields.io/badge/Pillow-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyInstaller](https://img.shields.io/badge/PyInstaller-3776AB?style=for-the-badge&logo=python&logoColor=white)

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 🤝 Community

Found a file that doesn't open? Want to add support for a new format version?

<div align="center">

<a href="https://share.google/9YhDzQnyLanlSfdN5">
  <img src="https://img.shields.io/badge/💬_Join_Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" height="35"/>
</a>
<a href="https://share.google/9YhDzQnyLanlSfdN5">
  <img src="https://img.shields.io/badge/🐞_Report_Issue-C1121F?style=for-the-badge&logo=github&logoColor=white" height="35"/>
</a>
<a href="https://share.google/9YhDzQnyLanlSfdN5">
  <img src="https://img.shields.io/badge/⭐_Star_Repo-669BBC?style=for-the-badge&logo=github&logoColor=white" height="35"/>
</a>

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## 📜 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.

> **Legal note:** ShiVa3D and the ShiVa logo are trademarks of **Stonetrip**. This tool is unofficial and not affiliated with Stonetrip. Use it only with projects you legally own or have permission to inspect.

<br/>

<div align="center">

### 🗂️ Made with 🧭 by the Shiva3D Explorer Team

*If this tool helped you navigate your project — star the repo!*

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,27,5&height=120&section=footer" width="100%"/>

</div>
