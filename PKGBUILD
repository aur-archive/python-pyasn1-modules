# Maintainer: Thomas Jost <schnouki@schnouki.net>
pkgname=python-pyasn1-modules
pkgver=0.0.5
pkgrel=2
pkgdesc="A collection of protocols modules written in ASN.1 language"
arch=('any')
url="http://pypi.python.org/pypi/pyasn1-modules/"
license=('BSD')
makedepends=('python-setuptools')
depends=('python-pyasn1')
source=(http://pypi.python.org/packages/source/p/pyasn1-modules/pyasn1-modules-${pkgver}.tar.gz)
md5sums=('6c5c9dd61a5784ff22695ac233cb11f8')
sha1sums=('108bdef1b3ca7050ff93c59e7ef7225c9c1a8b07')

package() {
  cd "${srcdir}/pyasn1-modules-${pkgver}"
  python setup.py install --root="${pkgdir}"
  install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
