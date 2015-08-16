# Maintainer: Muflone http://www.muflone.com/contacts/english/

pkgname=jtopen
pkgver=8.2
pkgrel=1
pkgdesc="Open Source version of the IBM Toolbox for Java, a series of tools to easily access to IBM AS/400 and iSeries data and resources"
arch=(any)
url="http://jt400.sourceforge.net/"
license=('custom')
depends=(java-environment)
optdepends=()
provides=(jt400)
source=("http://downloads.sourceforge.net/project/jt400/JTOpen-full/${pkgver}/jtopen_${pkgver/\./_}.zip")
md5sums=('b37151e1bdcd06d00b4c59b40fcda933')

package() {
  # Install files for the package
  install -d "${pkgdir}/usr/lib/${pkgname}"
  install -m 644 -t "${pkgdir}/usr/lib/${pkgname}" lib/*.jar

  install -d "${pkgdir}/usr/share/licenses/${pkgname}"
  install -m 644 -t "${pkgdir}/usr/share/licenses/${pkgname}" license.html

  install -d "${pkgdir}/usr/share/doc/${pkgname}"
  install -m 644 -t "${pkgdir}/usr/share/doc/${pkgname}" changes.html
  install -m 644 -t "${pkgdir}/usr/share/doc/${pkgname}" readme.html
}

