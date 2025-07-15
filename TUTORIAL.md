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
```
All options have inline comments. Customize to match your game needs:
• 	Use `ConsentRequired` to show onboarding UI
• 	Enable `DebugMode` to log session stats (if supported)
• 	Change `UITheme` to choose the style you like

---

## 🚀 Step 4: Understanding Remote Module Access
Roop’s system loads its internal logic from a protected MainModule on Roblox servers. You never modify this directly.
The `LoaderModule` uses:

```luau
return require(107376145207853)
```
So when your game runs:
• 	It connects to Roop’s remote code
• 	Loads services like `GroupManager`, `Analytics`, `MarkeplaceService`
• 	Keeps your local model small and safe
✅ This design ensures updates to core Roop logic happen automatically, without needing to re-insert models.

---

## 🧠 Step 5: Using Roop in Scripts
Once loaded, you can get the main Roop interface via:
```luau
local Roop = require(game.ServerScriptService:WaitForChild("MoreServices"))

-- Call services:
Roop:GetService("GroupManager"):AssignGroup(player, GroupID)
Roop:GetSetting("Analytics").Enabled
Roop:GetService("MarketplaceService"):PromptPurchase(Player, RoopAssetID)
```
Available functions may change as Roop evolves, so refer to the latest documentation.

---

## 🛡️ License & Restrictions
Use Roop responsibly. You may:
• 	Use it in your own game
• 	Customize the `Settings` and services
You may not:
• 	Re-upload Roop under your own name
• 	Modify the Loader to bypass licensing
• 	Access or clone the internal `MainModule`
Read the full Roop License for details.

---

## 🙋 Need Help?
For support or feedback:
• 	GitHub Issues: [DevQuest-Studio/Roop-Services](https://github.com/DevQuest-Studio/Roop-Services)
