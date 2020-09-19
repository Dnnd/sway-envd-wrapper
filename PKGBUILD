# Maintainer: Danila Maslennikov <d.v.maslennikov@outlook.com>
pkgname=sway-envd-git
pkgver=1.0.0
pkgrel=1
pkgdesc="Wrapper to load env variables in sway session"
arch=("any")
url="https://github.com/Dnnd/sway-envd-wrapper"
license=('MIT')
groups=()
depends=()
makedepends=('git')
provides=("${pkgname%-git}")
conflicts=("${pkgname%-git}")
replaces=()
backup=()
options=()
install=
source=('git+https://github.com/Dnnd/sway-envd-wrapper.git')
noextract=()
md5sums=('SKIP')

pkgver() {
	cd "$srcdir/${pkgname%-git}"
	git describe --long | sed 's/\([^-]*-\)g/r\1/;s/-/./g'
}

package() {
	cd "$srcdir/${pkgname%-git}"
	install -Dm755 $srcdir/sway-envd-wrapper $pkgdir/usr/bin/sway-envd-wrapper
	install -Dm644 $srcdir/sway-envd.desktop $pkgdir/usr/share/wayland-sessions/sway-envd.desktop
}
