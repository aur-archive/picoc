# $Id: pkgbuild-mode.el,v 1.23 2007/10/20 16:02:14 juergen Exp $
# Maintainer: perlawk
pkgname=picoc  
pkgver=2.1
pkgrel=2 
pkgdesc="PicoC is a very small C interpreter for scripting."
url="http://code.google.com/p/picoc"
arch=('x86_64' 'i686')
license=('BSD')
depends=()
makedepends=()
conflicts=()
replaces=()
backup=()
install=
source=(http://picoc.googlecode.com/files/$pkgname-$pkgver.tar.bz2)
md5sums=('6505fb108d195bad0854c7024993cc24')
build() {
  cd $startdir/src/$pkgname

  make || return 1
}
package() {
  cd $startdir/src/$pkgname
  install -d $pkgdir/usr/bin
  install -t $pkgdir/usr/bin picoc
}

