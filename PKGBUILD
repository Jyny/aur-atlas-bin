# Maintainer: Jerry Y. Chen <chen@jyny.dev>

pkgname=atlas-bin
pkgdesc="A modern tool for managing database schemas"
pkgver=0.26.0
pkgrel=1
binary=atlas
arch=("x86_64")
makedepends=("go")

license=("Apache-2.0")
provides=('atlas')
conflicts=('atlas')
url="https://github.com/ariga/${binary}"

source_x86_64=("https://release.ariga.io/atlas/${binary}-community-linux-amd64-v${pkgver}")

sha256sums_x86_64=('78eb214e6dec245ae3d2de6153c46f1083a67ef8f537e8835557e55146899265')
b2sums_x86_64=('369931eff8c34a7fb54cada4b3b811fa5b435ed65a2d26b7dabcb501b7fc46c887a2b7fe3f1492e175f9a0d4f474ae355f09e6f6203d0e54531d0951c6fe7f08')

package() {
    install -Dm755 "${srcdir}/${binary}-community-linux-amd64-v${pkgver}" "${pkgdir}/usr/bin/${binary}"
}