# DualCommander

Native two-panel file manager for **macOS 13+**, with Intel and Apple silicon support. Classic Norton blue styling, keyboard-first file operations, previews, editor, Apple Photos originals export, and per-file copy retry/skip handling.

## Downloads

Get the latest files from [Releases](https://github.com/emanuilexpress/DualCommander/releases/latest):

- **DualCommander-Installer.pkg** installs into `/Applications`. Quit all Commander copies first. Existing settings, bookmarks, drafts, history and recovery files are preserved.
- **DualCommander-USB.dmg** runs from its mounted image or a USB drive. Keep the disk image intact on exFAT drives.
- **SHA256SUMS.txt** lists download checksums.

This local build is **ad-hoc signed; its installer is unsigned and not Apple-notarized**. macOS may require **Open Anyway** in System Settings > Privacy & Security if you trust the download. Managed Macs may block it. Follow [Apple's instructions](https://support.apple.com/102445); do not disable security protections.

## Software updates

Use **DualCommander > Check for Updates… (Option-Command-U)** or the command palette. The app verifies an Ed25519-signed release manifest, streams the installer to a private partial file, then checks its exact size and SHA-256. Invalid signatures and damaged downloads are rejected. Daily launch checks are optional and off initially; enable and save them in the update window.

Finish file operations and save editor changes before opening the verified installer. Quit Commander, finish in macOS Installer, then open the updated app from Applications. Installation may require administrator authorization. The package refuses to replace a running app or downgrade a newer build. Updates never install silently. A portable copy is kept intact; its installer updates the Applications edition.

Update feed: `https://github.com/emanuilexpress/DualCommander/releases/latest/download/update.json`.
Only the public verification key is shipped. The private publisher key is never uploaded to this repository. The publisher signature is separate from Apple's Developer ID/notarization system.

## Help and permissions

F1 opens context help; Command-Shift-P opens the command palette. Tab switches panels; Command-A selects files; F5 copies; F4 edits. Preferences offers Classic Norton and other themes. Some Mac keyboards need fn/globe for function keys.

Photos and file access require permission on each Mac. The USB app does not carry cloud logins or permissions. Photos exports are original media files, not a complete backup of Photos album organization or edits.

This is a release-download repository. Demo images, when included, are concept artwork rather than app screenshots. The initial public build has automated updater/menu checks and a universal compile; actual Installer authorization and live UI still need user validation.
