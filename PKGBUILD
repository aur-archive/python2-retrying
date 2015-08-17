# Maintainer: David J. Haines <djhaines at gmx dot com>

_pkgname=retrying
pkgname=python2-${_pkgname}
pkgver=1.2.3
pkgrel=1
pkgdesc="A general purpose Python retyring library"
url="https://github.com/rholder/${_pkgname}"
depends=('python2' )
makedepends=('python2' )
conflicts=("${pkgname}-git")
license=('APACHE')
arch=('any')
source=("https://github.com/rholder/${_pkgname}/archive/v${pkgver}.tar.gz")
md5sums=('722ae7303db80df20c53fb2fb3bcc68b')

build() {
	cd ${_pkgname}-${pkgver}
    python2 setup.py build
}

package() {
	cd ${_pkgname}-${pkgver}
    python2 setup.py install --root="$pkgdir" --optimize=1 
}
