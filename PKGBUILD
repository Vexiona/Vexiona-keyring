# Maintainer: Guoxin "7Ji" Pu <pugokushin@gmail.com>

pkgname=7ji-keyring
pkgver=20231105
pkgrel=2
pkgdesc="7Ji's arch repo PGP keyring"
arch=('any')
url='https://github.com/7Ji/archrepo'
license=('GPL3')
install=$pkgname.install
source=(7Ji{.gpg,-{revoked,trusted}})
sha256sums=(
  '75827c7c280d5cdc4c333a187afddfb547e8486b7da0f74bbca3211545acf47d'
  'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'
  '771a132e7ca74f96047f79bbb4568ce80e6fbf7d82df71207e423bd4f9701d92'
)

package() {
  install -D --mode 0644 \
    --target-directory "${pkgdir}"/usr/share/pacman/keyrings/ \
    7Ji{.gpg,-{revoked,trusted}} 
}
