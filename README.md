# HomeAssistant-DashBoards
HomeAssistant DashBoards

# Home Assistant Theme Automation (Dark Mode, Day/Night Switching)

This repository contains example files to help you automatically switch between light and dark themes in Home Assistant — either based on sunrise/sunset or manually using input booleans.

These files are referenced in [Lazy Tech Geek's YouTube video – Home Assistant Dashboards Explained (Views, Cards, Themes) – Part 1](https://www.youtube.com/@LazyTechGeek).

---

## 🌗 Features

- Auto-switch between **day** and **night** themes using the sun entity
- Optional manual override using `input_boolean.theme_override`
- Compatible with both **single-file** and **split YAML** configurations

---

## 📁 Included Files

### 🔄 `Automation - Theme Switch.txt`
Automation that toggles between light and dark themes:
- Follows the sun (`sun.sun`) by default
- Supports override with `input_boolean.theme_override` and `input_boolean.dark_theme`

### ⚙️ `configuration.yaml`
If you're using a monolithic YAML setup:
- Includes theme definitions (`day`, `night`, and `day_and_night`)
- Adds the `input_boolean` definitions needed for manual override

### 🧠 `Input-boolean_dark_theme-overwrite.yaml`
For users with a split YAML setup (`!include_dir_merge_named`):
- Contains the two input booleans:
  - `input_boolean.dark_theme`
  - `input_boolean.theme_override`

### 🎨 `themes_day_night.yaml`
For users who split their themes into a separate file:
- Contains both **light** and **dark** theme definitions
- Includes an optional `day_and_night` theme with dual-mode support

---

## 🧠 Tip
If you’re not seeing theme changes apply on all devices, make sure each browser or app is set to use the “backend-selected” theme in its display settings.

---

## 📺 Watch the Video
📌 YouTube: [Home Assistant Dashboards Explained (Views, Cards, Themes) – Part 1](https://www.youtube.com/@LazyTechGeek)

---

## ☕ Support the Channel
If you found this helpful, consider supporting Lazy Tech Geek:
[Buy Me a Coffee ☕](https://buymeacoffee.com/lazytechgeek)
