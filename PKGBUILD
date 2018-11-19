# Maintainer: Daniel Hillenbrand <codeworkx [at] bbqlinux [dot] org>

pkgname=android-host-tools
pkgver=9.0.0
pkgrel=1
pkgdesc="Android Host Tools"
arch=('any')
provides=('dtbToolCM' 'fastboot' 'img2sdat' 'minigzip' 'mkbootfs' 'mkbootimg' 'mkyaffs2image' 'sdat2img' 'unpackbootimg' 'update_payload_extract' 'zipalign')
url="https://github.com/bbqlinux/android-host-tools"
license=('APACHE2')
depends=('libc++' 'python2-protobuf' 'python2-backports.lzma')

package() {
    mkdir -p "$pkgdir/opt" "$pkgdir/usr/bin" "$pkgdir/opt/android-host-tools/bin/python"
    
    cd "$pkgdir"

    # Install executables
    install -Dm755 "$srcdir/opt/android-host-tools/bin/dtbToolCM" opt/android-host-tools/bin/dtbToolCM
    install -Dm755 "$srcdir/opt/android-host-tools/bin/fastboot" opt/android-host-tools/bin/fastboot
    # https://github.com/xpirt/img2sdat
    install -Dm755 "$srcdir/opt/android-host-tools/bin/img2sdat" opt/android-host-tools/bin/img2sdat
    install -Dm755 "$srcdir/opt/android-host-tools/bin/minigzip" opt/android-host-tools/bin/minigzip
    install -Dm755 "$srcdir/opt/android-host-tools/bin/mkbootfs" opt/android-host-tools/bin/mkbootfs
    install -Dm755 "$srcdir/opt/android-host-tools/bin/mkbootimg" opt/android-host-tools/bin/mkbootimg
    install -Dm755 "$srcdir/opt/android-host-tools/bin/mkyaffs2image" opt/android-host-tools/bin/mkyaffs2image
    # https://github.com/xpirt/sdat2img
    install -Dm755 "$srcdir/opt/android-host-tools/bin/sdat2img" opt/android-host-tools/bin/sdat2img
    install -Dm755 "$srcdir/opt/android-host-tools/bin/unpackbootimg" opt/android-host-tools/bin/unpackbootimg
    # https://github.com/gmrt/update_payload_extractor
    install -Dm755 "$srcdir/opt/android-host-tools/bin/update_payload_extract" opt/android-host-tools/bin/update_payload_extract
    install -Dm755 "$srcdir/opt/android-host-tools/bin/zipalign" opt/android-host-tools/bin/zipalign

    # Create symlinks
    ln -s "/opt/android-host-tools/bin/dtbToolCM" "$pkgdir/usr/bin/dtbToolCM"
    ln -s "/opt/android-host-tools/bin/fastboot" "$pkgdir/usr/bin/fastboot"
    ln -s "/opt/android-host-tools/bin/img2sdat" "$pkgdir/usr/bin/img2sdat"
    ln -s "/opt/android-host-tools/bin/minigzip" "$pkgdir/usr/bin/minigzip"
    ln -s "/opt/android-host-tools/bin/mkbootfs" "$pkgdir/usr/bin/mkbootfs"
    ln -s "/opt/android-host-tools/bin/mkbootimg" "$pkgdir/usr/bin/mkbootimg"
    ln -s "/opt/android-host-tools/bin/mkyaffs2image" "$pkgdir/usr/bin/mkyaffs2image"
    ln -s "/opt/android-host-tools/bin/sdat2img" "$pkgdir/usr/bin/sdat2img"
    ln -s "/opt/android-host-tools/bin/unpackbootimg" "$pkgdir/usr/bin/unpackbootimg"
    ln -s "/opt/android-host-tools/bin/update_payload_extract" "$pkgdir/usr/bin/update_payload_extract"
    ln -s "/opt/android-host-tools/bin/zipalign" "$pkgdir/usr/bin/zipalign"
    
    # Copy deps
    cp -R "$srcdir/opt/android-host-tools/bin/python" opt/android-host-tools/bin
}
