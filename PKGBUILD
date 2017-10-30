# Maintainer: Florijan Hamzic <fh@infinicode.de>

pkgname=python-crossbar
pkgver=17.6.1
pkgrel=1
pkgdesc="Crossbar.io - WAMP application router http://crossbar.io/"
arch=('any')
url="https://github.com/crossbario/crossbar"
license=('AGPL')
depends=('python>=3.1')
provides=("${_pkgname}")
conflicts=("${_pkgname}")
source=(https://github.com/crossbario/crossbar/archive/v${pkgver}.tar.gz)
sha1sums=('38f8784f478a24b345b419682835a531b206ae2a')

package(){
    cd "${srcdir}/crossbar-${pkgver}"
    python setup.py install --root="$pkgdir" --prefix=/usr
    install -D -m644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
