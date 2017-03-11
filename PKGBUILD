# Maintainer: <github@fleuryn.fr>
pkgname=bash_config
pkgver=0.0.1.r0.g13e73b1
pkgrel=1
pkgdesc="Config scripts for bash environment"
arch=('any')
url="https://github.com/spamn/$pkgname"
license=('WTFLP')
makedepends=('git' 'bash')
provides=("bash_config")
#backup TODO ?
backup=()
install=
source=( "git://github.com/spamn/${pkgname}.git")
md5sums=("SKIP")

pkgver() {
    cd "${srcdir}/bash_config"
    printf "%s" "$(git describe --long --tags | sed 's/\([^-]*-g\)/r\1/;s/-/./g')" 
}

build() {
    :
}

package() {
	cd $_gitname
	make DESTDIR="$pkgdir/" install
}

