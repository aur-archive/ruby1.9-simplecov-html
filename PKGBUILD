# Generated by gem2arch (https://github.com/anatol/gem2arch)
# Maintainer: Babken Vardanyan <483ken@gmail.com>

_gemname=simplecov-html
pkgname=ruby1.9-$_gemname
pkgver=0.5.3
pkgrel=1
pkgdesc='Default HTML formatter for SimpleCov code coverage tool for ruby 1.9+'
arch=(any)
url='https://github.com/colszowka/simplecov-html'
license=()
depends=(ruby1.9)
options=(!emptydirs)
source=(https://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
sha1sums=('b872cae77e0bf95f62b8d8886625727e327dcf65')

package() {
  local _gemdir="$(ruby-1.9 -e'puts Gem.default_dir')"
  gem-1.9 install --ignore-dependencies --no-user-install -i "$pkgdir/$_gemdir" $_gemname-$pkgver.gem
  rm "$pkgdir/$_gemdir/cache/$_gemname-$pkgver.gem"
  install -D -m644 "$pkgdir/$_gemdir/gems/$_gemname-$pkgver/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
