# Contributor: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20100202
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'wget' 'pacman-contrib')
makedepends=()
optdepends=('vim')
source=(http://kmkeen.com/pacmatic/$pkgname-$pkgver.tar.gz)
md5sums=('75ec92cda21382852f60a8f34e1acf90')

build() {
  cd $startdir/src/$pkgname
  install -D -m 0755 pacmatic ${pkgdir}/usr/bin/pacmatic
}

