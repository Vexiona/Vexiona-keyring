# Maintainer: Vexiona <88843406+Vexiona@users.noreply.github.com>

pkgname=Vexiona-keyring
pkgver=20231221
pkgrel=3
pkgdesc="Vexiona's arch repo PGP keyring"
arch=('any')
url='https://github.com/Vexiona/archrepo'
license=('GPL3')
install=$pkgname.install
source=(Vexiona{.gpg,-{revoked,trusted}})
sha256sums=(
  '6c067d56cdd2f823c28d99b164888a5b52f55f7ad4f9254e987dfdf0e67faebc'
  '7eb70257593da06f682a3ddda54a9d260d4fc514f645237f5ca74b08f8da61a6'
  'bfac8931882fca826d646f52e3c1a49599b7683b18f3930c742bcdb601708aaa'
)

package() {
  install -D --mode 0644 \
    --target-directory "${pkgdir}"/usr/share/pacman/keyrings/ \
    Vexiona{.gpg,-{revoked,trusted}} 
}
