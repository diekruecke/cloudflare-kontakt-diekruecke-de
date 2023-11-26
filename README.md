# cloudflare-kontakt-diekruecke-de

1. Hugo Mod init

```shell
hugo mod init github.com/diekruecke/cloudflare-kontakt-diekruecke-de

hugo mod get -u -v joly.pw/gohugo-shorturl

hugo mod get -u -v github.com/diekruecke/krueckeKontaktTheme
```

2. Hugo Mod init

```bash
git submodule add https://github.com/cljoly/gohugo-shorturl.git themes/gohugo-shorturl
git submodule add https://github.com/martignoni/hugo-cloak-email.git themes/hugo-cloak-email

git submodule add https://github.com/diekruecke/krueckeKontaktTheme.git themes/krueckeKontaktTheme
```

3. Für die config

```yaml
[module]
  [[module.imports]]
    path = "joly.pw/gohugo-shorturl"

```

4. Submodule deinit

    ```shell
    git submodule deinit themes/krueckeKontaktTheme
    git rm themes/krueckeKontaktTheme

    git submodule deinit themes/joly.pw/gohugo-shorturl
    git rm themes/joly.pw/gohugo-shorturl
    ```


git submodule update --init --recursive