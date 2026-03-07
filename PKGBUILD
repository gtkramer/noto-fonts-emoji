# Maintainer: Antonio Rojas <arojas@archlinux.org>

pkgbase=noto-fonts-emoji
pkgname=(ttf-noto-fonts-emoji)
pkgver=2.051
pkgrel=2
epoch=1
pkgdesc='Google Noto Emoji font'
arch=(any)
url='https://fonts.google.com/noto'
license=(OFL-1.1)
provides=(emoji-font)
source=("https://github.com/googlefonts/noto-emoji/archive/refs/tags/v${pkgver}.zip")
b2sums=('52e27896626703b2bff43dcf85aab91e8e9ab71dd1bc940abe19bbebc0f026fae610681221200abeffd55351ea4cc019295815435f224577bf784d074efadc8c')

package_ttf-noto-fonts-emoji() {
  provides+=(noto-fonts-emoji)
  conflicts=(noto-fonts-emoji)
  replaces=(noto-fonts-emoji)

  cd "${srcdir}/noto-emoji-${pkgver}/fonts"
  install -Dm644 NotoColorEmoji.ttf "${pkgdir}/usr/share/fonts/${pkgbase//-fonts/}"
  install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/${pkgname}"
}
