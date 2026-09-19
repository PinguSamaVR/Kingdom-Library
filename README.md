# Kingdom

**Your library, your rules.**

A lightweight, offline game library manager for Windows.

Kingdom keeps your local game collection organized and under your control, bringing repacks, installed games, covers, playtime, updates, save backups, local folders, and common management actions together in one clean interface.

> **Current release:** Kingdom 1.1.2

## Download

- **GitHub Releases:** https://github.com/PinguSamaVR/Kingdom-Library/releases
- **itch.io:** https://pingusama.itch.io/kingdom-library

Download the complete Windows release and keep all bundled files together.

## Highlights

- Local library management in a single interface
- Installed / not installed filters and library search
- Install, launch, and uninstall actions
- Automatic and manual launch-executable selection
- Local files and repack-folder access
- Custom and automatic cover selection
- Persistent playtime tracking
- Game Update Manager
- Automatic ZIP, 7Z, and RAR update handling
- Per-game **Update Archive**
- Save Manager with backup, restore, delete, and open-folder actions
- Automatic save backup before game updates when available
- Clean uninstall option for local game data and saves
- Existing-backup warning when reinstalling a game
- Configurable repack and installation folders
- First-launch setup wizard
- Fully offline operation
- No account or registration required
- Five interface languages

## Supported languages

- English
- Italiano
- Español
- Deutsch
- Français

## Installation

1. Download and extract the complete Kingdom release.
2. Keep `Kingdom.exe` together with all bundled files and folders.
3. Launch `Kingdom.exe`.
4. Windows may request permission when Kingdom starts an installer, updater, game, or uninstaller with elevated privileges. Approve only when you recognize the action.

Python is **not required** for end users.

## First launch

Kingdom guides you through the initial setup:

1. Select your language.
2. Choose the folder containing your repacks.
3. Choose your game installation folder.

If you let Kingdom create the installation folder automatically, the default path is:

```text
C:\KingdomGames
```

You can also select another folder manually.

## Library

Each game card can show its cover, title, repack size, installation status, installed size, and tracked playtime.

Use the library filters and search bar to quickly find games.

Depending on the current state, the main action becomes:

- `INSTALL`
- `LAUNCH`
- `UNINSTALL`

## Installing a game

1. Press `INSTALL`.
2. Kingdom prepares the expected installation path.
3. Copy the path when requested.
4. Open the installer.
5. Use the proposed path in the installer.

If Kingdom detects existing save backups for that game, it warns you before continuing.

## Launching a game

Press `LAUNCH` after installation.

Kingdom tries to identify the correct executable automatically and remembers the selected file.

If the wrong executable is detected, open the game-card gear menu and use **Launch executable** to choose the correct one manually.

## Save Manager

After the game has been launched through Kingdom, open:

```text
Gear menu → Saves
```

You can:

- create a save backup;
- restore a previous backup;
- delete the current local saves;
- open the original save folder.

Backups are stored by game inside:

```text
Savedata backup
```

Kingdom keeps multiple backups without silently overwriting earlier ones.

Before restoring a backup, Kingdom tries to create a safety backup of the current saves when possible.

## Updating a game

Open:

```text
Gear menu → Update
```

Kingdom can work with supported update folders and ZIP, 7Z, or RAR archives.

Follow the guided procedure and use the installation path shown by Kingdom when the external updater asks for it.

Before an update, Kingdom tries to back up the current saves when their location is known.

Completed updates are archived by game inside:

```text
Update Archive
```

Kingdom currently handles **one update at a time**.

## Uninstalling a game

Press `UNINSTALL` and follow the confirmation prompts.

A **Clean uninstall** option can also remove detected local save data and related local game data.

Existing backups stored in `Savedata backup` are preserved.

## Game-card gear menu

The gear menu provides quick access to actions such as:

- Cover
- Repack path
- Local files
- Playtime
- Update
- Saves
- Launch executable
- Delete repack

When deleting a repack, Kingdom can separately ask whether the archived updates for that game should also be removed.

Save backups are kept separate.

## Covers

You can select a cover manually.

If no cover is already configured, Kingdom can automatically use an image found directly in the repack folder when there is exactly one valid candidate.

Supported formats include:

`PNG`, `JPG`, `JPEG`, `WEBP`, `BMP`

## Playtime

Kingdom tracks playtime while a launched game process is running.

Tracked time is persistent and can be reset from the available playtime controls after confirmation.

## Settings

From Settings you can manage:

- folders;
- language;
- playtime;
- Kingdom reset;
- tutorial / FAQ;
- other application information.

Changing the interface language takes effect immediately.

## Resetting Kingdom

The reset makes Kingdom forget the configured repack and installation folders so the initial setup appears again at the next launch.

It does **not** delete your games, repacks, save backups, or other personal files.

## Legal note

Kingdom is a local library and game-management utility.

It does **not** provide games, repacks, download sources, cracks, DRM-bypass tools, or piracy links. Use Kingdom only with files and software obtained lawfully.

## Closed-source project

Kingdom is distributed as proprietary software. The source code is not published in this repository.

## Author

Created by **PinguSama**.

Thanks for downloading, trying, and supporting Kingdom. Feedback is always welcome.

---

**Kingdom 1.1.2**  
*Your library, your rules.*
