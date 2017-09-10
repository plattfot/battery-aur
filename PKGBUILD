# Maintainer: Fredrik Salomonsson <plattfot@gmail.com>
pkgname=battery
pkgver=1.1.0
pkgrel=1
epoch=
pkgdesc="Simple battery monitor for i3blocks"
arch=('x86_64')
url="https://github.com/plattfot/battery"
license=('GPL3')
groups=()
depends=()
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=ChangeLog
source=("$pkgname-$pkgver::git+https://github.com/plattfot/battery.git#tag=v$pkgver")
noextract=()
md5sums=('SKIP') #generate with 'makepkg -g'

build() {
	cd "$pkgname-$pkgver"
	make
}

package() {
	cd "$srcdir/$pkgname-$pkgver"
	mkdir -p $pkgdir/usr/bin
	make PREFIX="$pkgdir/usr/bin" install
}


