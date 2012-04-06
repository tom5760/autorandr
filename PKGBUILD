# Maintainer: Tom Wambold <tom5760@gmail.com>
# Maintainer: Ng Oon-Ee <ngoonee.talk@gmail.com>
# Contributor (auto-disper-git): Byron Clark <byron@theclarkfamily.name>
pkgname=autorandr-git
pkgver=20120406
pkgrel=1
pkgdesc="Auto-detect connected display hardware and load appropriate X11 setup using xrandr or disper. Formerly auto-disper."
url="http://github.com/tom5760/autorandr"
arch=('any')
license=('None')
optdepends=('disper')
conflicts=('auto-disper-git')
makdepends=('git')

#_gitroot="http://github.com/tom5760/autorandr.git"
#_gitname=autorandr

build() {
  install -D -m 0755 $srcdir/../autorandr ${pkgdir}/usr/bin/autorandr
  install -D -m 0755 $srcdir/../autorandr-monitor ${pkgdir}/usr/bin/autorandr-monitor
  ln -s /usr/bin/autorandr ${pkgdir}/usr/bin/auto-disper
  install -D -m 0755 $srcdir/../pm-utils/40autorandr ${pkgdir}/etc/pm/sleep.d/40autorandr
  install -D -m 0755 $srcdir/../bash_completion/autorandr ${pkgdir}/etc/bash_completion.d/autorandr
}
# vim: set ft=sh ts=2 sw=2 et:
