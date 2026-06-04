[日本語](README.md) | **English**

# CammandoTab

A **Command+Tab app-switcher replacement** for macOS that always appears on the monitor where your cursor is.

On multi-monitor setups, the built-in Command+Tab switcher shows up on a display that doesn't match your intuition, which feels awkward. CammandoTab takes over the standard Command+Tab and always shows its own switcher **on the monitor under your mouse cursor**.

## Download

1. Download the latest `CammandoTab-<version>.zip` from [Releases](../../releases/latest).
2. Unzip it and move `CammandoTab.app` to your `Applications` folder.
3. On first launch you'll be asked for **Accessibility permission**.
   - Go to System Settings → Privacy & Security → Accessibility, **enable CammandoTab**, then relaunch the app (required to intercept the Command+Tab key input).
4. After changing the setting, quitting and relaunching the app once makes it take effect reliably.

The app is **notarized by Apple**, so it launches without Gatekeeper warnings.

## Usage

| Action | Behavior |
|--------|----------|
| `Command + Tab` | Show switcher / move to next app |
| `Command + Shift + Tab` | Move to previous app |
| Release `Command` | Switch to the selected app |
| `Esc` (while shown) | Cancel |
| Mouse | Hover to select, click to confirm |

Apps are ordered by **MRU (most recently used)**, just like the standard Command+Tab.
The Calendar.app icon shows **today's date**, just like the real Dock.

## Features

- Always shows the switcher **on the monitor under your mouse cursor** (multi-monitor friendly)
- Looks like the standard macOS switcher (translucent blur, selection highlight, app-name label)
- Orders apps by MRU (most recently used)
- Direct selection and click-to-confirm with the mouse
- Lives in the menu bar (not shown in the Dock), with an "open at login" option
- **Disable ⌘M / ⌘⌥M (window minimize)** via a menu toggle
- **Push the standard Dock off your main display** (jail it on a virtual display — handy alongside a high-function dock)

## Dock Jail: hide the standard Dock from your main display (virtual display)

If you use a high-function dock/launcher such as QuickQuay, the standard macOS Dock tends to just get in the way (minimizing can be suppressed with CammandoTab's "Disable ⌘M Minimize", and the Trash can be replaced by your high-function dock). However, macOS has no setting to "not show the standard Dock on a specific display."

So CammandoTab creates that "left extended display" itself, as a **virtual display** (a "Dock Jail"). Turn on "Dock Jail (Virtual Display)" from the menu, place that virtual display at the far left in System Settings, and set the Dock position to "Left" — then the standard Dock and the standard Command+Tab switcher disappear from your main display (the steps are explained in the menu item "How to Use Dock Jail…"). It's a workaround, but a practically effective one.

## Requirements

- **OS**: macOS 13.0 or later
- **Architecture**: Universal (Apple Silicon / Intel)
- **Signing**: Notarized by Apple (Developer ID)

## License / Author

Copyright © 2026 EVA Titer. All rights reserved.
