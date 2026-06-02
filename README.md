# BAMB/Build a Military Base Macro

## 📌 Prerequisites

Before running the macro, ensure your system meets the following requirements:

### 1. AutoHotkey v2
This macro is built entirely using features exclusive to AHK v2. 
* **Download:** [AutoHotkey Official Website](https://www.autohotkey.com/) (Make sure to download **v2.x**, not v1.1 or it will not work).

### 2. Windows WebView2 Runtime
The macro uses html for the ui via the `WebViewToo` library. 
* **Note:** The `WebViewToo` helper library is already **included inside this project folder** you do not need to download it separately.
* **System Requirement:** Your computer needs the core Microsoft WebView2 runtime installed. This is **installed by default on modern Windows 10 and Windows 11 systems**. If your GUI isn't loading, you can update it manually from Microsoft's website (But you should generally not have to).

### 3. Screen Resolution Support
* 🖥️ **All Resolutions Supported:** The macro and its UI are fully responsive and designed to work for all resolutions, as it minimizes your window to the smallest roblox allows, designed this way intentionally as I plan to use bitmap later for detection.

## ✨ Features yay

Automate the bamb shop
* **Select and customize what to buy** Filter and toggle specific items across multiple tiers (Common, Uncommon, Rare) and categories like Decoration, Production, Units, or Special tabs. 
* **Complete Buying Control:** Set exact item quantities, save your settings and selected items in to different profiles.

### ⚙️ Smart Settings & Utilities

* **Robux Prompt Detection:**
  * Automatically scans the center of the Roblox window every 500ms for unexpected purchase prompts.
  * **Custom Safety Actions:** Choose exactly what happens if a prompt is detected (Though it shouldn't be just a backup measurement):
    * **Close Roblox:** Instantly terminates `RobloxPlayerBeta.exe`.
    * **Pause Macro:** Halts the macro loop while leaving Roblox open.
    * **Exit Purchase:** Sends the `Escape` key to safely dismiss the prompt and quickly resumes your macro!


* **Extra Utilities**
  * **Spam Enter + Click:** Fast-click utility toggleable via the `F5` hotkey (designed for fast purchasing however as of today they have removed it I will still keep it if you want the auto clicker feature).


> [!IMPORTANT]
> **Notice regarding Robux Detection:**
> The current version of this macro relies on pixel color detection with color tolerance thresholds to scan for Robux prompts. Because color detection can occasionally be finicky depending on screen lighting or minor UI shifts this system is temporary.
> 
> I am actively working on improving this mechanics. In a future update, the macro will likely switch over to bitmap or something else, though it should suffice for now.
