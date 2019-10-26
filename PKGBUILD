# Maintainer: Allen Choong <allencch at hotmail dot com>
pkgname=compiz-session
pkgver=0
pkgrel=1
pkgdesc="Compiz standalone"
arch=('any')
url=""
license=('GPL')
depends=('compiz' 'xterm' 'dex')
source=(compiz-session
        compiz-session-logout
        compiz-session.desktop)
md5sums=('51542ae1f8c27e06fe43fd52cbd32a78'
         '138716c3bdd0c66e236d40956756910a'
         '695bc9924ed97e81bf243872f2c4686f')
noextract=()

package() {
  mkdir -p "$pkgdir/usr/share/xsessions"
  mkdir -p "$pkgdir/usr/bin"

  cd "$srcdir"

  install -m644 compiz-session.desktop "$pkgdir/usr/share/xsessions"
  install -m755 compiz-session "$pkgdir/usr/bin"
  install -m755 compiz-session-logout "$pkgdir/usr/bin"
}

# vim:set ts=2 sw=2 et:
