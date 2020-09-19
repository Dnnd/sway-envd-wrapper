# Maintainer: Danila Maslennikov <d.v.maslennikov@outlook.com>
pkgname=sway-envd
pkgver=1.0.0
pkgrel=1
pkgdesc="Wrapper to load env variables in sway session"
arch=("any")
url="https://github.com/Dnnd/sway-envd-wrapper"
license=('MIT')
groups=()
depends=()
makedepends=('sway')
provides=("${pkgname%}")
conflicts=("${pkgname%}")
replaces=()
backup=()
options=()
install=
source=("sway-envd-wrapper"
	"sway-envd.desktop")
noextract=()
md5sums=('SKIP'
	 'SKIP')

package() {
	install -Dm755 "$srcdir/sway-envd-wrapper" "$pkgdir/usr/bin/sway-envd-wrapper"
	install -Dm644 "$srcdir/sway-envd.desktop" "$pkgdir/usr/share/wayland-sessions/sway-envd.desktop"
}
