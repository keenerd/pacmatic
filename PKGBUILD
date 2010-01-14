# Contributor: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20100114
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'wget' 'pacman-contrib')
makedepends=()
optdepends=('vim')
source=(http://kmkeen.com/pacmatic/$pkgname-$pkgver.tar.gz)
md5sums=('f11e023af6ef1335a5642c83bdf925db')

build() {
  cd $startdir/src/$pkgname
  install -D -m 0755 pacmatic ${pkgdir}/usr/bin/pacmatic
}

