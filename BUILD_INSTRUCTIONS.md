# 🌟 Stellar External - Build Instructions

<div align="center">

![Stellar](https://img.shields.io/badge/Stellar-External-blue?style=for-the-badge)
![Version](https://img.shields.io/badge/Version-2026-green?style=for-the-badge)
![Roblox](https://img.shields.io/badge/Roblox-Compatible-red?style=for-the-badge)

**A powerful external tool for Roblox with advanced features**

[Features](#-features) • [Requirements](#-requirements) • [Installation](#-installation) • [Usage](#-usage) • [Troubleshooting](#-troubleshooting)

</div>

---

## 📋 Table of Contents

- [Features](#-features)
- [System Requirements](#-system-requirements)
- [Development Requirements](#-development-requirements)
- [Installation Guide](#-installation-guide)
- [Building the Project](#-building-the-project)
- [Usage](#-usage)
- [Keybinds](#-keybinds)
- [Troubleshooting](#-troubleshooting)
- [Offsets Updates](#-offsets-updates)
- [Disclaimer](#-disclaimer)

---

## ✨ Features

### 🎯 Combat Features
- **Aimbot** - Automatic target acquisition and tracking
- **Triggerbot** - Automatic shooting when crosshair is on target
- **Silent Aim** - Invisible aim assistance
- **Anti-Lock** - Counter anti-cheat detection

### 🏃 Movement Features
- **Speed Hack** - Adjustable movement speed
- **Custom WalkSpeed** - Precise speed control
- **Jump Power** - Enhanced jumping capabilities

### 👁️ Visual Features
- **ESP (Extra Sensory Perception)** - Player visualization
  - Box ESP
  - Name ESP
  - Health ESP
  - Distance ESP
  - Team ESP

### 🛠️ Additional Features
- **Custom Menu** - User-friendly ImGui interface
- **Keybind System** - Customizable hotkeys
- **Real-time Updates** - Live game state monitoring

---

## 💻 System Requirements

### Minimum Requirements
- **OS**: Windows 10/11 (64-bit)
- **RAM**: 4GB minimum, 8GB recommended
- **Processor**: Intel Core i3 or AMD equivalent
- **Graphics**: DirectX 11 compatible GPU
- **Storage**: 500MB free space

### Software Requirements
- **Roblox**: Latest version installed
- **Administrator Rights**: Required for memory access
- **.NET Framework**: 4.7.2 or higher

---

## 🔧 Development Requirements

### Required Software

#### 1. **Visual Studio 2022** (Recommended)
Download from: https://visualstudio.microsoft.com/downloads/

**Required Workloads:**
- ✅ Desktop development with C++
- ✅ Windows 10/11 SDK (latest version)

**Required Individual Components:**
- ✅ MSVC v143 - VS 2022 C++ x64/x86 build tools (Latest)
- ✅ C++ ATL for latest v143 build tools (x86 & x64)
- ✅ C++ MFC for latest v143 build tools (x86 & x64)
- ✅ Windows 10/11 SDK (10.0.22621.0 or newer)
- ✅ C++ CMake tools for Windows
- ✅ C++ Clang tools for Windows

#### 2. **DirectX SDK**
- DirectX 11 SDK (included in Windows SDK)
- D3D11 libraries
- D3DCompiler

#### 3. **Additional Libraries** (Included in Project)
- **ImGui** - GUI framework
- **FreeType** - Font rendering
- **Detours** - Function hooking
- **libcurl** - HTTP requests

---

## 📦 Installation Guide

### Step 1: Clone or Download the Repository

```bash
git clone https://github.com/yourusername/stellar-external.git
cd stellar-external
```

Or download the ZIP file and extract it.

### Step 2: Install Visual Studio 2022

1. Download Visual Studio 2022 Community (Free)
2. Run the installer
3. Select **"Desktop development with C++"** workload
4. In the **Individual Components** tab, ensure these are checked:
   - MSVC v143 build tools
   - Windows 10/11 SDK (latest)
   - C++ ATL and MFC libraries
5. Click **Install** and wait for completion

### Step 3: Install Windows SDK

If not included with Visual Studio:
1. Download from: https://developer.microsoft.com/en-us/windows/downloads/windows-sdk/
2. Install with default options
3. Ensure DirectX components are selected

---

## 🔨 Building the Project

### Method 1: Using Visual Studio IDE

1. **Open the Solution**
   - Navigate to the project folder
   - Double-click `rwar.sln`
   - Visual Studio will open the project

2. **Configure Build Settings**
   - Select **Release** configuration (top toolbar)
   - Select **x64** platform (top toolbar)
   
   ```
   Configuration: Release
   Platform: x64
   ```

3. **Restore NuGet Packages** (if prompted)
   - Right-click on Solution → **Restore NuGet Packages**
   - Wait for completion

4. **Build the Project**
   - Press `Ctrl + Shift + B` or
   - Go to **Build** → **Build Solution**
   - Wait for compilation to complete

5. **Locate the Output**
   - The compiled executable will be in:
   ```
   stellar/x64/Release/stellar.exe
   ```

### Method 2: Using Command Line (MSBuild)

1. **Open Developer Command Prompt**
   - Search for "Developer Command Prompt for VS 2022"
   - Run as Administrator

2. **Navigate to Project Directory**
   ```cmd
   cd path\to\stellar-external
   ```

3. **Build the Solution**
   ```cmd
   msbuild rwar.sln /p:Configuration=Release /p:Platform=x64
   ```

4. **Output Location**
   ```
   stellar/x64/Release/stellar.exe
   ```

---

## 🎮 Usage

### Starting the Application

1. **Disable Antivirus** (Temporarily)
   - Add `stellar.exe` to exclusions
   - Windows Defender may flag it as false positive

2. **Run as Administrator**
   - Right-click `stellar.exe`
   - Select **"Run as administrator"**
   - This is **REQUIRED** for memory access

3. **Launch Roblox**
   - Start Roblox after Stellar is running
   - Or start Stellar while Roblox is already open
   - Wait for initialization messages

4. **Initialization Messages**
   ```
   [stellar leaked XD] Starting Stellar initialization...
   [stellar leaked XD] Initializing driver system...
   [DEBUG] Roblox window found
   [DEBUG] Process ID: XXXXX
   [SUCCESS] Found RobloxPlayerBeta.exe
   [stellar leaked XD] New driver system initialized successfully!
   ```

5. **Open the Menu**
   - Press **INSERT** key to toggle menu
   - Menu will appear as overlay on Roblox window

---

## ⌨️ Keybinds

### Default Hotkeys

| Key | Function |
|-----|----------|
| **INSERT** | Toggle Menu (Show/Hide) |
| **F1** | Toggle Aimbot |
| **F2** | Toggle ESP |
| **F3** | Toggle Speed Hack |
| **F4** | Toggle Triggerbot |

### Menu Navigation

| Key | Function |
|-----|----------|
| **Mouse** | Navigate menu |
| **Left Click** | Select/Toggle options |
| **ESC** | Close menu (or press INSERT) |

### Customization

All keybinds can be customized through the menu:
1. Open menu (INSERT)
2. Navigate to **Settings** tab
3. Click on keybind field
4. Press desired key
5. Changes save automatically

---

## 🎨 Menu Features

### Main Tabs

#### 🎯 Combat Tab
- Aimbot settings
  - FOV (Field of View)
  - Smoothness
  - Target selection
  - Visibility checks
- Triggerbot settings
  - Delay
  - Burst mode
- Silent aim options

#### 👁️ Visuals Tab
- ESP options
  - Box ESP (2D/3D)
  - Name tags
  - Health bars
  - Distance display
  - Team colors
- Color customization
- Visibility filters

#### 🏃 Movement Tab
- Speed multiplier
- Jump power
- Hip height
- Anti-lock settings

#### ⚙️ Settings Tab
- Keybind configuration
- Performance options
- Debug information
- Offset updates

---

## 🔧 Troubleshooting

### Common Issues

#### ❌ "Failed to initialize new driver system!"

**Causes:**
- Not running as Administrator
- Antivirus blocking
- Outdated offsets
- Roblox not running

**Solutions:**
1. **Run as Administrator**
   ```
   Right-click stellar.exe → Run as administrator
   ```

2. **Disable Antivirus**
   - Add to Windows Defender exclusions:
   ```
   Windows Security → Virus & threat protection → 
   Manage settings → Exclusions → Add folder
   ```

3. **Update Offsets**
   - Check `OFFSETS_UPDATE_LOG.md`
   - Visit: https://imtheo.lol/Offsets/Offsets.hpp
   - Join Discord: https://discord.gg/rbxoffsets

4. **Check Roblox**
   - Ensure Roblox is running
   - Try restarting both applications

#### ❌ "Roblox window not found!"

**Solution:**
- Start Roblox first
- Wait for Roblox to fully load
- Then start Stellar

#### ❌ Menu not showing (INSERT key not working)

**Solutions:**
1. Check if Roblox window is focused
2. Try pressing INSERT multiple times
3. Check if another program is using INSERT key
4. Restart Stellar

#### ❌ Features not working in-game

**Solutions:**
1. **Update Offsets**
   - Roblox updates frequently
   - Check for offset updates
   
2. **Check Game Compatibility**
   - Some games have additional anti-cheat
   - Try different games

3. **Verify Settings**
   - Ensure features are enabled in menu
   - Check keybinds are correct

#### ❌ Compilation Errors

**Missing SDK:**
```
Error: Windows SDK not found
```
**Solution:** Install Windows 10/11 SDK from Visual Studio Installer

**Missing Libraries:**
```
Error: Cannot open include file 'd3d11.h'
```
**Solution:** Install DirectX SDK / Windows SDK

**Linker Errors:**
```
Error LNK2001: unresolved external symbol
```
**Solution:** 
- Clean solution (Build → Clean Solution)
- Rebuild (Build → Rebuild Solution)

---

## 🔄 Offsets Updates

### Current Version
- **Roblox Version**: `version-df7528517c6849f7`
- **Last Updated**: February 18, 2026
- **Source**: https://imtheo.lol/Offsets/Offsets.hpp

### How to Update Offsets

1. **Check Current Version**
   - Open `stellar/src/stellar/stellar.hpp`
   - Look for version comment at top

2. **Get Latest Offsets**
   - Visit: https://imtheo.lol/Offsets/Offsets.hpp
   - Copy the new offsets

3. **Update File**
   - Replace offsets in `stellar.hpp`
   - Update version comment
   - Rebuild project

4. **Automatic Updates** (Future)
   - Join Discord for notifications
   - https://discord.gg/rbxoffsets

### Signs You Need to Update

- ❌ "Failed to initialize new driver system!"
- ❌ "Failed to get Visual Engine"
- ❌ "Failed to get DataModel"
- ❌ Features not working after Roblox update

---

## 📚 Additional Resources

### Documentation
- `TROUBLESHOOTING.md` - Detailed troubleshooting guide
- `OFFSETS_UPDATE_LOG.md` - Complete offset changelog
- `README.md` - Project overview

### Community
- **Discord**: https://discord.gg/rbxoffsets (Offsets updates)
- **GitHub Issues**: Report bugs and request features

### Learning Resources
- **ImGui Documentation**: https://github.com/ocornut/imgui
- **DirectX 11 Tutorial**: https://docs.microsoft.com/en-us/windows/win32/direct3d11
- **C++ Reference**: https://en.cppreference.com/

---

## ⚠️ Disclaimer

```
╔══════════════════════════════════════════════════════════════╗
║                    IMPORTANT DISCLAIMER                       ║
╠══════════════════════════════════════════════════════════════╣
║                                                               ║
║  This software is provided for EDUCATIONAL and RESEARCH      ║
║  purposes ONLY.                                              ║
║                                                               ║
║  • Use at your own risk                                      ║
║  • May violate Roblox Terms of Service                       ║
║  • Can result in account termination                         ║
║  • No warranty or support provided                           ║
║  • Authors not responsible for misuse                        ║
║                                                               ║
║  By using this software, you acknowledge and accept          ║
║  all risks and consequences.                                 ║
║                                                               ║
╚══════════════════════════════════════════════════════════════╝
```

### Legal Notice

- This project is **NOT affiliated** with Roblox Corporation
- Using this software may result in **permanent account ban**
- The developers are **NOT responsible** for any consequences
- This is a **leaked/archived** project for educational purposes
- **No official support** or updates are provided

### Ethical Use

- Use only on **test accounts**
- Do not use to harm other players' experience
- Respect game developers and their work
- Learn from the code, don't abuse it

---

## 🙏 Credits

### Original Developers
- Original development: 2022-2023
- Fixed driver implementation
- Community contributions

### Libraries Used
- **ImGui** - Dear ImGui by Omar Cornut
- **FreeType** - Font rendering library
- **Detours** - Microsoft Research
- **libcurl** - Data transfer library

### Special Thanks
- **theo** (imtheo.lol) - Offset dumper
- **RbxOffsets Discord** - Community support
- All contributors and testers

---

## 📝 Version History

### v2026 (Current)
- ✅ Fixed driver system
- ✅ Updated offsets (Feb 2026)
- ✅ Added diagnostic logging
- ✅ Improved stability
- ✅ Enhanced menu UI

### v2023 (Original)
- Initial release
- Basic features
- Original driver implementation

---

<div align="center">

### 🌟 Star this repository if you found it useful!

**Made with ❤️ for the Roblox development community**

[⬆ Back to Top](#-stellar-external---build-instructions)

</div>
