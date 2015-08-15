#Maintainer: Jesse Jaara <jesse.jaara@gmail.com>

pkgname=eris
pkgver=1.3.21
pkgrel=1
pkgdesc="Provides a common system to deal with the back-end Atlas tasks."
arch=(i686 x86_64)
url="http://worldforge.org/dev/eng/libraries/eris"
license=('LGPL')
depends=('atlas_cpp' 'mercator' 'skstream' 'libsigc++2.0')
options=(!libtool)
source=("http://downloads.sourceforge.net/sourceforge/worldforge/$pkgname-$pkgver.tar.bz2")

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  ./configure --prefix=/usr
  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"

  make DESTDIR="${pkgdir}" install
}

md5sums=('bc3e81d6fd93f9c0483efbca2ebdab90')
