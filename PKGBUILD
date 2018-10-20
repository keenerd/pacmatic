# $Id: PKGBUILD 100043 2013-10-31 15:45:57Z kkeen $
# Maintainer: Kyle Keen <keenerd@gmail.com>
pkgname=pacmatic
pkgver=20141006
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
source=("http://kmkeen.com/$pkgname/$pkgname-$pkgver.tar.gz"
        "_pacmatic"
        "pacmatic.bash-completion")
md5sums=('1fe11adaa39aae9d3146ddbc3808eb23'
         '1c369c8fe595cbb41d04e214efd39a1e'
         '915cca3c2306ba74b3973afd64217700')

package() {
  cd "$srcdir/$pkgname"
  install -Dm0755 pacmatic                    "$pkgdir/usr/bin/pacmatic"
  install -Dm0755 cron-pacmatic               "$pkgdir/usr/bin/cron-pacmatic"
  install -Dm0644 pacmatic.1                  "$pkgdir/usr/share/man/man1/pacmatic.1"
  install -Dm0644 ../_pacmatic                "$pkgdir/usr/share/zsh/site-functions/_pacmatic"
  install -Dm0644 ../pacmatic.bash-completion "$pkgdir/usr/share/bash-completion/completions/pacmatic"
}

