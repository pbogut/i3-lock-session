# Maintainer: Pawel Bogut <pbogut@pbogut.me>

pkgname=i3-lock-session
pkgver=0.1
pkgrel=1
epoch=1
pkgdesc="Start i3lock before starting i3 wm."
arch=('any')
url="https://github.com/pbogut/i3-lock-session"
license=('MIT')
depends=(
	'i3-wm'
	'i3lock'
)
optdepends=()
source=(i3-lock-session
        i3-lock.desktop
        i3-lock.xsession.desktop
        locktile.png)
sha512sums=('3495911cb70c11b4bf5affbeef5e6644a1feda24dee7ff938ff5eda4aa416b5f7616affd05e54678550f9a6a84587674e35a108665cd78c6793b425df61dd063'
            'e861d325c6f5437c5ad7c5f3e40b74a74e7d062ac13656c666f49dfed5fe54d991fef7d465b82e5bee66c99010317dbe16754ecff0bd4bd2ef00b4312d1ea439'
            'bb3ede91fc8807713866e5376f23df281b0c1bc6d1a1e40c9b32e8ba5f3cf64bd96e443a09019786e7437a997f9fb8a00e6193b58289a7ff3604abd31270be0e'
            '3299ba9edc5b48fcfddc07f91f5bba058c287395a19496683ac8711662bc8a3797cfba6ec3d67e9b921d10350f44b5975083ead1013909ae9ec5c1bf0ca638a4')


package() {
  install -m0644 -D i3-lock.xsession.desktop "$pkgdir"/usr/share/xsessions/i3-lock.desktop
  install -m0644 -D i3-lock.desktop "$pkgdir"/usr/share/applications/i3-lock.desktop
  install -m0755 -D i3-lock-session "$pkgdir"/usr/bin/i3-lock-session
  install -m0755 -D locktile.png "$pkgdir"/usr/share/i3-lock-session/locktile.png
}
