# Dynamic Island for Windows — Customized (Status Bar Edition)

A smooth, interactive always-on-top overlay for your desktop, built on the original Dynamic Island and repurposed as a lightweight **status bar**: a replacement for the parts of the bottom taskbar you actually glance at — the **time and battery** — plus live media, Wi‑Fi, privacy dots and system alerts, all in one compact pill at the top of the screen.

> **This is a customized / forked version of the original
> [Dynamic Island for Windows](https://github.com/devcode90/Dynamic-Island-for-Windows)
> by [devcode90 (Linus)](https://github.com/devcode90).**
> It keeps the original look and its core dashboards, and adds a different input model
> and a couple of new settings. See [What's different in this fork](#️-whats-different-in-this-fork).

---

## 📸 See it in Action

<p align="center">
  <img src="https://raw.githubusercontent.com/devcode90/Dynamic-Island-for-Windows/9fdd6610ff4e48928ecde99362a87f1d43afefbe/previews/desktop.png" alt="Dynamic Island running on the desktop" width="900" style="border-radius: 8px; margin: 10px;"/>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/devcode90/Dynamic-Island-for-Windows/9fdd6610ff4e48928ecde99362a87f1d43afefbe/previews/Full-preview-v2.png" alt="Dynamic Island surfaces" width="760" style="border-radius: 8px; margin: 10px;"/>
</p>

### Dashboards

| Media Player | Calendar | Weather | Game Overlay | Idle View |
| :---: | :---: | :---: | :---: | :---: |
| <img src="https://raw.githubusercontent.com/devcode90/Dynamic-Island-for-Windows/9fdd6610ff4e48928ecde99362a87f1d43afefbe/previews/media-v2.png" width="200" /> | <img src="https://raw.githubusercontent.com/devcode90/Dynamic-Island-for-Windows/9fdd6610ff4e48928ecde99362a87f1d43afefbe/previews/calendar.png" width="200" /> | <img src="https://raw.githubusercontent.com/devcode90/Dynamic-Island-for-Windows/9fdd6610ff4e48928ecde99362a87f1d43afefbe/previews/weather-v2.png" width="200" /> | <img src="https://raw.githubusercontent.com/devcode90/Dynamic-Island-for-Windows/9fdd6610ff4e48928ecde99362a87f1d43afefbe/previews/gamebar-v2.png" width="200" /> | <img src="https://raw.githubusercontent.com/devcode90/Dynamic-Island-for-Windows/9fdd6610ff4e48928ecde99362a87f1d43afefbe/previews/idle-v2.png" width="200" /> |

### Privacy Indicators

| Camera Detected | Microphone Detected |
| :---: | :---: |
| <img src="https://raw.githubusercontent.com/devcode90/Dynamic-Island-for-Windows/9fdd6610ff4e48928ecde99362a87f1d43afefbe/previews/camera-detected-v2.png" width="200" /> | <img src="https://raw.githubusercontent.com/devcode90/Dynamic-Island-for-Windows/9fdd6610ff4e48928ecde99362a87f1d43afefbe/previews/mic-detected-v2.png" width="200" /> |

---

## ✨ What it does

**Status bar at a glance:**

- 🕒 **Idle status view:** The collapsed idle dashboard shows the current **time** and **battery**, so you can check what you'd normally open the taskbar for without moving your mouse.
- 📶 **Wi‑Fi signal:** Signal quality is tracked from the WLAN interface.
- 🟢 **Privacy dots:** An orange dot when your mic is on, a green dot when your camera is on.
- 🎵 **Now playing:** Album art, title/artist, a live waveform and playback controls appear whenever media is playing.

**Core features:**

- 📅 **Dashboards:** Scroll the mouse wheel to switch between Media, Calendar and live Weather (via wttr.in).
- 📋 **Clipboard previews:** Instantly see copied text or an image thumbnail.
- 🔔 **Windows notifications:** Preview your latest notification with a high‑res app icon.
- 🔒 **Key alerts:** Quick popups when you hit Caps Lock or Num Lock.
- 🔋 **Battery & power:** Animations when you plug in, unplug, or hit low battery.
- 🔌 **USB & Bluetooth status:** Visual alerts when a drive or Bluetooth device connects/disconnects.
- 🔊 **Volume flyout:** A banner when the system volume changes, with the device name and mute state.
- ⏳ **Progress ring:** A ring around the island for downloads and file copies.
- 📊 **Game overlay:** Real‑time FPS, CPU, GPU and RAM stats built in.
- 🎨 **Themes:** OLED Black, Dark Gray, Midnight Blue, Deep Purple and Fluent Design, switchable from the right‑click menu.
- 🖥️ **Windows 11 style:** Swap the Apple pill for a modern Windows 11 rounded box.
- 🎢 **Fluid animations:** Hardware‑accelerated Direct2D spring animations with near‑zero idle CPU usage.

---

## ⚙️ Controls

| Input | Action |
| :--- | :--- |
| **Single click** | Open the Windows **Action Center** (`Win+A`) |
| **Double click** | Open the Windows **Notification Center** (`Win+N`) |
| **Middle click** | Toggle the default audio device mute |
| **Hover** | Expand the island (when "Expand on hover" is enabled) |
| **Scroll wheel** | Swipe between dashboard tabs |
| **Drag** | Move the island anywhere on screen |
| **Right click** | Theme, transparency, pin open, game‑overlay pin, reset position, Windhawk settings |

---

## 🛠️ What's different in this fork

Compared with the upstream mod, this fork changes how the island is used and adds a couple of options:

- **Reframed as a status bar:** Positioned as an always‑on‑top pill that replaces the need to glance at the taskbar for time and battery, while still expanding into the full dashboards when needed.
- **New input model:**
  - **Single click** now opens the **Action Center** (`Win+A`).
  - **Double click** now opens the **Notification Center** (`Win+N`).
  - A single click is **deferred** until the double‑click window expires, so a double click is never mistaken for a single click.
- **New `Double‑click delay (ms)` setting:** Choose how long the island waits for a possible second click (25 ms – 1000 ms). Windows default is 500 ms.
- **New `0.9x` Size scale option** for finer control over the island's size.

**Not included from the latest upstream release:** the focus timer, file shelf/tray, multi‑language support, the extended 8‑theme set, custom font families, audio‑spectrum styles, and backdrop blur/acrylic. This fork sticks to the core dashboards and a lean status‑bar experience.

---

## 🎛️ Customization

Configure everything from the **Windhawk Mod Settings** panel:

- **Position:** Top Center, Top Left, Top Right, or Bottom Center, with `Offset X` / `Offset Y` fine‑tuning.
- **Target monitor:** Primary, a specific display, or **Follow Mouse**.
- **Size scale:** 0.8x, 0.9x, 1.0x, 1.2x, 1.5x, 1.8x, 2.0x, 2.5x, with optional automatic DPI scaling.
- **Behavior:** Auto‑hide idle island, unhide on hover, always on top, expand on hover, animation speed, and **Double‑click delay**.
- **Style:** Native Windows 11 style toggle.
- **Colors & theming:** Accent color mode (Auto from album art / System / Custom hex), background/text hex colors, tint intensity, and pill transparency.
- **Modules:** Media, Clipboard, Battery, Progress, Game Overlay, metric labels, weather city and units.

> [!IMPORTANT]
> **The right‑click menu is per‑session, not persistent configuration.**
> Theme, Windows 11 style and pin‑open are re‑applied from your Windhawk settings every time the mod restarts, so a reboot or mod update discards whatever you picked from the menu. Set anything you want to keep in the **Mod Settings** tab instead.

### Notifications setup

To use the notification module:

1. Add `explorer.exe` to the process inclusion list under the **Advanced** tab of the mod settings, then restart the mod.
2. Allow apps to read notifications in **Settings → Privacy & security → Notifications → "Let apps access your notifications"**. If this is off, Windows denies the listener and no notification reaches the island.

---

## 📦 Installation

This is a [Windhawk](https://windhawk.net/) mod.

1. Install [Windhawk](https://windhawk.net/).
2. In Windhawk, open **Create a new mod** (or a local mod) and paste the contents of `main.cpp`, then click **Compile**.
3. Open the mod settings and configure appearance, colors and modules as you like.

---

## 💬 Let's Chat!

Found a bug or have an idea? Please open an issue on this fork's [GitHub repository](https://github.com/sunil-bhattaraii/windhawk-dynamic-island-fork/issues). For issues with the original mod, use the [upstream issues](https://github.com/devcode90/Dynamic-Island-for-Windows/issues).

---

## 🙌 Credits

Original project and contributors:

- **[devcode90 (Linus)](https://github.com/devcode90)** — Original author of [Dynamic Island for Windows](https://github.com/devcode90/Dynamic-Island-for-Windows), which this fork is based on.
- **[Sarthak Singh (sarthakaksh)](https://github.com/sarthakaksh)** — Major feature overhaul including the right‑click focus timer, hover clock, robust media controls, zero‑CPU instant hide shortcut, Bluetooth battery integration, image clipboard thumbnails, and full‑screen autohide fixes.
- **[ciizerr](https://github.com/ciizerr)** — UI alignment fixes, dashboard sizing, and calendar/weather polishing.
- **[ChrisSch-dev](https://github.com/ChrisSch-dev)** — Album title support, weather word wrapping, sleep/resume fixes, and performance/stability improvements.
- **[thevioletto](https://github.com/thevioletto)** — Custom font support, Windows Do Not Disturb integration, improved album‑art color extraction, and settings reorganization.
- **[David Ravelo (DavidRaveloU)](https://github.com/DavidRaveloU)** — Selectable audio spectrum styles, progress bar styles, track‑change animations, and brightness flyout.
- **[Retr0dev-jpg](https://github.com/Retr0dev-jpg)** — Event‑driven volume flyout and locale‑aware calendar.

This fork:

- **[sunil-bhattaraii](https://github.com/sunil-bhattaraii)** — Status‑bar reframing, single/double‑click Action/Notification Center actions, deferred single‑click handling with a configurable double‑click delay, and the 0.9x size scale option.

---

## 📜 License

MIT — see the [original project](https://github.com/devcode90/Dynamic-Island-for-Windows) for details.
