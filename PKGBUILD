# Contributor: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20110321
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'wget' 'pacman-contrib' 'expac-git')
makedepends=()
optdepends=('vim: for vimdiff')
source=(http://kmkeen.com/pacmatic/$pkgname-$pkgver.tar.gz)
md5sums=('0a71d63c736c180008dc7689bc17a42d')

build() {
  cd "$srcdir"/$pkgname
  install -D -m 0755 pacmatic "$pkgdir"/usr/bin/pacmatic
}

