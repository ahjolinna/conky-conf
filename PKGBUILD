# Maintainer: ahjolinna <@yahoo.com>

pkgname=ahjolinna-conky-conf
pkgver=0.3
pkgrel=1
pkgdesc="this is my personal conky conf"
url='https://github.com/ahjolinna/conky-conf'
screenshot=('http://i.imgur.com/JGFrAQQ.png')
arch=('any')
license=('GPLv2')
depends=('conky' 'vnstat' 'otf-source-sans-pro' 'lm_sensors' 'libatasmart' 'wget' 'dmidecode')
optdepends=('spotify: For the music you love. Or else no widget'
    'dropbox')
provides=('conky-conf')
options=(!strip !emptydirs)
source=('chakra-logo.png' 'conky.conf' 'cover.txt' 'dropbox.py' 'last_album_pic.png' 'conky-conf.install' 'spotify-cover.sh')
install=conky-conf.install

sha256sums=('947e71ea0ee8d2400a627fae8279a7959ebbcbc7747696aeaf78d225a95f868b'
            '3ece93208712746ee2e750571e3ebcc9e5558a6d4d6e536d3435f6a03be511f8'
            '0c2fbf2a5ea2f9899b9affe4855ec081d7bb3484d02b1a887573ce5b376b9f26'
            '23732bac8f363b9573fc9cd8d83593f3396773f1340e3bff0bcfa68e41991a22'
            'c3c1183ce3958d79b78134de2404288c3415e69f36f5f77c238f04a1f0299914'
            'fe5d990cea5e256cc30940bb4f05e54aade7ff66eedd6aff35ae4949e0710db9'
            '73e6a8fd93c30095c0d7e6105c374d980809457419e4230e924c0e717bb69c6d')
user_name="$(logname)"
package() {
    
        mkdir -p $pkgdir/home/${user_name}/.config/conky/
        chown -R ${user_name}:users $pkgdir/home/${user_name}/.config/conky/

 cp -r $srcdir/* ${pkgdir}/home/${user_name}/.config/conky/

}


