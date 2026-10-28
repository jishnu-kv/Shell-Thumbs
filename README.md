# ShellThumbs

<p align="center">
  <strong>High-Performance Windows Shell Extension Suite for File Explorer Thumbnails & Interactive Previews</strong>
</p>

<p align="center">
  <a href="https://github.com/jishnu-kv/Shell-Thumbs/issues"><img src="https://img.shields.io/badge/Issues-Report%20a%20Bug-blue.svg" alt="Issues"></a>
  <a href="https://github.com/jishnu-kv/Shell-Thumbs/issues/new?template=format_request.md"><img src="https://img.shields.io/badge/Format%20Request-Suggest%20Format-green.svg" alt="Format Request"></a>
  <img src="https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-0078D6.svg" alt="Platform">
  <img src="https://img.shields.io/badge/Architecture-x64-brightgreen.svg" alt="Arch">
</p>

---

## 📌 Public Issue Tracker & Community Hub

> **Note**: This repository serves as the **official public issue tracker, format request hub, and community forum** for ShellThumbs. The application source code is maintained in a private repository.

* 🐛 **Found a bug or rendering issue?** &rarr; [Submit a Bug Report](https://github.com/jishnu-kv/Shell-Thumbs/issues/new?template=bug_report.md)
* 💡 **Need support for a new 2D, 3D, CAD, or graphic format?** &rarr; [Submit a Format Request](https://github.com/jishnu-kv/Shell-Thumbs/issues/new?template=format_request.md)
* 💬 **Questions & Feedback** &rarr; [Browse Open Issues](https://github.com/jishnu-kv/Shell-Thumbs/issues)

---

## 🚀 Overview

**ShellThumbs** is a zero-dependency, ultra-fast Windows Shell Extension suite and modern WinUI 3 management utility providing native Windows File Explorer **Thumbnail Providers** (`IThumbnailProvider`) and **Preview Handlers** (`IPreviewHandler`) for complex 2D, 3D, CAD, vector, font, and code formats.

### Key Highlights
* **Sub-Millisecond Thumbnail Generation**: Instant rendering directly inside Windows File Explorer folders.
* **Hardware-Accelerated 3D & Vector Rendering**: Direct3D 11 and Direct2D pipelines for smooth, high-fidelity rendering.
* **Isolated Process Security**: Preview handlers execute safely inside Windows' isolated surrogate process (`prevhost.exe`).
* **Modern Windows 11 Fluent UI App**: Easy-to-use management app with Mica material, instant search, and one-click format configuration.

---

## 📁 Supported Formats

ShellThumbs supports **41+ primary formats** and **539 programming language code extensions**:

### 1. 3D Models & CAD Files
| Format | Extension | Thumbnail | Preview | Description |
|---|---|:---:|:---:|---|
| **STEP 3D CAD** | `.step`, `.stp` | ✅ | ✅ | Standard for the Exchange of Product model data (ASCII wireframe & ISO projection) |
| **IGES 3D CAD** | `.iges`, `.igs` | ✅ | ✅ | Initial Graphics Exchange Specification CAD wireframe |
| **Wavefront 3D** | `.obj` | ✅ | ✅ | Standard 3D geometry with material and texture support |
| **Autodesk FBX** | `.fbx` | ✅ | ✅ | Binary FBX tokenized 3D mesh and scene parser |
| **glTF 2.0 Binary** | `.glb` | ✅ | ✅ | Khronos Group binary 3D container |
| **glTF 2.0 Scene** | `.gltf` | ✅ | ✅ | Khronos Group JSON & binary buffer mesh format |
| **Stereolithography** | `.stl` | ✅ | ✅ | 3D printing binary & ASCII triangle meshes |
| **Stanford Triangle** | `.ply` | ✅ | ✅ | 3D scanning and polygonal mesh format |
| **COLLADA 3D** | `.dae` | ✅ | ✅ | Digital Asset Exchange XML geometry |
| **Rhino 3D** | `.3dm` | ✅ | ✅ | Robert McNeel & Associates Rhino 3D model |
| **Autodesk 3DS** | `.3ds` | ✅ | ✅ | Legacy 3D Studio mesh chunk format |
| **SketchUp** | `.skp` | ✅ | ✅ | Trimble SketchUp 3D scene model |
| **Autodesk 3ds Max** | `.max` | ✅ | ✅ | OLE container embedded scene stream preview |
| **3D Manufacturing** | `.3mf` | ✅ | ✅ | Modern 3D printing container format |
| **Blender Project** | `.blend` | ✅ | ✅ | Blender 3D scene embedded thumbnail extractor |
| **Universal Scene Description** | `.usd`, `.usdz` | ✅ | ✅ | Pixar USD / USDC crate delta-tokenized mesh format |

### 2. Design, Vector & Publishing
| Format | Extension | Thumbnail | Preview | Description |
|---|---|:---:|:---:|---|
| **Scalable Vector Graphics** | `.svg` | ✅ | ✅ | Native Direct2D vector graphics engine |
| **Adobe Photoshop** | `.psd`, `.psb` | ✅ | ✅ | Photoshop document RLE & raw channel decoder |
| **Adobe Illustrator** | `.ai` | ✅ | ✅ | Illustrator vector & embedded PDF stream renderer |
| **Encapsulated PostScript** | `.eps` | ✅ | ✅ | PostScript vector & TIFF preview decoder |
| **Adobe InDesign** | `.indd`, `.idml` | ✅ | ✅ | Shuksan database defragmenter & IDML XMP extractor |
| **CorelDRAW** | `.cdr` | ✅ | ✅ | CorelDRAW ZIP container vector preview |

### 3. Engineering & CNC Toolpath
| Format | Extension | Thumbnail | Preview | Description |
|---|---|:---:|:---:|---|
| **AutoCAD Drawing** | `.dwg` | ✅ | ✅ | AutoCAD sentinel header & WIC PNG/BMP decoder |
| **AutoCAD Exchange** | `.dxf` | ✅ | ✅ | ASCII DXF entity parser & Direct2D vector geometry |
| **Delcam ArtCAM** | `.art`, `.rlf` | ✅ | ✅ | ArtCAM 3D reliefs and machining models |
| **CNC & 3D G-code** | `.gcode`, `.bgcode`, `.nc`, `.tap`, `.gco`, `.ngc` | ✅ | ✅ | Slicer embedded previews & 3D toolpath trajectories |

### 4. Camera RAW Photography
| Format | Extension | Thumbnail | Preview | Description |
|---|---|:---:|:---:|---|
| **Canon RAW** | `.cr2`, `.cr3` | ✅ | ✅ | Canon Digital Camera RAW |
| **Nikon RAW** | `.nef` | ✅ | ✅ | Nikon Electronic Format RAW |
| **Sony Alpha RAW** | `.arw` | ✅ | ✅ | Sony Alpha Camera RAW |
| **Adobe Digital Negative** | `.dng` | ✅ | ✅ | Open standard camera RAW |
| **Olympus RAW** | `.orf` | ✅ | ✅ | Olympus Camera RAW |
| **Panasonic Lumix RAW** | `.rw2` | ✅ | ✅ | Panasonic Digital Camera RAW |
| **Pentax RAW** | `.pef` | ✅ | ✅ | Pentax Electronic File |
| **Fujifilm RAW** | `.raf` | ✅ | ✅ | Fujifilm Digital Camera RAW |

### 5. Media, Typography & Code
| Format | Extension | Thumbnail | Preview | Description |
|---|---|:---:|:---:|---|
| **TrueType & OpenType Fonts** | `.ttf`, `.otf` | ✅ | ✅ | DirectWrite typography specimen layout |
| **Animated GIF** | `.gif` | ✅ | ✅ | Multi-frame animated image player |
| **Quite OK Image** | `.qoi` | ✅ | ✅ | Lossless fast image format |
| **Cinema 4D Scene** | `.c4d` | ✅ | ✅ | Maxon Cinema 4D scene |
| **Truevision Targa** | `.tga` | ✅ | ✅ | Game and texture raster format |
| **DirectDraw Surface** | `.dds` | ✅ | ✅ | Direct3D GPU compressed texture |
| **Markdown Documents** | `.md` | — | ✅ | GitHub Flavored Markdown typography renderer |
| **539 Code & Script Files** | `.cs`, `.cpp`, `.py`, `.rs`, `.ts`, `.json`, ... | — | ✅ | Syntax-highlighted code preview engine |

---

## 📥 Installation

ShellThumbs is available on the **Microsoft Store**:

* Download on the [Microsoft Store](#) *(Link coming soon with Store release)*

### System Requirements
* **Operating System**: Windows 11 (all versions) or Windows 10 (version 1809 or higher)
* **Architecture**: x64 (64-bit)

---

## 📝 Reporting Issues

When reporting an issue, please provide:
1. The **file extension** and the software that generated the file.
2. Your **Windows version** (run `winver`).
3. If possible, a non-confidential **sample file** reproducing the issue.

Thank you for helping us make ShellThumbs better!
