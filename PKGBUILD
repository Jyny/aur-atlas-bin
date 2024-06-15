# Maintainer: Jerry Y. Chen <chen@jyny.dev>

pkgname=atlas-bin
pkgdesc="A modern tool for managing database schemas"
pkgver=0.24.0
pkgrel=2
binary=atlas
arch=("x86_64")
makedepends=("go")

license=("Apache-2.0")
provides=('atlas')
conflicts=('atlas')
url="https://github.com/ariga/${binary}"

source_x86_64=("https://release.ariga.io/atlas/${binary}-community-linux-amd64-v${pkgver}")

sha256sums_x86_64=('29c3430947656d492203e0368de92a3fab2ab5c32e43087d1c443668f5f5c0b1')
b2sums_x86_64=('6d31f1759d9d7421cbd1145507c12bff6e6e70d8e3624deeb54a6149dc25390a1604e1dba9750d7722d422c3f35292d853e349d2c911ab13d173be1a3fe45b4f')

package() {
    install -Dm755 "${srcdir}/${binary}-community-linux-amd64-v${pkgver}" "${pkgdir}/usr/bin/${binary}"
}