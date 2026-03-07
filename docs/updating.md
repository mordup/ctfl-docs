# Updating

CTFL can check for new releases automatically and, depending on how you installed it, update itself.

## Automatic update checks

By default, CTFL checks GitHub for new releases every 24 hours. You can change this in **Settings → Check for updates** (set to 0 to disable).

When an update is found, the tray menu item changes from "Check for Updates" to "Update to vX.Y.Z".

## Update behavior by install method

| Install method | What happens |
|---|---|
| **pip** | Downloads the new `.whl` and runs `pip install --upgrade`. Restarts automatically. |
| **AppImage** | Downloads the new AppImage and replaces the current one in place. Restarts automatically. |
| **System package** (deb/rpm/pacman) | Opens the GitHub release page in your browser so you can download the new package. |

## Manual check

You can check for updates at any time from the tray menu: **Right-click → Check for Updates**.

If you're already on the latest version, a notification will confirm it.
