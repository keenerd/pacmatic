# Contributor: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20100204
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'wget' 'pacman-contrib')
makedepends=()
optdepends=('vim: for vimdiff')
source=(http://kmkeen.com/pacmatic/$pkgname-$pkgver.tar.gz)
md5sums=('544eeb9828af072a092d0f1cc50cd9bb')

build() {
  cd $startdir/src/$pkgname
  install -D -m 0755 pacmatic ${pkgdir}/usr/bin/pacmatic
}

