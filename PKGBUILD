# Maintainer: Dark Witcher <archlinux.sulfide764@passmail.net>

pkgname=droidcam-client-bin
pkgver=20260129
pkgrel=1
pkgdesc="DroidCam client (prebuilt binary)"
arch=('x86_64')
url="https://www.dev47apps.com/"
license=('custom')

depends=(
  'qt5-base'
  'qt5-svg'
  'qt5-wayland'
  'alsa-lib'
  'libpulse'
)

source=("droidcam_client_amd64.deb::https://droidcam.app/go/droidCam.client.setup.deb")
sha256sums=('a7b613fb5e5732c3d60a4c8da6527862b4936d8aa7d3e1bd1723dc9f2a52a989')

package() {
  ar x "$srcdir"/droidcam_client_amd64.deb
  tar -xf data.tar.* -C "$pkgdir"

  # Remove forbidden non-Arch paths
  rm -rf "$pkgdir/usr/local"

  # Always provide a license file (proprietary upstream)
  install -Dm644 <(echo "Proprietary software. See https://www.dev47apps.com/ for license terms.") \
    "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}


