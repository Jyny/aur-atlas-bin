# Maintainer: Jerry Y. Chen <chen@jyny.dev>

pkgname=atlas-bin
pkgdesc="A modern tool for managing database schemas"
pkgver=0.25.0
pkgrel=1
binary=atlas
arch=("x86_64")
makedepends=("go")

license=("Apache-2.0")
provides=('atlas')
conflicts=('atlas')
url="https://github.com/ariga/${binary}"

source_x86_64=("https://release.ariga.io/atlas/${binary}-community-linux-amd64-v${pkgver}")

sha256sums_x86_64=('c6070097bc39496470d55d42d9ae25f44e87f8d9a63c7309ef5f71c5b0496c62')
b2sums_x86_64=('f904e14d552d3049bb5bc568e86cf17ab01c4fb9a41973542bc040d618f95d61e3a21a50ae57a27401ffa2b760aeb4d049ea8d77b90476621b3ded5990dd07f4')

package() {
    install -Dm755 "${srcdir}/${binary}-community-linux-amd64-v${pkgver}" "${pkgdir}/usr/bin/${binary}"
}