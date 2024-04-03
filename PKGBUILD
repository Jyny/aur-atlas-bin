# Maintainer: Jerry Y. Chen <chen@jyny.dev>

pkgname=atlas-bin
pkgdesc="A modern tool for managing database schemas"
pkgver=0.21.0
pkgrel=1
binary=atlas
arch=("x86_64")
makedepends=("go")

license=("Apache-2.0")
provides=('atlas')
conflicts=('atlas')
url="https://github.com/ariga/${binary}"

source_x86_64=("https://release.ariga.io/atlas/${binary}-community-linux-amd64-v${pkgver}")

sha256sums_x86_64=('63dcef42a407c8d0a998f8215a68a61cc0bc0b528a016ecbd39aa68323c32816')
b2sums_x86_64=('3ce52193582d094903aa3890e1e7ac5b254f7404b0ccdb8d3ccc4d15b30437602e32af63e5fcd8ec6ce6ce81d38e3ab1561eff429058cacbdd50672673ac3d2a')

package() {
    install -Dm755 "${srcdir}/${binary}-community-linux-amd64-v${pkgver}" "${pkgdir}/usr/bin/${binary}"
}