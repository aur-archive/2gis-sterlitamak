pkgname=2gis-sterlitamak
pkgver=7
pkgrel=1
pkgdesc="Map of Sterlitamak for 2GIS, June 2012"
arch=('i686' 'x86_64')
url="http://sterlitamak.2gis.ru/how-get/linux/"
license=('custom')
depends=('2gis>=3.6.0.2')
source=("http://download.2gis.ru/arhives/2GISData_Sterlitamak-7.orig.zip")
md5sums=('b8859a095d9fb0dcf13b2efc0c645eff')

build() {
  cd $startdir
# Installing to /opt/2gis
  install -D -m 644 ${startdir}/src/2gis/3.0/Data_Sterlitamak.dgdat "${startdir}/pkg/opt/2gis/sterlitamak.dgdat" || return 1
  install -D -m 644 ${startdir}/src/2gis/3.0/Plugins/DGisLan/Sterlitamak.dglf "${startdir}/pkg/opt/2gis/Plugins/DGisLan/Sterlitamak.dglf" || return 1
}
