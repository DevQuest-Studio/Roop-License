# 📚 Roop Services Setup Tutorial (Remote Module Edition)

Welcome! This guide walks you through how to integrate **Roop Services** into your Roblox game using the official model loader system. The core logic is hosted remotely inside `MainModule`, so you won’t see or edit that directly.

---

## 🔧 What You’ll Need

- The **Roop Model Folder** (from GitHub or Roblox Studio)
- Proper placement of Roop folders inside your game workspace
- Active internet connection (for remote require call)

---

## 📦 Step 1: Import the Roop Model

After downloading or inserting the Roop model:
- Place the top-level `Roop` folder into `Workspace`
- Make sure it contains:

| Folder or Script     | Description                                     |
|----------------------|-------------------------------------------------|
| `Core/LoaderModule`  | Connects to the remote MainModule via `require()` |
| `Modules/Settings`   | Configuration for Roop behavior and features   |
| `READ_ME`, `LICENSE` | Documentation and terms                        |
| `ThumbnailCamera` | You can delete, it for the tumbnail image |

---

## 🛠 Step 2: Enable Required Services

Before launching your game:

- Go to **Home > Game Settings > Security**
- Enable the following:
  - ✅ `APIService` — used for player verification and data ops
  - ✅ `Third Party Sales` — required by some Roop commerce flows

These settings are **mandatory** for Roop to function properly.

---

## ⚙️ Step 3: Configure Roop Settings

Inside `Modules > Settings`:

```lua
return {
  config.OutputEnable = true
config.UpdateNotify = true
config.ConsentRequired = true
config.DebugMode = false
config.UITheme = "Legacy" -- ====== IT STILL IN DEV AND IT NOT AVAILABLE DON'T CHANGE ======
}
