# Author: Fokke Zandbergen <mail@fokkezb.nl>
# Maintainer: fokkezb <mail@fokkezb.nl>
_npmname=gittio
pkgname=nodejs-gittio
pkgver=0.4.4
pkgrel=1
pkgdesc="Install Titanium modules and Alloy widgets"
arch=(any)
url="http://gitt.io/cli"
license=(Apache Public License v2)
depends=('nodejs')
optdepends=()

package() {
  cd $srcdir
  local _npmdir="$pkgdir/usr/lib/node_modules/"
  mkdir -p "$_npmdir"
  cd "$_npmdir"
  npm install -g --prefix "$pkgdir/usr" $_npmname@$pkgver
}
