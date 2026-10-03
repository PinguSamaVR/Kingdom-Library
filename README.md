# Kingdom

**Your library, your rules.**

Current public release: **Kingdom 1.1.4**

Kingdom is a local Windows game-library manager created by PinguSama. It helps
you organize, install, launch, update, back up, restore, and remove locally
managed games from one interface. Kingdom does not provide games, downloads,
repacks, cracks, DRM bypasses, or links to unauthorized content.

Kingdom works offline, requires no account, and does not require a cloud
service to manage the local library.

## Download

- **GitHub Releases:** https://github.com/PinguSamaVR/Kingdom-Library/releases
- **itch.io:** https://pingusama.itch.io/kingdom-library

Download the complete Windows release and keep all bundled files together.
The corresponding sources required for covered third-party components are
published separately from the proprietary Kingdom application as a release
asset and alongside the itch.io distribution.

## Main features

- Local game library with custom cover images.
- Guided installation from configured repack folders using external installers.
- Launch installed games and track local play time.
- Automatic executable detection with manual selection when needed.
- Open the game folder, repack/source folder, and related local paths.
- Remove an installed game through a guarded uninstall flow.
- Update Manager for a single update package at a time.
- Supported update archive formats: ZIP, 7Z, and RAR.
- Automatic or manual updater selection.
- Local archive of successfully applied update packages.
- Save Manager with backup, restore, delete, and open-folder operations.
- Automatic save backup before an update when configured and available.
- Optional removal of local save data during uninstall, with explicit
  confirmation and backup-oriented warnings.
- Guided first-run folder configuration.
- English, Italian, Spanish, German, and French interface languages.

## Requirements

- Windows.
- Permission to access the folders selected for the library, games, repacks,
  updates, and save backups.
- Sufficient disk space for installation, extraction, update staging, and
  backups.

Some installers or update programs may request Windows elevation. Kingdom does
not bypass Windows security prompts and does not modify games by itself when an
external installer or updater is responsible for that operation.

## Installation

1. Download Kingdom only from an official Kingdom distribution channel.
2. Extract or install the complete release as instructed for that release.
3. Keep all distributed files together, including the `tools` directory and
   legal or license files.
4. Start Kingdom and complete the first-run folder configuration.

Do not remove bundled runtime or third-party files. An incomplete distribution
may not start or may be unable to process supported archives.

## Library workflow

Add a game to the library and select the appropriate local source. Kingdom can
use the configured automatic game folder or a folder chosen by the user. When
an executable cannot be identified safely, Kingdom asks for an explicit manual
selection.

Kingdom stores its own settings and management metadata locally. Games and
user-supplied files remain under the paths selected by the user.

## Linked installations

Kingdom can discover an existing installation under a selected games folder,
or the user can explicitly link an installation folder from the game-card
menu. Name matching helps propose and rank candidates, but the validated,
persisted linked folder becomes the authoritative location for installed
status, launch, executable selection, updates, saves, and uninstall actions.

Changing the default games root does not move or silently relink an existing
game. A validated folder with an unusual name can still be linked manually,
and the same folder cannot be linked to two different library entries.

When launching a game, Kingdom resolves executable candidates inside the
linked installation and remembers an explicit manual selection when needed.

When uninstalling, Kingdom searches for compatible local uninstallers only
inside the linked installation folder. Windows uninstall metadata may confirm
identity or provide arguments, but it is not mandatory when a unique safe
local uninstaller is available. If Kingdom cannot verify a suitable uninstall
route, it does not start one or delete the installation. Without confirming
metadata, successful removal is verified from the disappearance of the linked
folder; an uncertain result does not trigger save or local-data cleanup.

## Update Manager

The Update Manager handles one update package per operation. It can normalize
a folder or a ZIP, 7Z, or RAR archive, identify an updater, copy the known game
path for use in the external updater, and monitor the launched updater's
technical exit status.

An exit status of zero means only that the external updater did not report a
technical error. It is not proof that every game file was updated correctly.
Users should verify the game after each update.

After a technically successful update, Kingdom preserves the original archive
when one exists, or creates a ZIP for a folder-only update, and places the
result in the per-game `Update Archive` location. Destructive cleanup occurs
only after the destination archive has been created or copied and verified.

## Save Manager

The Save Manager operates only on folders that the user explicitly selects or
confirms. It can create local backups, restore a selected backup, delete save
data with confirmation, and open the relevant folder.

Backups reduce risk but do not guarantee recoverability. Users should keep
independent copies of important save data, especially before updates,
uninstalls, or manual file operations.

## Privacy

Kingdom is designed as an offline local utility. It does not require an
account, advertising profile, or Kingdom-operated cloud service to manage the
library. External programs launched by the user, Windows, games, installers,
updaters, distribution platforms, and linked third-party services have their
own behavior and policies.

Kingdom does not require an account or a Kingdom-operated online service.
Questions about privacy or compliance may be sent to
`pingusama.info@gmail.com`.

## Security and support

- Read [SECURITY.md](SECURITY.md) before reporting a vulnerability.
- Read [SUPPORT.md](SUPPORT.md) for normal bugs, installation questions, and
  feature requests.

Do not publish credentials, personal data, copyrighted game files, or
unauthorized download links in reports.

## Legal notice

Kingdom is a local management utility. Users are responsible for ensuring that
they have the right to possess and use every game, archive, installer, update,
save file, and other item managed through Kingdom. Kingdom does not include or
authorize piracy-related content or activity.

## License and third-party software

The original Kingdom code, branding, documentation, and proprietary assets are
proprietary. See [LICENSE.md](LICENSE.md) for the applicable
Kingdom license.
Kingdom is not an open-source project, and no publication of a third-party
component's source code makes Kingdom's proprietary source code open source.

Third-party software, fonts, tools, and assets remain governed by their own
licenses and notices. Those licenses control for their respective components
and may grant rights that the Kingdom license does not restrict. Keep all
third-party notices included with an official distribution. See
[THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt),
[COMPONENTS.txt](COMPONENTS.txt), and the [LICENSES](LICENSES) directory.
For LGPL-covered components, also see
[BUILDING-AND-RELINKING.txt](BUILDING-AND-RELINKING.txt) and
[OPEN-SOURCE-SOURCE-AVAILABILITY.txt](OPEN-SOURCE-SOURCE-AVAILABILITY.txt).

## Distribution

Subject to the Kingdom license, the complete, official, unmodified Kingdom
distribution may be shared without charge for lawful, non-commercial purposes.
It may not be sold, offered as a paid feature, misleadingly rebranded, or
bundled with malware, adware, or unwanted software.

## Project status

Kingdom is independently developed and maintained by PinguSama. Features,
platform support, and availability may change in later releases.

---

**Kingdom 1.1.4 — PinguSama**
