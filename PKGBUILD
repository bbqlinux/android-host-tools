# Maintainer: Daniel Hillenbrand <codeworkx@bbqlinux.org>

pkgname=android-host-tools
pkgver=4.2.2
pkgrel=1
pkgdesc="Android Host Tools"
arch=('any')
url="https://github.com/bbqlinux/android-host-tools"
license=('APACHE2')

package() {
    cd "$pkgdir"

    install -Dm755 "$srcdir/usr/bin/fastboot" usr/bin/fastboot
    install -Dm755 "$srcdir/usr/bin/img2simg" usr/bin/img2simg
    install -Dm755 "$srcdir/usr/bin/minigzip" usr/bin/minigzip
    install -Dm755 "$srcdir/usr/bin/mkbootfs" usr/bin/mkbootfs
    install -Dm755 "$srcdir/usr/bin/mkbootimg" usr/bin/mkbootimg
    install -Dm755 "$srcdir/usr/bin/mkimage" usr/bin/mkimage
    install -Dm755 "$srcdir/usr/bin/mksdcard" usr/bin/mksdcard
    install -Dm755 "$srcdir/usr/bin/mkyaffs2image" usr/bin/mkyaffs2image
    install -Dm755 "$srcdir/usr/bin/simg2img" usr/bin/simg2img
    install -Dm755 "$srcdir/usr/bin/simg2simg" usr/bin/simg2simg
    install -Dm755 "$srcdir/usr/bin/unpackbootimg" usr/bin/unpackbootimg
    install -Dm755 "$srcdir/usr/bin/unyaffs" usr/bin/unyaffs
    install -Dm755 "$srcdir/usr/bin/zipalign" usr/bin/zipalign

}
