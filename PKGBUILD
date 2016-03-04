# Maintainer: Faule Socke <github@socker.lepus.uberspace.de>

pkgname=mkinitcpio-multiencrypt
pkgver=1.1
pkgrel=1
pkgdesc="Allows to open multiple LUKS containers during boot (optionally using just a single passphrase)"
arch=(any)
url="https://github.com/faulesocke/mkinitcpio-multiencrypt"
license=('GPL')
depends=(mkinitcpio coreutils)
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=install
changelog=
source=("multiencrypt_hook"
        "multiencrypt_install"
        "LICENSE")
sha256sums=('105be328329e6352df601d64982d90d9cea7c8e7e630739bc69f42882c8523c6'
            '06609a990366c1074b4a694525aa1e741fdb452ee1f1c1aa0f8f5e2c3191c4de'
            'c03cea027b4b40e4402fabd08557736727ec3d5bc54ad64ab6472de432198cad')
validpgpkeys=()


package() {
    install -Dm644 multiencrypt_hook "$pkgdir/usr/lib/initcpio/hooks/multiencrypt"
    install -Dm644 multiencrypt_install "$pkgdir/usr/lib/initcpio/install/multiencrypt"
    install -Dm644 LICENSE "$pkgdir/usr/share/mkinitcpio-multiencrypt/LICENSE"
}
