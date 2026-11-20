# Blog do Victor Neves

Blog pessoal em HTML estático, com ensaios sobre "tudo um pouco": programação, filosofia moderna, economia e comportamento. Funciona como PWA (instalável e com cache offline via service worker).

**Demo:** https://voaneves.github.io/blog/

## Posts

- **Como começar a programar websites**: ponto de partida para quem quer construir sites.
- **O pobre que compra iPhone**: ensaio sobre consumo e escolhas financeiras.
- **Somos bons ou maus? Um estudo em várias áreas do conhecimento**: ensaio que cruza diferentes áreas para discutir a natureza humana.

## Como rodar

Não há build nem dependências. Clone e sirva a pasta com qualquer servidor estático (o service worker exige `http://localhost` ou HTTPS):

```bash
gh repo clone voaneves/blog
cd blog
python -m http.server 8000
```

Acesse http://localhost:8000.

## Estrutura

```
index.html                           página inicial
como-começar-a-programar-websites.html
o-pobre-que-compra-iphone.html
somos-bons-ou-maus.html
manifest.json                        manifesto PWA
sw.js / sw.min.js                    registro do service worker
worker.js / worker.min.js            service worker
assets/                              fonts, img, js e styles
```

## Stack

HTML, CSS e JavaScript puros; metadados de SEO (description, keywords, Open Graph), tema claro/escuro (`color-scheme`) e PWA com manifest + service worker.

## Licença

O código está sob a licença MIT (veja [LICENSE](LICENSE)). Os textos dos posts e as imagens são © Victor Neves, todos os direitos reservados.
