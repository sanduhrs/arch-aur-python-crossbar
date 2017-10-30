# Maintainer: Florijan Hamzic <fh@infinicode.de>

pkgname=python-crossbar
pkgver=17.5.1
pkgrel=1
pkgdesc="Crossbar.io - WAMP application router http://crossbar.io/"
arch=('any')
url="https://github.com/crossbario/crossbar"
license=('AGPL')
depends=('python>=3.1')
provides=("${_pkgname}")
conflicts=("${_pkgname}")
source=(https://github.com/crossbario/crossbar/archive/v${pkgver}.tar.gz)
sha1sums=('5dbd0478883203b8672f8f37615d450529f36015')

package(){
    cd "${srcdir}/crossbar-${pkgver}"
    python setup.py install --root="$pkgdir" --prefix=/usr
    install -D -m644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
