# Contributor: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20090822
pkgrel=4
pkgdesc="Prevent Arch from bricking your system, and avoid other surprises."
arch=('i686' 'x86_64')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'wget' 'pacman-contrib')
makedepends=()
optdepends=()
source=(http://kmkeen.com/pacmatic/$pkgname-$pkgver.tar.gz)
md5sums=('61c8ae58c27e342fefc5a58396ead6e9')

build() {
  cd $startdir/src/$pkgname
  install -D -m 0755 pacmatic ${pkgdir}/usr/bin/pacmatic
}

