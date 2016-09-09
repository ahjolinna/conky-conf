# Maintainer: ahjolinna <@yahoo.com>

pkgname=ahjolinna-conky-conf
pkgver=0.3
pkgrel=3
pkgdesc="this is my personal conky conf"
url='https://github.com/ahjolinna/conky-conf'
screenshot=('http://i.imgur.com/aBcU2gW.jpg')
arch=('any')
license=('GPLv2')
depends=('conky' 'vnstat' 'otf-source-sans-pro' 'lm_sensors' 'wget')
optdepends=('spotify: For the music you love. Or else no widget'
    'dropbox')
makedepends=("git")
provides=('conky-conf')
options=(!strip !emptydirs)
source=('https://raw.githubusercontent.com/ahjolinna/conky-conf/master/conky.tar.gz')
install=conky-conf.install

sha256sums=('aaedf987c59018ac889459252835fb61dce96a313f97dc06a2bc5cf1f462651d')

user_name="$(logname)"
package() {
       mkdir -p $pkgdir/home/${user_name}/.config/conky/
       install -d  "${pkgdir}/home/${user_name}/.config/conky/" 
       cp -r $srcdir/conky/* "${pkgdir}/home/${user_name}/.config/conky/"
    chown -R ${user_name}:users $pkgdir/home/${user_name}/.config/conky/
}
