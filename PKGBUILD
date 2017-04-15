# Maintainer: Simon Brakhane <simon@aur.brakhane.net>

pkgname=certbot-systemd
pkgver=0.2.2
pkgrel=1
pkgdesc='Systemd scripts for certbot (letsencrypt) renewals'
license=('GPL3')
source=("git+https://github.com/luminger/certbot-systemd#tag=$pkgver")
sha512sums=('SKIP')
arch=('any')
depends=('certbot' 'systemd')
backup=('etc/certbot-users')


package() {
        install -Dm644 "$srcdir/$pkgname/certbot.service" "$pkgdir/usr/lib/systemd/system/certbot.service"
        install -Dm644 "$srcdir/$pkgname/certbot.timer" "$pkgdir/usr/lib/systemd/system/certbot.timer"
	install -Dm644 "$srcdir/$pkgname/certbot-users" "$pkgdir/etc/certbot-users"
}
