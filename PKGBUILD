# Maintainer: Flavio Heleno <flaviohbatista@gmail.com>

pkgname='tkn-bin'
pkgver=0.37.0
pkgrel=1
pkgdesc='A CLI for interacting with Tekton!'
url='https://github.com/tektoncd/cli'
arch=('aarch64' 'ppc64le' 's390x' 'x86_64')
license=('Apache 2.0')
provides=('tkn')

sha256sums_aarch64=('9bc6e2aa07012c843bfaaf68b8d536f7d23a110f1ffa09dee5a12057f8712360')
sha256sums_ppc64le=('676a542c9766a772445f132eb017df8533f23b3fb9e7af5c12f5239a44a5c984')
sha256sums_s390x=('63504d50c2c6eb538aa5495111efd63946fc7e3df841f03e45a51d75ed71a51a')
sha256sums_x86_64=('3430878665d3c1026d510d9daf6e26fe72454da9ca2cdc34bd7c5fca75c3322f')

source_aarch64=("${pkgname}_${pkgver}_aarch64::https://github.com/tektoncd/cli/releases/download/v${pkgver}/tkn_${pkgver}_Linux_aarch64.tar.gz")
source_ppc64le=("${pkgname}_${pkgver}_ppc64le::https://github.com/tektoncd/cli/releases/download/v${pkgver}/tkn_${pkgver}_Linux_ppc64le.tar.gz")
source_s390x=("${pkgname}_${pkgver}_s390x::https://github.com/tektoncd/cli/releases/download/v${pkgver}/tkn_${pkgver}_Linux_s390x.tar.gz")
source_x86_64=("${pkgname}_${pkgver}_x86_64.tar.gz::https://github.com/tektoncd/cli/releases/download/v${pkgver}/tkn_${pkgver}_Linux_x86_64.tar.gz")

package() {
  install -Dm755 "./tkn" "${pkgdir}/usr/bin/tkn"

  install -Dm644 "./LICENSE" "${pkgdir}/usr/share/licenses/tkn/LICENSE"
}
