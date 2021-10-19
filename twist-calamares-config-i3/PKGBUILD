# Maintainer: Erik Dubois <erik.dubois@gmail.com>
# Edited: PeterDauwe <bobo5290461@gmail.com>

_namepackage="${PWD##*/}"
pkgname=${_namepackage}
_destname1="/etc"
_destname2="/etc"
_destname3="/etc"
_destname4="/etc"
_date_mybuild="$(date +%y)_$(date +%m)_$(date +%d)"
_hour_mybuild="$(date +%H)$(date +%M)$(date +%S)"
pkgver=${_date_mybuild}
pkgrel=${_hour_mybuild}
pkgdesc=${_namepackage}
arch=('any')
url="https://github.com/PeterDauwe"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=()
replaces=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
}
