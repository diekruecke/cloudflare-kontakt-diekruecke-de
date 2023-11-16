# cloudflare-kontakt-diekruecke-de
hugo mod init github.com/diekruecke/cloudflare-kontakt-diekruecke-de

hugo mod get -u -v joly.pw/gohugo-shorturl
hugo mod get -u -v github.com/diekruecke/krueckeKontaktTheme



config/_default/module.toml
[[imports]]
path = "joly.pw/gohugo-shorturl"

git clone https://github.com/diekruecke/krueckeKontaktTheme themes/krueckeKontaktTheme --depth=1

cd themes/PaperMod
git pull