_realname=bazel

pkgbase=mingw-w64-${_realname}
pkgname="${MINGW_PACKAGE_PREFIX}-${_realname}"
pkgver=0.17.2
pkgrel=1
pkgdesc="A fast, scalable, multi-language and extensible build system"

license=('Apache License 2.0')
url="https://bazel.build/"
source=(https://github.com/bazelbuild/bazel/releases/download/${pkgver}/${_realname}-${pkgver}-dist.zip)
sha256sums=('b6e87acfa0a405bb8b3417c58477b66d5bc27dc0d31ba6fa12bc255b9278d33b')

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
