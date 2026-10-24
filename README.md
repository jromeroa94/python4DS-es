# Python for Data Science en español

Traducción al español, no oficial, de [**Python for Data Science**](https://aeturrell.github.io/python4DS/), el libro abierto de Arthur Turrell y la comunidad Py4DS que enseña a cargar, transformar, visualizar y comunicar datos con Python. El original sigue la estructura de *R for Data Science (2e)*.

**Lee el libro en:** <https://jromeroa94.github.io/python4DS-es/>

- Original en inglés: <https://aeturrell.github.io/python4DS/> · repositorio [aeturrell/python4DS](https://github.com/aeturrell/python4DS)
- Versión del original que se tradujo: ver [`UPSTREAM.md`](UPSTREAM.md)

## Sobre la traducción

- Español neutro, con trato de «tú», pensado para lectores de Latinoamérica y España.
- El código, los identificadores, los nombres de librerías y de conjuntos de datos, la bibliografía y los términos técnicos de uso habitual (dataframe, pipeline, string, tidy data…) se mantienen en inglés, como es costumbre en la comunidad hispanohablante de ciencia de datos. Las etiquetas de las figuras están traducidas.
- La traducción se hizo con ayuda de inteligencia artificial (Claude), con comprobaciones automáticas de cada bloque (código, enlaces, referencias cruzadas) y revisión manual. Puede contener errores.

Este repositorio es un fork del original, de modo que comparte su historial de git. Cada semana un workflow comprueba si el original cambió y, si es así, abre un issue con los capítulos afectados para mantener la traducción al día.

## Cómo contribuir

Las correcciones son muy bienvenidas:

- Si encuentras un error de traducción, abre un [issue](https://github.com/jromeroa94/python4DS-es/issues) o propón el cambio directamente con un pull request.
- Los errores de contenido que también estén en el original conviene reportarlos en [aeturrell/python4DS](https://github.com/aeturrell/python4DS/issues).

## Construir el libro en local

Necesitas Python 3.10 o superior, [**uv**](https://docs.astral.sh/uv/) y [**Quarto**](https://quarto.org/docs/get-started/).

```bash
git clone https://github.com/jromeroa94/python4DS-es
cd python4DS-es
uv sync
uv run quarto render --execute
```

El libro queda en `_book/`. Antes de enviar un pull request, comprueba que pasan los hooks de pre-commit (`uv run pre-commit run --all-files`) y que los notebooks no guardan salidas.

Al publicar cambios en `main`, el workflow `.github/workflows/release.yml` vuelve a construir el libro y lo publica en GitHub Pages.

## Créditos y licencia

El contenido original es obra de [Arthur Turrell](https://aeturrell.com/) y de [los colaboradores de Python4DS](https://aeturrell.github.io/python4DS/), y se distribuye con licencia MIT. Esta traducción, de Johan Romero Aguirre ([@jromeroa94](https://github.com/jromeroa94)), se publica con la misma licencia; consulta [`LICENSE`](LICENSE).
