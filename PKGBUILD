# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Furkan Kurt <afurkankurt@outlook.com>
pkgname=noble-quran.git
pkgver=0.1.r1.f78905c
pkgrel=1
epoch=
pkgdesc="Word of Allah in your terminal! In 3 diffirent languages with search functions."
arch=(x86_64 i686)
url="https://www.github.com/furkkurt/nobleQuran"
license=('GPL')
groups=()
depends=(less)
makedepends=(git)
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("git+$url")
noextract=()
md5sums=()
validpgpkeys=()

pkgver() {
	cd "${_pkgname}"
	printf "0.1.r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

build() {
	cd "${_pkgname}"
	make
}
check() {
  make -k check
}
package() {
	cd "${_pkgname}"
	make DESTDIR="$pkgdir/" install
}
sha256sums=('SKIP')
sha256sums=('SKIP')
sha256sums=('SKIP')
sha256sums=('SKIP')
sha256sums=('SKIP')
