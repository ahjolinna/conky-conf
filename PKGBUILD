# Maintainer: ahjolinna <@yahoo.com>

pkgname=ahjolinna-conky-conf
pkgver=1.0
pkgrel=1
pkgdesc="this is my personal conky conf"
screenshot=('http://i.imgur.com/JGFrAQQ.png')
arch=('any')
license=('GPLv2')
depends=('conky' 'vnstat' 'otf-source-sans-pro' 'lm_sensors' 'libatasmart')
optdepends=('spotify: For the music you love. Or else no widget'
    'dropbox')
provides=('conky-conf')
options=(!strip !emptydirs)
source=('chakra-logo.png'  'conky.conf'  'cover.txt'  'dropbox.py' 'last_album_pic.png'  'spotify-cover.sh'
)
sha256sums=('947e71ea0ee8d2400a627fae8279a7959ebbcbc7747696aeaf78d225a95f868b'
            '9620b0fcb5b67cab1ebbef0fc11b73a988c905f563cd8e7c2dd799e6de1319d2'
            '0c2fbf2a5ea2f9899b9affe4855ec081d7bb3484d02b1a887573ce5b376b9f26'
            '23732bac8f363b9573fc9cd8d83593f3396773f1340e3bff0bcfa68e41991a22'
            'c3c1183ce3958d79b78134de2404288c3415e69f36f5f77c238f04a1f0299914'
            '1e4c246fafa613a52108248ce17d9dc7aae629af3bbc7e11b418ae44079c9e5b')
user_name="$(logname)"
package() {
    
        mkdir -p $pkgdir/home/${user_name}/.config/conky/
        chown -R ${user_name}:users $pkgdir/home/${user_name}/.config/conky/

 cp -r $srcdir/* ${pkgdir}/home/${user_name}/.config/conky/

}


