# Haul — Download Manager

Installers and automatic updates for **Haul**, a download manager for macOS and Windows:
multi-connection downloads that resume after any interruption, queues and a scheduler, video and
audio from streaming sites, and browser integration for Chrome, Edge, Brave, Arc, Vivaldi, Opera,
Helium and Firefox.

## Download

Get the newest version from **[Releases → Latest](https://github.com/AdkHex/Haul-Releases/releases/latest)**:

| System | File |
|---|---|
| macOS 11 or later, Apple Silicon (M1–M4) | `Haul_<version>_aarch64.dmg` |
| Windows 10 / 11, 64-bit | `Haul_<version>_x64-setup.exe` |
| Windows without installing | `Haul_<version>_x64-portable.zip` |

Once installed, Haul keeps itself up to date. It checks for a new version shortly after it starts
and every few hours, or right away with **Help → Check for Updates…**. Running downloads pause for
the restart and continue in the new version. You can turn automatic checks off in
**Options → General**.

## Installing

### macOS
1. Open the `.dmg` and drag **Haul** into **Applications**. Start it from Applications, not from the
   DMG window.
2. Haul is not signed by Apple yet, so macOS blocks the first launch. Right-click Haul in
   Applications → **Open** → **Open**, or go to **System Settings → Privacy & Security** and click
   **Open Anyway**. If macOS says the app "is damaged", run this in Terminal, then open Haul again:
   ```sh
   xattr -dr com.apple.quarantine /Applications/Haul.app
   ```

### Windows
1. Run `Haul_<version>_x64-setup.exe`. No administrator rights are needed.
2. The installer is not signed yet, so SmartScreen may warn: **More info → Run anyway**.

Portable: unzip `Haul_<version>_x64-portable.zip` anywhere and run `Haul.exe`. Keep `haul-host.exe`
and the `extension` folder next to it.

## Browser extension

Start Haul once first. It keeps an up-to-date copy of the extension on your disk:

| | Folder |
|---|---|
| Windows | `%APPDATA%\com.haul.app\extension\` |
| macOS | `~/Library/Application Support/com.haul.app/extension/` |

- **Chrome, Edge, Brave, Arc, Vivaldi, Opera, Helium**: open `chrome://extensions` (or `edge://`,
  `brave://`, …), turn on **Developer mode**, click **Load unpacked**, then paste the folder path
  above plus `chromium` into the dialog's address bar (macOS: press ⌘⇧G first). Pick the folder
  that directly contains `manifest.json`.
- **Firefox**: `about:debugging` → **This Firefox** → **Load Temporary Add-on** → `manifest.json` in
  the `firefox` folder. Firefox removes temporary add-ons when it restarts.

Click the Haul icon in the browser toolbar: it should say "Connected". Downloads you start in the
browser now open in Haul.

## Good to know

- Merging separate video and audio streams needs **ffmpeg** (macOS: `brew install ffmpeg`; Windows:
  put it in `C:\ffmpeg\bin` or on the `PATH`). Normal downloads don't need it.
- If you report a problem, include the logs from `~/Library/Application Support/com.haul.app/logs`
  (macOS) or `%APPDATA%\com.haul.app\logs` (Windows).
