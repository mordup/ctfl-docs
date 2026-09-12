# Updating

CTFL can check for new releases automatically and, depending on how you installed it, update itself.

## Automatic update checks

By default, CTFL checks GitHub for new releases every 24 hours. You can change this in **Settings → Check for updates** (set to 0 to disable).

When an update is found, the tray menu item changes from "Check for Updates" to "Update to vX.Y.Z".

## Update behavior by install method

| Install method | What happens |
|---|---|
| **pip** | Downloads the new `.whl` and runs `pip install --upgrade`, then asks whether to restart now. |
| **AppImage** | Downloads the new AppImage and replaces the current one in place, then asks whether to restart now. |
| **AUR** (Arch Linux) | Update through your AUR helper: `yay -Syu ctfl`. Within a minute the tray notifies you and the menu entry becomes **Restart to use vX.Y.Z**. |
| **System package** (deb/rpm) | Opens the GitHub release page in your browser so you can download the new package. Once it is installed, the tray offers a restart the same way as for AUR. |

## Manual check

You can check for updates at any time from the tray menu: **Right-click → Check for Updates**.

If you're already on the latest version, a notification will confirm it.
