# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Shuihuo
pkgname=jywjl
pkgver=1.0.0
pkgrel=2
pkgdesc="局域网精灵的 Linux 客户端"
arch=('x86_64')
url="https://jywjl.github.io/"
license=('Proprietary')
depends=('gtk2')
source=("https://github.com/jywjl/binaries/releases/download/v1.0/jywjl-linux_x86_64-latest.tar.bz2"
	"https://github.com/jywjl/jywjl.github.io/raw/master/icons/transparent.png")
noextract=()
sha512sums=("9a91d87c48a480b049e19a9707aa70f9a10d890daa94ba95c7f16931183cc47f926654b57b411b0c81162aa859d6700bd724bc8c467745c236a6c9951d844962"
		"77cae7a6b60e0b33910413059f49fb21f25f0f762724a0637b5f0ad2de04064f7b0d8a1cb06e81fb0c29035aa544609995ba19fe16b2e48144b000a08529b50b")

package() {
#tar xf jywjl-linux_x86_64-latest.tar.bz2
	mkdir -p "${pkgdir}/usr/bin/"
	cp jywjl/jywjl "${pkgdir}/usr/bin/jywjl"
	mkdir -p "${pkgdir}/usr/share/pixmaps/"
	cp transparent.png "${pkgdir}/usr/share/pixmaps/jywjl.png" 
	mkdir -p "${pkgdir}/usr/share/applications/"
	echo "[Desktop Entry] 
Name=局域网精灵
GenericName=局域网精灵
Comment=局域网精灵客户端
Exec=jywjl
Icon=/usr/share/pixmaps/jywjl.png
Terminal=false
Type=Application
Categories=Network;
StartupNotify=true" > "${pkgdir}/usr/share/applications/jywjl.desktop"
}
