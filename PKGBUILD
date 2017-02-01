pkgname=libchardet
pkgver=1.0.5
pkgrel=1
pkgdesc="Mozilla's Universal Charset Detector C/C++ API"
arch=('x86_64')
license=('MPL')
url="http://ftp.oops.org/pub/oops/libchardet"
depends=('gcc-libs' 'bash')
options=('!libtool')
source=("https://github.com/Joungkyun/libchardet/archive/$pkgver.tar.gz")
md5sums=('218efba7ae9789202d40fe8133311729')

build() {
  cd "${srcdir}/${pkgname}-${pkgver}"
    ./configure --prefix=/usr 
  make
}

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"
  
  make DESTDIR="${pkgdir}" install

}
