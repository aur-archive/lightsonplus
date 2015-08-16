# Maintainer: klenamenis <klenamenis@posteo.org>

pkgname=lightsonplus
pkgver=20150221
pkgrel=1
pkgdesc="Bash script that prevents the screensaver and display power management (DPMS) to be activated when you are watching Videos fullscreen on Firefox and Chromium (Fork of github.com/iye/lightsOn)"
arch=(any)
url=https://github.com/devkral/lightsonplus
license=(GPL2)
depends=(bash xorg-xvinfo xorg-xprop)
source=($pkgname::https://raw.githubusercontent.com/devkral/$pkgname/master/lightson+.sh
	$pkgname-cmd::https://raw.githubusercontent.com/devkral/$pkgname/master/lightson+cmd.sh)
md5sums=('c51f084518f73ca73f98fa6511033c9c'
         'aa64124ca62f9b96201292522f4bc51b')
pkgver() {
	date +%Y%m%d
}

package() {
	install -Dm755 $srcdir/$pkgname $pkgdir/usr/bin/$pkgname
	install -Dm755 $srcdir/$pkgname-cmd $pkgdir/usr/bin/$pkgname-cmd
}
