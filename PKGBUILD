pkgname=libchardet
pkgver=1.0.4
pkgrel=1
pkgdesc="Mozilla's Universal Charset Detector C/C++ API"
arch=('x86_64')
license=('MPL')
url="http://ftp.oops.org/pub/oops/libchardet"
depends=('gcc-libs' 'bash')
options=('!libtool')
source=("ftp://ftp.oops.org/pub/oops/$pkgname/${pkgname}-${pkgver}.tar.bz2")
md5sums=('93edadd9353325405d6e092127339f33')

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"
  
    ./configure --prefix=/usr 
  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"
  
  make DESTDIR="${pkgdir}" install

}