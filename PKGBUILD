# Maintainer: Daniel Hillenbrand <codeworkx [at] bbqlinux [dot] org>

pkgname=android-host-tools
pkgver=7.1.2
pkgrel=2
pkgdesc="Android Host Tools"
arch=('any')
provides=('dtbToolCM' 'fastboot' 'minigzip' 'mkbootfs' 'mkbootimg' 'mkyaffs2image' 'unpackbootimg' 'zipalign')
url="https://github.com/bbqlinux/android-host-tools"
license=('APACHE2')
depends=('libc++')

package() {
    mkdir -p "$pkgdir/opt" "$pkgdir/usr/bin"
    
    cd "$pkgdir"
    
    install -Dm755 "$srcdir/opt/android-host-tools/bin/dtbToolCM" opt/android-host-tools/bin/dtbToolCM
    install -Dm755 "$srcdir/opt/android-host-tools/bin/fastboot" opt/android-host-tools/bin/fastboot
    install -Dm755 "$srcdir/opt/android-host-tools/bin/minigzip" opt/android-host-tools/bin/minigzip
    install -Dm755 "$srcdir/opt/android-host-tools/bin/mkbootfs" opt/android-host-tools/bin/mkbootfs
    install -Dm755 "$srcdir/opt/android-host-tools/bin/mkbootimg" opt/android-host-tools/bin/mkbootimg
    install -Dm755 "$srcdir/opt/android-host-tools/bin/mkyaffs2image" opt/android-host-tools/bin/mkyaffs2image
    install -Dm755 "$srcdir/opt/android-host-tools/bin/unpackbootimg" opt/android-host-tools/bin/unpackbootimg
    install -Dm755 "$srcdir/opt/android-host-tools/bin/zipalign" opt/android-host-tools/bin/zipalign

    ln -s "/opt/android-host-tools/bin/dtbToolCM" "$pkgdir/usr/bin/dtbToolCM"
    ln -s "/opt/android-host-tools/bin/fastboot" "$pkgdir/usr/bin/fastboot"
    ln -s "/opt/android-host-tools/bin/minigzip" "$pkgdir/usr/bin/minigzip"
    ln -s "/opt/android-host-tools/bin/mkbootfs" "$pkgdir/usr/bin/mkbootfs"
    ln -s "/opt/android-host-tools/bin/mkbootimg" "$pkgdir/usr/bin/mkbootimg"
    ln -s "/opt/android-host-tools/bin/mkyaffs2image" "$pkgdir/usr/bin/mkyaffs2image"
    ln -s "/opt/android-host-tools/bin/unpackbootimg" "$pkgdir/usr/bin/unpackbootimg"
    ln -s "/opt/android-host-tools/bin/zipalign" "$pkgdir/usr/bin/zipalign"
}
