# Home Assistant DashBoards

These files are referenced in [Lazy Tech Geek's YouTube video – Home Assistant Dashboards Explained (Views, Cards, Themes) – Part 1](https://www.youtube.com/@LazyTechGeek).

## ⚙️ Automation to switch between day and night theme

- Auto-switch between **day** and **night** themes using the sun entity
- Optional manual override using `input_boolean.theme_override`
- Depending on your setup, I've included example code for both single-file and split configuration.yaml configurations

---

## 📁 Included Files

### 🔄 `Automation - Theme Switch.txt`
Automation that toggles between light and dark themes:
- Follows the sun (`sun.sun`) by default
- Supports override with `input_boolean.theme_override` and `input_boolean.dark_theme`

📌 How to use:

Go to Settings > Automations & Scenes
Click + Create Automation > Click the three dots (⋮) in the top right and select Edit in YAML
Paste the contents of Automation - Theme Switch.txt
Click Save


### ⚙️ `configuration.yaml`
Link https://github.com/LazyTechGeek/HomeAssistant-DashBoards/blob/main/Automation%20-%20Theme%20Switch.txt
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
If you’re not seeing theme changes apply on all devices, make sure from profile > browser settings that the option “Use default theme" is selected and mode set to 'Auto' for mobile phones & tablets, or 'Light' for PCs

---

## ☕ Support the Channel
If you found this helpful, consider supporting Lazy Tech Geek:
[Buy Me a Coffee ☕](https://buymeacoffee.com/lazytechgeek)
