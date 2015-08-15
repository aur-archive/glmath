# Peter Hatina <phatina AT gmail.com>
pkgname=glmath
pkgver=0.9.3.1
pkgrel=1
pkgdesc="C++ mathematics library for 3D software based on the OpenGL Shading Language (GLSL) specification."
arch=('i686' 'x86_64')
license=('GPL')
sources=("glm-$pkgver.zip")
source=("http://sourceforge.net/projects/ogl-math/files/glm-$pkgver/glm-$pkgver.zip")
url="http://glm.g-truc.net"
md5sums=('b03e518c3d741f6c1dffd8c14319451b')

package() {
    mkdir -p $pkgdir/usr/include/glm
    cp -r $srcdir/glm $pkgdir/usr/include
    rm -f $pkgdir/usr/include/glm/CMakeLists.txt
    find $pkgdir -type f -exec chmod 644 {} \;
    find $pkgdir -type d -exec chmod 755 {} \;
}
