# SysDocs - web-estatica-ss-as

Web de documentació tècnica per a administradors de sistemes, feta amb **MkDocs 1.6.1** (Python) i publicada amb GitHub Pages.

**URL publicada:** https://aaronsanchez2811.github.io/web-estatica-ss-as/

## Eina i motiu

He triat **MkDocs** perquè està pensat per a documentació tècnica, es configura amb un sol fitxer (`mkdocs.yml`) i el contingut s'escriu en Markdown.

| | Hugo | Jekyll | MkDocs |
|---|------|--------|--------|
| Llenguatge | Go | Ruby | Python |
| Orientació | Webs i blogs | Blogs i webs senzilles | Documentació tècnica |
| Velocitat | Molt alta | Mitjana | Alta |
| Configuració | `hugo.toml` | `_config.yml` | `mkdocs.yml` |

## Instal·lació i ús local

```bash
pip install mkdocs

mkdocs serve      # servidor local a http://127.0.0.1:8000
mkdocs build      # genera la carpeta site (HTML, CSS, JS)
```

## Publicació

1. `git add`, `git commit`, `git push` a la branca `main`.
2. A GitHub: *Settings > Pages > Source: GitHub Actions*.

## Desplegament automàtic

El workflow `.github/workflows/deploy.yml` s'executa a cada `push` a `main`: instal·la MkDocs, executa `mkdocs build` i publica `site` a GitHub Pages.

## Estructura

```text
.github/workflows/deploy.yml   # GitHub Actions
mkdocs.yml                     # configuració
docs/                          # fitxers font (Markdown, imatges, CSS)
  index.md  linux/  xarxes/  serveis/  blog/  img/  stylesheets/
site/                          # fitxers generats (no es puja a Git)
```
