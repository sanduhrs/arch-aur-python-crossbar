# Maintainer: Florijan Hamzic <fh@infinicode.de>

pkgname=python-crossbar
pkgver=17.9.2
pkgrel=1
pkgdesc="Crossbar.io - WAMP application router http://crossbar.io/"
arch=('any')
url="https://github.com/crossbario/crossbar"
license=('AGPL')
depends=('python>=3.1')
provides=("${_pkgname}")
conflicts=("${_pkgname}")
source=(https://github.com/crossbario/crossbar/archive/v${pkgver}.tar.gz)
sha1sums=('c92f6b92853ba6d840ea0768b4d3752ddc71c9a9')

package(){
    cd "${srcdir}/crossbar-${pkgver}"
    python setup.py install --root="$pkgdir" --prefix=/usr
    install -D -m644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
