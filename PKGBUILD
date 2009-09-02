# Contributor: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20090901
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('i686' 'x86_64')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'wget' 'pacman-contrib')
makedepends=()
optdepends=('vi' 'vim')
source=(http://kmkeen.com/pacmatic/$pkgname-$pkgver.tar.gz)
md5sums=('f8948f4ffb7135ad665a7cba63fbcb34')

build() {
  cd $startdir/src/$pkgname
  install -D -m 0755 pacmatic ${pkgdir}/usr/bin/pacmatic
}

