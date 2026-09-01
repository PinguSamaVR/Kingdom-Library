# Kingdom

**Your library, your rules.**

A lightweight, offline Steam-like game library manager for Windows.

Kingdom is designed to keep your local game collection organized, accessible, and entirely under your control. It brings repacks, installed games, covers, playtime, local folders, and common game-management actions together in one clean interface.

> **Current release:** Kingdom 1.0.1

## Download

The current public release is available on itch.io:

**https://pingusama.itch.io/kingdom-library**

GitHub Releases will also be used for packaged Windows builds.

## Features

- Local game library management in a single interface
- Installed / not installed filtering
- Repack and installed-size information
- Install, launch, and uninstall actions
- Local files access for installed games
- Repack-folder access from each game card
- Custom cover selection
- Automatic cover detection when exactly one valid image is present
- Persistent playtime tracking
- Playtime reset tools
- Repack management and deletion tools
- Configurable repack and installation folders
- First-launch setup wizard
- Fully offline operation
- No account or registration required
- Multilingual interface

## Supported languages

- English
- Italiano
- Español
- Deutsch
- Français

## Installation

1. Download the complete Kingdom release folder.
2. Keep `Kingdom.exe` together with the `_internal` folder and all bundled resources.
3. Do **not** move `Kingdom.exe` out of the release folder.
4. Launch `Kingdom.exe`.
5. Windows may request permission when Kingdom starts installers, games, or uninstallers with elevated privileges. Approve only when you recognize the action.

Python is **not required** for end users. Kingdom is distributed as a compiled Windows application.

## First launch

On first launch, Kingdom guides you through the initial setup:

1. Select your language.
2. Choose the folder containing your repack folders.
3. Choose how Kingdom should handle the game installation folder:
   - allow Kingdom to create one automatically; or
   - select an existing folder manually.

If Kingdom creates the folder automatically, it creates a folder named:

```text
installed Kingdom Games
```

inside the parent folder that contains your repack folder.

## Folder structure

Kingdom expects each repack to be stored in its own subfolder.

Example:

```text
Repacks/
├─ Game One/
├─ Game Two/
└─ Game Three/
```

Kingdom identifies installed games by checking whether the expected game folder exists inside the configured installation folder.

Example:

```text
Installed Games/
└─ Game One/
```

If you select an installation folder that already contains games, Kingdom can recognize them when:

- the corresponding repack is also present in the library;
- the installed folder name matches the title Kingdom expects.

More advanced recognition of already-installed games is planned for a future version.

## Library

The main library displays repacks as game cards. Each card can show:

- cover image;
- game title;
- repack size;
- installation status;
- installed size;
- tracked playtime;
- `INSTALL`, `LAUNCH`, or `UNINSTALL` actions depending on the game state.

### Filters

Use:

- `ALL`
- `INSTALLED`
- `NOT INSTALLED`

for quick library filtering.

## Installing a game

1. Press `INSTALL` on a game card.
2. Kingdom prepares the expected installation path.
3. Copy the path shown in the installation window.
4. Press `OPEN INSTALLER`.
5. Kingdom launches `setup.exe` from the repack folder with elevated privileges.
6. Paste the proposed path into the game installer when needed.

Kingdom does not replace the original installer. It helps keep installation paths consistent.

## Launching a game

When Kingdom detects a game as installed, `INSTALL` becomes `LAUNCH`.

Press `LAUNCH` to start the detected game executable. Kingdom may request elevated privileges.

## Uninstalling a game

1. Press `UNINSTALL`.
2. Confirm the action.
3. Kingdom searches the Windows uninstall registry entries for the game.
4. If a valid uninstaller is found, Kingdom launches it.
5. Complete the uninstall procedure.
6. If the installation folder still exists afterward, Kingdom can ask whether you want to remove the remaining files.

Always review destructive prompts carefully before confirming.

## Game-card gear menu

Press the gear icon on a game card to open the quick menu.

### Cover
Select a cover manually.

### Path
Open the repack folder.

### Local files
Visible only when the game is installed. Opens the detected installation folder.

### Playtime
Reset the recorded playtime after confirmation.

### Delete repack
Permanently deletes the entire repack folder after two confirmations.

> **Warning:** `Delete repack` removes the repack folder from disk. This operation is irreversible.

## Covers

### Manual cover
Use the gear menu → **Cover** and select a supported image.

### Automatic cover
If no cover is already configured, Kingdom checks the repack folder:

- **0 valid images:** no action;
- **exactly 1 valid image:** Kingdom assigns it automatically;
- **2 or more valid images:** no automatic choice is made.

Kingdom does not automatically overwrite an already configured cover.

Supported formats:

`PNG`, `JPG`, `JPEG`, `WEBP`, `BMP`

## Playtime

Kingdom tracks playtime while it detects a game process running from the configured installation folder.

Playtime is saved persistently and can be reset from:

- the game-card gear menu;
- `Settings → Playtime`.

## Settings

### Folders
Change the repack folder and game installation folder.

### Repack management
Open repack management, delete repacks, or reset the initial folder configuration.

### Language
Change the interface language. The interface updates immediately.

### Playtime
Select a game and reset its tracked playtime.

### About Kingdom
Access the tutorial / FAQ and other information pages.

## Resetting the initial configuration

Go to:

```text
Settings → Repack management → RESET
```

The reset:

- forgets the configured repack folder;
- forgets the configured installation folder;
- does **not** delete, move, or modify any file or folder.

After two confirmations, the first-launch wizard appears again on the next start.

## Planned improvements

Future development currently includes improvements such as:

- smarter recognition of games that are already installed;
- local save-game management.

## Legal note

Kingdom is a local library and game-management utility.

It does **not** provide games, repacks, download sources, cracks, DRM-bypass tools, or piracy links. Kingdom is intended to manage local files and software that users have obtained lawfully.

## Closed-source project

Kingdom is distributed as proprietary software. The source code is not published in this repository.

## Author

Created by **PinguSama**.

---

**Kingdom 1.0.1**  
*Your library, your rules.*