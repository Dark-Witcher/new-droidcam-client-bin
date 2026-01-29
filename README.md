# droidcam-client-bin (Arch Linux)

Arch Linux PKGBUILD for the **new official DroidCam desktop client** distributed by Dev47Apps.

⚠️ This is **NOT** the legacy DroidCam client and **NOT** DroidCam OBS.  
It repackages the **new Qt-based DroidCam client** provided upstream as a `.deb`.

## What this is
- Repackages the official `droidCam.client.setup.deb`
- Uses the **new DroidCam desktop client**
- Qt5-based GUI
- Works on **GNOME Wayland**
- Proprietary software

## What this is NOT
- Not the old DroidCam client
- Not `droidcam-obs`
- Not built from source
- Not an open-source implementation

## Build & Install

```bash
git clone https://github.com/Dark-Witcher/droidcam-client-bin.git
cd droidcam-client-bin
makepkg -si
