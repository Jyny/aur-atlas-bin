# Maintainer: Jerry Y. Chen <chen@jyny.dev>

pkgname=atlas-bin
pkgdesc="A modern tool for managing database schemas"
pkgver=0.22.0
pkgrel=2
binary=atlas
arch=("x86_64")
makedepends=("go")

license=("Apache-2.0")
provides=('atlas')
conflicts=('atlas')
url="https://github.com/ariga/${binary}"

source_x86_64=("https://release.ariga.io/atlas/${binary}-community-linux-amd64-v${pkgver}")

sha256sums_x86_64=('b6be8d0608c215698e52d7be6de77d29602bc51eb015c7e322d01bbcaf46e119')
b2sums_x86_64=('709049fdd23a78bb49700fece97bc686ca6b55919fcf89285cc328aa676e6c154ad53068e5bea83e6f74b70660d5915f4f4555c710f9d632619025f816fc8a10')

package() {
    install -Dm755 "${srcdir}/${binary}-community-linux-amd64-v${pkgver}" "${pkgdir}/usr/bin/${binary}"
}