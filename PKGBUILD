# Maintainer: Daniel Hillenbrand <codeworkx@bbqlinux.org>

pkgname=android-host-tools
pkgver=4.3.0
pkgrel=1
pkgdesc="Android Host Tools"
arch=('any')
provides=('fastboot' 'img2simg' 'minigzip' 'mkbootfs' 'mkbootimg' 'mkimage' 'mksdcard' 'mkyaffs2image' 'simg2img' 'simg2simg' 'unpackbootimg' 'unyaffs' 'zipalign')
url="https://github.com/bbqlinux/android-host-tools"
license=('APACHE2')

package() {
    mkdir -p "$pkgdir/opt" "$pkgdir/usr/bin"
    
    cd "$pkgdir"

    install -Dm755 "$srcdir/opt/android-host-tools/bin/fastboot" opt/android-host-tools/bin/fastboot
    install -Dm755 "$srcdir/opt/android-host-tools/bin/img2simg" opt/android-host-tools/bin/img2simg
    install -Dm755 "$srcdir/opt/android-host-tools/bin/minigzip" opt/android-host-tools/bin/minigzip
    install -Dm755 "$srcdir/opt/android-host-tools/bin/mkbootfs" opt/android-host-tools/bin/mkbootfs
    install -Dm755 "$srcdir/opt/android-host-tools/bin/mkbootimg" opt/android-host-tools/bin/mkbootimg
    install -Dm755 "$srcdir/opt/android-host-tools/bin/mkimage" opt/android-host-tools/bin/mkimage
    install -Dm755 "$srcdir/opt/android-host-tools/bin/mksdcard" opt/android-host-tools/bin/mksdcard
    install -Dm755 "$srcdir/opt/android-host-tools/bin/mkyaffs2image" opt/android-host-tools/bin/mkyaffs2image
    install -Dm755 "$srcdir/opt/android-host-tools/bin/simg2img" opt/android-host-tools/bin/simg2img
    install -Dm755 "$srcdir/opt/android-host-tools/bin/simg2simg" opt/android-host-tools/bin/simg2simg
    install -Dm755 "$srcdir/opt/android-host-tools/bin/unpackbootimg" opt/android-host-tools/bin/unpackbootimg
    install -Dm755 "$srcdir/opt/android-host-tools/bin/unyaffs" opt/android-host-tools/bin/unyaffs
    install -Dm755 "$srcdir/opt/android-host-tools/bin/zipalign" opt/android-host-tools/bin/zipalign

    ln -s "/opt/android-host-tools/bin/fastboot" "$pkgdir/usr/bin/fastboot"
    ln -s "/opt/android-host-tools/bin/img2simg" "$pkgdir/usr/bin/img2simg"
    ln -s "/opt/android-host-tools/bin/minigzip" "$pkgdir/usr/bin/minigzip"
    ln -s "/opt/android-host-tools/bin/mkbootfs" "$pkgdir/usr/bin/mkbootfs"
    ln -s "/opt/android-host-tools/bin/mkbootimg" "$pkgdir/usr/bin/mkbootimg"
    ln -s "/opt/android-host-tools/bin/mkimage" "$pkgdir/usr/bin/mkimage"
    ln -s "/opt/android-host-tools/bin/mksdcard" "$pkgdir/usr/bin/mksdcard"
    ln -s "/opt/android-host-tools/bin/mkyaffs2image" "$pkgdir/usr/bin/mkyaffs2image"
    ln -s "/opt/android-host-tools/bin/simg2img" "$pkgdir/usr/bin/simg2img"
    ln -s "/opt/android-host-tools/bin/simg2simg" "$pkgdir/usr/bin/simg2simg"
    ln -s "/opt/android-host-tools/bin/unpackbootimg" "$pkgdir/usr/bin/unpackbootimg"
    ln -s "/opt/android-host-tools/bin/unyaffs" "$pkgdir/usr/bin/unyaffs"
    ln -s "/opt/android-host-tools/bin/zipalign" "$pkgdir/usr/bin/zipalign"
}
