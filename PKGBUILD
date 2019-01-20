# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Shuihuo
pkgname=jywjl
pkgver=2.0.0
pkgrel=1
pkgdesc="局域网精灵的 Linux 客户端"
arch=('x86_64')
url="https://jywjl.github.io/"
license=('Proprietary')
depends=('webkitgtk2')
source=("http://files.git.oschina.net/group1/M00/06/51/PaAvDFxBK-KAf_QhAExNPrRCK1o231.bz2?token=6be8eecec4d19209234cc4d64a0d469f&ts=1547777013&attname=jywjl_v2.0.0.tar.bz2"
	"https://github.com/jywjl/jywjl.github.io/raw/master/icons/transparent.png")
noextract=()
sha512sums=("0fbfee5a4a07fa1c292660d88a16412587df47a41c9fd061ae3971dbeaaf37790995e86ca8ce1824d29707f67592c3e6a68ee46ce4c9cc857072f91a8a8a2337"
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
