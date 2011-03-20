# Contributor: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20110320
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'wget' 'pacman-contrib' 'expac')
makedepends=()
optdepends=('vim: for vimdiff')
source=(http://kmkeen.com/pacmatic/$pkgname-$pkgver.tar.gz)
md5sums=('3a18fdabf0f6607241f9a9d2ec54a303')

build() {
  cd "$srcdir"/$pkgname
  install -D -m 0755 pacmatic "$pkgdir"/usr/bin/pacmatic
}

