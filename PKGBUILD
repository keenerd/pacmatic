# Contributor: Kyle Keen <keenerd@gmail.com>
# Contributor: Christophe-Marie Duquesne <chm.duquesne@gmail.com>
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
source=(pacmatic--lib pacmatic cron-pacmatic)
md5sums=('e623d1d805c69a0c90c23cf042198580'
         '3c6bdb4d14f875ca021b45ffe14ff866'
         '4ebe242252bd0945953ff687f5dcec6b')

build() {
  install -D -m 0644 pacmatic--lib "$pkgdir"/usr/lib/pacmatic--lib
  install -D -m 0755 pacmatic "$pkgdir"/usr/bin/pacmatic
  install -D -m 0755 cron-pacmatic "$pkgdir"/usr/bin/cron-pacmatic
}

