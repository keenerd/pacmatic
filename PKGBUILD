# $Id: PKGBUILD 100043 2013-10-31 15:45:57Z kkeen $
# Maintainer: Kyle Keen <keenerd@gmail.com>
# Maintainer: Erik Nelson <erik@nsk.io>
pkgname=pacmatic
pkgver=movefix
pkgrel=1
pkgdesc="A pacman wrapper to avoid bricking your system and such other surprises."
arch=('any')
url="http://kmkeen.com/pacmatic/"
license=('GPL')
depends=('pacman' 'bash' 'expac')
makedepends=()
optdepends=('vim: for vimdiff'
            'html2text: for prettier news'
            'fakeroot: for cron-pacmatic script')
source=("https://github.com/eriknelson/pacmatic/archive/move-fix.tar.gz"
        "_pacmatic")
md5sums=('d3d08a542a314a4392ef86de71d34b21'
         '1c369c8fe595cbb41d04e214efd39a1e')

package() {
  cd "$srcdir/$pkgname"
  install -Dm0755 pacmatic      "$pkgdir/usr/bin/pacmatic"
  install -Dm0755 cron-pacmatic "$pkgdir/usr/bin/cron-pacmatic"
  install -Dm0644 pacmatic.1    "$pkgdir/usr/share/man/man1/pacmatic.1"
  install -Dm0644 ../_pacmatic  "$pkgdir/usr/share/zsh/site-functions/_pacmatic"
}

