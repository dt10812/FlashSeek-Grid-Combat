# FlashSeek: Grid Combat 

![Platform Support](https://img.shields.io/badge/platforms-Windows%20%7C%20macOS%20%7C%20Linux-blue?style=flat-square)
![Engine](https://img.shields.io/badge/engine-Godot%204.5-orange?style=flat-square)
![Status](https://img.shields.io/badge/status-Pre--Release%20Alpha-red?style=flat-square)

Welcome to **FlashSeek: Grid Combat**, a high-octane 3D arcade brawler developed under the FlashSeek brand. Take control, manage your positioning on the grid, and neutralize waves of rogue security units before they breach your parameters.

## Core Mechanics & Features

* **Kinetic 3D Combat:** Fast-paced movement physics paired with responsive attack hitboxes and momentum calculation.
* **Responsive GUI Engine:** A procedurally scaling layout stack that dynamically recalculates bounding boxes and anchors to support any monitor resolution cleanly.
* **Vector Tracking AI:** Custom enemy navigation routines running client-side tracking, accompanied by nested 3D-to-2D floating viewport health bars.
* **Match State Triggers:** Fully integrated round management handling win/loss logic conditions and scene navigation loops.

---

## System Requirements

### Windows
* **Minimum:**
  * **OS:** Windows 10 (64-bit, version 1809 or higher for D3D12 support)
  * **Processor:** Dual-Core Intel Core i3 / AMD Ryzen 3 @ 2.5 GHz
  * **Memory:** At least **350 MB free RAM** available
  * **Graphics:** Intel HD Graphics 620 / AMD Radeon Vega 3 or better (Direct3D 12 or OpenGL 3.3 support) with at least **200 MB free VRAM** available
  * **Storage:** At least **200 MB free storage space** available

* **Recommended:**
  * **OS:** Windows 10 / 11 (64-bit)
  * **Processor:** Quad-Core Intel Core i5 / AMD Ryzen 5 or better
  * **Memory:** At least **512 MB free RAM** available
  * **Graphics:** NVIDIA GTX 1050 / AMD RX 560 or better (Vulkan 1.0 / Direct3D 12 native support) with at least **512 MB free VRAM** available
  * **Storage:** At least **200 MB free storage space** available

### macOS
* **Minimum:**
  * **OS:** macOS 10.12 (Sierra) for Intel Macs / macOS 11.0 (Big Sur) for Apple Silicon
  * **Processor:** Dual-Core Intel Core i5 (2015 or later) / Apple Silicon M1
  * **Memory:** At least **350 MB free RAM** available
  * **Graphics:** Intel Iris Graphics / Apple M1 Integrated GPU (OpenGL 3.3 / Metal) with at least **200 MB free VRAM** available
  * **Storage:** At least **200 MB free storage space** available

* **Recommended:**
  * **OS:** macOS 11.0 (Big Sur) or newer
  * **Processor:** Quad-Core Intel Core i7 / Apple Silicon M1 or better
  * **Memory:** At least **512 MB free RAM** available
  * **Graphics:** Intel Iris Plus / AMD Radeon Pro or Apple M1 GPU with at least **512 MB free VRAM** available
  * **Storage:** At least **200 MB free storage space** available

### Linux
* **Minimum:**
  * **OS:** Ubuntu 22.04 LTS / Fedora / Arch Linux (64-bit)
  * **Processor:** Dual-Core Intel/AMD @ 2.5 GHz
  * **Memory:** At least **350 MB free RAM** available
  * **Graphics:** Mesa Intel HD Graphics / AMD Radeon drivers (OpenGL 3.3 Core Profile or Vulkan 1.0 support) with at least **200 MB free VRAM** available
  * **Storage:** At least **200 MB free storage space** available
 
---

## Installation

Download the appropriate `.zip` file for your platform from the **[Releases](../../releases)** tab.

### Windows
1. Download `FlashSeek_GridCombat_v0.1-alpha1_Windows.zip`.
2. Extract the archive completely into a dedicated folder.
3. Launch `FlashSeek_GridCombat.exe`.

### Linux
1. Download `FlashSeek_GridCombat_v0.1-alpha1_Linux.zip` and extract its contents.
2. Open your terminal inside the extracted directory.
3. Grant execution permissions to the binary runner:
```bash
chmod +x FlashSeek_GridCombat.x86_64
```

## Release Cycle
The release cycle will not follow a specific schedule. Instead, we will tag the upcoming release 1-2 weeks before the release date.
