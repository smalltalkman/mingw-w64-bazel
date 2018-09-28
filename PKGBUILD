_realname=bazel

pkgbase=mingw-w64-${_realname}
pkgname="${MINGW_PACKAGE_PREFIX}-${_realname}"
pkgver=0.17.2
pkgrel=1
pkgdesc="A fast, scalable, multi-language and extensible build system"

license=('Apache License 2.0')
url="https://bazel.build/"
source=(https://github.com/bazelbuild/bazel/archive/${pkgver}.tar.gz)
sha256sums=('810AB0EF8F9976AD3CCC881F2B7EBD82736B8BDB8D5257B22768704C2F407EBC')

arch=('any')
depends=()
makedepends=()

build() {
  cd "${srcdir}/${_realname}-${pkgver}"
  exit
}

package() {
  cd "${srcdir}/${_realname}-${pkgver}"
  make DESTDIR="${pkgdir}/" install
}
