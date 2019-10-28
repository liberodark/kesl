# Maintainer: liberodark

pkgname=kesl
pkgver=10.1.1
pkgrel=6421
pkgdesc="Kaspersky Endpoint Security Linux"
arch=('x86_64')
url="https://www.kaspersky.fr/small-to-medium-business-security/endpoint-linux"
license=('Proprietary')
depends=('xdg-utils' 'which' 'perl')
source_x86_64=("https://products.s.kaspersky-labs.com/endpoints/keslinux10/${pkgver}.${pkgrel}/multilanguage-${pkgver}.${pkgrel}/babce9ef/kesl_${pkgver}-${pkgrel}_amd64.deb")
#source=($pkgname.desktop
#        $pkgname.png)
#sha512sums=('c7fd2848a7881f42e703614132751c2a9a754004064904573b67816c174d1b1b6287378f72f2fbdeaa67df4a787978fa9c373b642a12eaac9e30a51cd70a2877'
#         '798bab296302facf5597a71d2f038de89417c0e99c63d891e6f03cafa1758bb993c762942b29b8f1caf3787d0553d15deb612f7a756ea6faef4e2348f08230e2')
sha512sums_x86_64=('b50fb626523fa3f06cc809279b960db682c9eee89c9cd55d8fe9eb318f8d25e2c039259554871ec25f44946bc7c09609dadf50967792755dfabd4352c8e6f5c9')
        
package() {
  cd $srcdir
  tar xvf data.tar.xz
  cp -r var/opt/kaspersky/kesl/install/ $pkgdir
  #install -vDm644 $srcdir/$pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
  #install -vDm644 $srcdir/$pkgname.png $pkgdir/usr/share/pixmaps/$pkgname.png
}
