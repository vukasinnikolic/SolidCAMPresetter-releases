# SolidCAM Presetter

Internal tool for SolidCAM support: switch SolidCAM between setups in one
click. It points a SolidCAM version at a main folder (CAM-Parts,
post-processors, machine simulation), makes SOLIDWORKS load that SolidCAM
version and restarts SOLIDWORKS.

Built by Vukasin Nikolic - SolidCAM International Support Serbia.

**Download the latest version** (now 1.4.2):
[SolidCAMPresetter.zip](https://github.com/vukasinnikolic/SolidCAMPresetter-releases/raw/main/SolidCAMPresetter.zip)
or the exe on its own:
[SolidCAMPresetter.exe](https://github.com/vukasinnikolic/SolidCAMPresetter-releases/raw/main/SolidCAMPresetter.exe).
The zip gets through mail, chat and browsers that block a bare `.exe`.

1. Right-click the downloaded file -> Properties -> tick **Unblock** -> OK (the
   app is not code-signed yet). For the zip, then unzip it.
2. Run `SolidCAMPresetter.exe` (Windows 10/11, nothing else to install).
   "Install for you" adds a Start menu shortcut and the Explorer right-click
   entry, with no administrator rights. A newer version run the same way
   asks to update the installed copy.

**Administrator rights.** Switching between installs of the same SolidCAM
version (e.g. 2026 and 2026 DV) needs none. Switching to another version
(e.g. 2026 → 2025) registers it for the computer, because SOLIDWORKS only
loads a version registered for the computer: Windows asks once per switch.

- With the default UAC setting, an administrator account sees "Do you want
  to allow this app to make changes to your device?" (*Publisher: Unknown*,
  the app is not code-signed yet): Yes. A standard account is asked for an
  administrator's user name and password.
- With UAC on "Never notify", an administrator account is not asked at all;
  a standard account cannot switch versions.
- No, or Cancel: SOLIDWORKS stays as it was, and the app says so.

**Unregister SolidCAM** disconnects every SolidCAM version from SOLIDWORKS
(the same Windows prompt when one is registered for the computer); Register
add-in connects one again. **Dark mode** is in the *View* menu.

Do not run the app as administrator to skip this: dragging folders and zips
from Explorer onto it stops working, and mapped drive letters may be missing.

Found a bug or have an idea? *Help → Report a bug or request a feature* in
the app, or [open an issue here](https://github.com/vukasinnikolic/SolidCAMPresetter-releases/issues/new/choose) (needs a GitHub
account). This repository is public: leave out customer names, case numbers
and paths you cannot share.

Earlier versions are in [versions](versions). This repository only holds the
downloads; the source code is private.
