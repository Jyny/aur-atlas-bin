# Maintainer: Jerry Y. Chen <chen@jyny.dev>

pkgname=atlas-bin
pkgdesc="A modern tool for managing database schemas"
pkgver=0.23.0
pkgrel=2
binary=atlas
arch=("x86_64")
makedepends=("go")

license=("Apache-2.0")
provides=('atlas')
conflicts=('atlas')
url="https://github.com/ariga/${binary}"

source_x86_64=("https://release.ariga.io/atlas/${binary}-community-linux-amd64-v${pkgver}")

sha256sums_x86_64=('a196e447445611573ab302a3180e87a5f8b2698d07da0f19d29ab90c6f6a76ae')
b2sums_x86_64=('ab961b76c6e6056d052d9b3b0ea05b1dcf14785070a1ab8f14bbbb4bed9791cf3f35dbad298808a7e873bf92e42233d0109550f50a6dee9056e20f070e60b63b')

package() {
    install -Dm755 "${srcdir}/${binary}-community-linux-amd64-v${pkgver}" "${pkgdir}/usr/bin/${binary}"
}