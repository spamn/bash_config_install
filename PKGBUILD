# Maintainer: <github@fleuryn.fr>
pkgname=bash_config
pkgver=0.0.2.r0.ge119177
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
    cd "${srcdir}/${pkgname}"
    printf "%s" "$(git describe --long --tags | sed 's/\([^-]*-g\)/r\1/;s/-/./g')" 
}

build() {
    :
}

package() {
	cd $pkgname
	make DESTDIR="$pkgdir/" install
}

