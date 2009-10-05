# Contributor: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20091004
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'wget' 'pacman-contrib')
makedepends=()
optdepends=('vim')
source=(http://kmkeen.com/pacmatic/$pkgname-$pkgver.tar.gz)
md5sums=('8dc473930fcca5f1007626c3a38944b7')

build() {
  cd $startdir/src/$pkgname
  install -D -m 0755 pacmatic ${pkgdir}/usr/bin/pacmatic
}

