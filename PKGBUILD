# Contributor: Jimmy Ricco van Turnhout <j.r.v.turnhout@student.tue.nl>

pkgname='tue-font-ttf'
pkgver=1
pkgrel=1
pkgdesc="Fonts used at Eindhoven University of Technology (TTF version)"
arch=('any')
url="http://pkgs.jrvturnhout.nl/tue-font-ttf/"
license=('unknown')
depends=('fontconfig' 'xorg-font-utils')
install='tue-font-ttf.install'
source=("http://pkgs.jrvturnhout.nl/tue-font-ttf/Telogbol.ttf"
        "http://pkgs.jrvturnhout.nl/tue-font-ttf/Telognor.ttf"
        "http://pkgs.jrvturnhout.nl/tue-font-ttf/Temetboo.ttf"
        "http://pkgs.jrvturnhout.nl/tue-font-ttf/Temetmed.ttf"
        "http://pkgs.jrvturnhout.nl/tue-font-ttf/Temetwid.ttf"
        "http://pkgs.jrvturnhout.nl/tue-font-ttf/Tescabit.ttf"
        "http://pkgs.jrvturnhout.nl/tue-font-ttf/Tescabol.ttf"
        "http://pkgs.jrvturnhout.nl/tue-font-ttf/Tescaita.ttf"
        "http://pkgs.jrvturnhout.nl/tue-font-ttf/Tescanor.ttf")

build()
{
	cd "${srcdir}"

    for i in *.ttf; do
        local destname="$(echo "$i" | sed 's|-[[:digit:].]\{1,\}\.ttf$|.ttf|')"
        install -Dm 644 "$i" "${pkgdir}/usr/share/fonts/TTF/${destname}"
    done
}

md5sums=('ee5a9a023eb5b68bba1d31e3b1c9800a'
         'b3c653ef2938e635ca004fa484d215f1'
         'be0f6b98cf3012533e3a94809aedd17b'
         'a334b1046a88f00391ea540307c1eee0'
         'a247b9aefe30fe8391224632841c40a0'
         '1095679a2a62a5de8cabdfa4f2f109b1'
         'ddd77cbbd6bffe4064509943bc5703ee'
         'bd7b854afa5201e383349fd47b995764'
         'ae690bd3569e1a17aafd2ebed003393d')