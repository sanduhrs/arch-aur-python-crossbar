# Maintainer: Florijan Hamzic <fh@infinicode.de>

pkgname=python-crossbar
pkgver=17.8.1
pkgrel=1
pkgdesc="Crossbar.io - WAMP application router http://crossbar.io/"
arch=('any')
url="https://github.com/crossbario/crossbar"
license=('AGPL')
depends=('python>=3.1')
provides=("${_pkgname}")
conflicts=("${_pkgname}")
source=(https://github.com/crossbario/crossbar/archive/v${pkgver}.tar.gz)
sha1sums=('d8ec801444ab769c9fd33c54d9f9fd1acd04d6e3')

package(){
    cd "${srcdir}/crossbar-${pkgver}"
    python setup.py install --root="$pkgdir" --prefix=/usr
    install -D -m644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
