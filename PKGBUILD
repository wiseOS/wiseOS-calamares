 # Maintainer: MetalNeox 
pkgname=arcolinux-calamares-git
_pkgname=arcolinux-calamares
_destname="/etc/calamares"
pkgver=19.09
pkgrel=8
pkgdesc="Calamares for wiseos"
arch=('any')
url="https://github.com/wiseos/wiseos-calamares"
license=('GPL3')
makedepends=('git')
depends=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${_pkgname}::"git+https://github.com/wiseos/${_pkgname}.git")
sha256sums=('SKIP')
install='readme.install'
package() {
	mv "${srcdir}/${_pkgname}/"LICENSE "${pkgdir}${_licensedir}${_pkgname}/LICENSE"
	mkdir -p "${pkgdir}${_destname}"
	cp -r "${srcdir}/${_pkgname}/calamares/"* "${pkgdir}${_destname}"
}
