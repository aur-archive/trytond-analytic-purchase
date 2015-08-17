# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-analytic-purchase
_pkgname=trytond_analytic_purchase
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The analytic_purchase module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-analytic-account>=3.4' 'trytond-analytic-invoice>=3.4' 'trytond-purchase>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("c2bb7b709377306e5f2bc2bb06b97918")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}