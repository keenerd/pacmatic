# Maintainer: Somasis <somasis@cryptolab.net>
# Original Maintainer: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic-fork
pkgver=r50.056515f
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://github.com/Somasis/pacmatic-fork"
license=('GPL')
depends=('pacman' 'bash' 'pacman-contrib' 'expac')
makedepends=()
optdepends=('vim: for vimdiff'
            'html2text: for prettier news')
conflicts=('pacmatic')
provides=('pacmatic')
source=(git+https://github.com/Somasis/$pkgname.git)
md5sums=(SKIP)

pkgver() {
    cd "$pkgname"
    printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
    cd "$pkgname"
    install -D -m 0755 pacmatic      "$pkgdir/usr/bin/pacmatic"
    install -D -m 0755 cron-pacmatic "$pkgdir/usr/bin/cron-pacmatic"
    install -D -m 0644 pacmatic.1    "$pkgdir/usr/share/man/man1/pacmatic.1"
}

