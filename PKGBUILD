# Maintainer: Jerry Y. Chen <chen@jyny.dev>

pkgname=atlas-bin
pkgdesc="A modern tool for managing database schemas"
pkgver=0.27.0
pkgrel=1
binary=atlas
arch=("x86_64")
makedepends=("go")

license=("Apache-2.0")
provides=('atlas')
conflicts=('atlas')
url="https://github.com/ariga/${binary}"

source_x86_64=("https://release.ariga.io/atlas/${binary}-community-linux-amd64-v${pkgver}")

sha256sums_x86_64=('b7065a576b7b632b32553ffcaf5e54c7f6fd4ac2a5f84a10f5389cf588bde993')
b2sums_x86_64=('2b0ad3664f1aab5dd74d269dbc2dd720b85470ea7de0b52b443b74dee09268b54cabfb9aa22104f90ec8d1eb1715ea0b97f2ac86cc6307e3257c73a08c4486c1')

package() {
    install -Dm755 "${srcdir}/${binary}-community-linux-amd64-v${pkgver}" "${pkgdir}/usr/bin/${binary}"
}