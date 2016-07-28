# Maintainer: Anselmo L. S. Melo <anselmo.melo@intel.com>
pkgname=qgroundcontrol
pkgver=3.0.0
pkgrel=1
pkgdesc="Micro air vehicle ground control station."
arch=('any')
url="http://qgroundcontrol.org/"
license=('GPL3')
depends=(\
  'espeak'  # optional but you have to decide if you want it at built-time\
  'qt5-svg' 'qt5-graphicaleffects' 'qt5-webkit' 'phonon-qt4' 'qt5-serialport'\
  'qt5-quickcontrols')

source=('https://github.com/mavlink/qgroundcontrol/releases/download/v'${pkgver}'/qgroundcontrol.tar.bz2')
md5sums=('10ce90dd55c31ac769ba62278053c3e9')

package() {
  mkdir -p "${pkgdir}/opt" "${pkgdir}/usr/bin"
  cp -R "$srcdir/${pkgname}" "${pkgdir}/opt/qgroundcontrol"
  ln -s "/opt/qgroundcontrol/qgroundcontrol-start.sh" "${pkgdir}/usr/bin/qgroundcontrol"
}

# vim:set ts=2 sw=2 et:
