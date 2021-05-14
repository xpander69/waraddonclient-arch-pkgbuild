# Maintainer: xpander <xpander0 at gmail dot com>

pkgname=waraddonclient
_pkgname=WARAddonClient
pkgver=1.10.2
pkgrel=1
pkgdesc="Warhammer Return of Reckoning Addon Client"
arch=('x86_64')
url="https://github.com/Idrinth/WARAddonClient"
license=('MIT')
depends=('java-runtime')
source=("$_pkgname.jar::$url/releases/download/$pkgver/$_pkgname.jar"
        "$pkgname.desktop"
        "logo.png")
sha256sums=('SKIP'
            'SKIP'
            'SKIP')

package() {
	cd "$src"
	install -Dm644 $_pkgname.jar "$pkgdir/opt/$_pkgname/bin/$_pkgname.jar"
	install -Dm644 logo.png "$pkgdir/usr/share/pixmaps/$pkgname.png"
	install -Dm755 "$pkgname.desktop" -t "$pkgdir/usr/share/applications"
}
