# Maintainer: Jerry Y. Chen <chen@jyny.dev>

pkgname=atlas-bin
pkgdesc="A modern tool for managing database schemas"
pkgver=0.22.0
pkgrel=1
binary=atlas
arch=("x86_64")
makedepends=("go")

license=("Apache-2.0")
provides=('atlas')
conflicts=('atlas')
url="https://github.com/ariga/${binary}"

source_x86_64=("https://release.ariga.io/atlas/${binary}-community-linux-amd64-v${pkgver}")

sha256sums_x86_64=('57eaf5ac62100372d33607e0f6e23c32fa1680ac102ebeacb19f415fce81e870')
b2sums_x86_64=('36012d0645beb8052a254a596517ecc45730bc17e81ae025e0b46121fc5e77c2812af84f6438d2ae7379a913f1ee6b3b1ef9464895f0fdc57c124f82afbde0f8')

package() {
    install -Dm755 "${srcdir}/${binary}-community-linux-amd64-v${pkgver}" "${pkgdir}/usr/bin/${binary}"
}