# Maintainer: Logan Allen <loganfynne at gmail dot com>
pkgname=chromium-update
pkgver=1.1
pkgrel=13
pkgdesc='Simple SH installer and updater of precompiled Chromium nightly builds'
arch=('any')
url="http://www.loganfynne.com/pkg/chromium-update.tar"
license=('GPL')
conflicts=('chromium')
depends=('gconf' 'libpng12' 'gtk2' 'dbus-glib' 'nss' 'alsa-lib' 'xdg-utils' 'bzip2' 'libevent' 'libxss' 'libxtst' 'ttf-dejavu' 'desktop-file-utils' 'hicolor-icon-theme' 'unzip')
source=('http://www.loganfynne.com/pkg/chromium-update.tar')
md5sums=('26846ca8759a47bd5a97e91df560b205')

package() {
  tar -xf chromium-update.tar
  mkdir -p ${pkgdir}/usr/share/applications
  mkdir -p ${pkgdir}/usr/bin
  cp `uname -m`/chromium-update ${pkgdir}/usr/bin/
  chmod +x ${pkgdir}/usr/bin/chromium-update
  cp chromium.desktop ${pkgdir}/usr/share/applications/
  cp chromium ${pkgdir}/usr/bin/
}
