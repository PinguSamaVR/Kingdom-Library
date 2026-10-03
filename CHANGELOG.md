# Changelog

All notable public changes to Kingdom will be documented here.

## 1.1.4 — 2026-10-03

### Added
- Existing-installation discovery and an explicit manual linking workflow.
- Release-specific third-party notices, component inventory, source
  availability, patch statement, and replacement/relinking information.

### Improved
- Unified each game's persisted installation binding across installed status,
  launch, executable selection, updates, save handling, and uninstall flows.
- Made product-name matching more conservative while allowing a validated
  folder with an unusual name to be linked explicitly.
- Hardened post-install verification and prevented one folder from being
  linked to multiple games or silently replacing an invalid binding.
- Restricted local uninstaller discovery to the linked installation folder;
  Windows uninstall metadata can confirm identity and arguments but is no
  longer mandatory for a unique safe local uninstaller.
- Strengthened persistence migration, save-backup safety, update-source
  preservation, staged-repack handling, and interface state refreshes.

### Notes
- Kingdom remains closed-source proprietary software.
- Corresponding sources for covered third-party components are distributed as
  a separate release asset; Kingdom's proprietary source code is not included.
- The Windows runtime was qualified with 395 passing automated tests and a
  completed real-user runtime validation.

## 1.0.1 — 2026-09-01

### Added
- First-launch setup wizard.
- Multilingual interface: English, Italian, Spanish, German, and French.
- Library filters for all, installed, and not installed games.
- Local files shortcut for installed games.
- Manual and automatic cover handling.
- Persistent playtime tracking and reset tools.
- Repack management tools.
- Configurable repack and installation folders.
- Tutorial / FAQ section.

### Improved
- Language switching now applies immediately.
- Window and header icon handling.
- Settings navigation and back-button behavior.
- General interface polish and stability.

### Notes
- Kingdom is distributed as a closed-source Windows application.
- Smarter recognition of already-installed games and local save-game management are planned for a future release.
