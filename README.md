# Command & Conquer 3: Tiberium Wars/Kane's Wrath - Setup Guide

This guide will help you configure **C&C3: Tiberium Wars/Kane's Wrath** on modern systems, fix common crashes, and install custom maps and mods.

---

## Multiplayer

There are two main ways to play multiplayer. You only need to set up one method:

### Option 1: C&C:Online (Recommended)

1. Create an account on **C&C:Online**: [https://cnc-online.net/en/](https://cnc-online.net/en/)
2. [Install](https://cnc-online.net/en/download/) and launch the client, I use the "Tacitus version" which automatically applies the above patches for multiplayer, so you don't have to do the fixes below.
3. Launch the game → **Multiplayer** → **Online** and log in with your C&C:Online account.
4. You can now join public games or create a private match.

**Video Guide:** [YouTube Tutorial](https://www.youtube.com/watch?v=24uFA1MCaqk)

### Option 2: LAN / Direct IP

1. Ensure all players are on the same network (or use a VPN like Hamachi or SoftEther for remote LAN play).
2. Launch the game → **Multiplayer** → **LAN** or **Direct IP**.
3. Enter the host’s IP address to join.

**Tips for multiplayer stability:**

- All players should use the same game version, maps, and mods.
- Avoid mods that increase FPS, as the game speed is affected by FPS: [More info](https://www.reddit.com/r/commandandconquer/comments/o9lhs5/question_how_do_i_make_tiberium_wars_run_this/)
- Apply the **[4GB patch](#4gb-patch-fix)** to all clients if using large maps or mods (Tacitus client already does this).
- Use **[cnc-ddraw](#alt-tab-crashes-fix)** to prevent alt-tab crashes mid-game (Tacitus client already does this).

---

## Fixes
You don't need to add these when you already use Tacitus client installed from the [Multiplayer section](#option-1-cconline-recommended).

### Alt-Tab Crashes Fix

Modern Windows versions can cause crashes when alt-tabbing. To fix this:

1. Download **cnc-ddraw** and follow the instructions:  
   [https://github.com/FunkyFr3sh/cnc-ddraw](https://github.com/FunkyFr3sh/cnc-ddraw)

2. Optionally: after installation, you can use `cnc-ddraw config.exe` to configure settings, or manually change them in `cnc-ddraw.ini`.

<br>

### 4GB Patch Fix

Large maps or mods may trigger errors such as:

```
Direct3D error (E_OUTOFMEMORY) 22 addresses
```

To fix this:

1. Download the **4GB Patch**: [https://ntcore.com/4gb-patch/](https://ntcore.com/4gb-patch/)
2. Run `4gb_patch.exe`.
3. When prompted, navigate to your game installation folder:
   - For Steam: Right-click the game → **Properties** → **Installed Files** → **Browse…**
   - Open the `RetailExe` folder → select the folder with the latest version (or your custom version).
4. Select `cnc3game.dat` (or the closest equivalent) to patch.
5. Launch the game; large maps and mods should now load correctly.

**Video Guide:** [YouTube Tutorial](https://www.youtube.com/watch?v=8r3gD4Xdq1E)

---

## Custom Maps

1. Download custom maps from sites like **CnCLabs** or this collection of 760 maps:  
   [https://steamcommunity.com/sharedfiles/filedetails/?id=1503194353](https://steamcommunity.com/sharedfiles/filedetails/?id=1503194353)

2. On Windows 8 and later, navigate to:

`C:\Users\<username>\AppData\Roaming\<game_name>`
for example: `C:\Users\Bob\AppData\Roaming\Command & Conquer 3 Tiberium Wars`

3. Create a folder named `Maps`.
4. Extract the downloaded maps into this folder.

---

## Custom Mods

1. For Steam users:

   - Right-click the game → **Properties** → **General**
   - Add `-ui` in the **Launch Options** box

2. On Windows 8 and later, navigate to:

`C:\Users\<username>\Documents\<game_name>`
for example: `C:\Users\Bob\Documents\Command & Conquer 3 Tiberium Wars`

3. Create a folder named `Mods`.
4. Place your custom mods in this folder.
