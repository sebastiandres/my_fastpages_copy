---
toc: true
description: Ejemplo usando markdown con fastpages.
categories: [fastpages, markdown]
---
# Test 1: Post mediante Markdown

## Configuración básica

Un blog post files debe tener el siguiente formato:

`AAAA-MM-DD-filename.md`

Donde `AAAA` es el año con 34 dígitos, `MM` es el mes con 2 dígitos, `DD` es el día con 2 dígitos, y `filename` es un nombre de referencia para recordarte de que se trataba el post (el título real se indica adentro). La extensión `.md` se usa para archivos markdown.

La primera línea del archivo debe comenzar con `# Mi título` para que se defina "Mi título" como el título del post. Dentro del post, se pueden hacer subtítulos `## Mi subtítulo` (y sub-subtítulos, `### Mi sub-subtítulo`, pero ya es desaconsejado.)

# Configuración avanzada

Para agregar una descripción, categorías (etiquetas/tags), y toc (table of contents - tabla de contenidos) es necesario agregar un contenido específico encerrado por `---`. Por ejemplo, las primeras 10 líneas de este post son las siguientes:

```
---
toc: true
description: Ejemplo usando markdown con fastpages.
categories: [fastpages, markdown]
---
# Test 1: Post mediante Markdown

## Configuración básica

Un blog post files debe tener el siguiente formato:
```

Para desactivar la funcionalidad basta con eliminarla o dejarla vacía.

## Formato básico

Se pueden usar *cursivas*, **negritas**, ***negritas cursivas***, `código`, y crear [links](https://www.markdownguide.org/cheat-sheet/). También notas a pie de página [^1]. También una línea horizontal:

---

## Listas

Acá hay una lista (regular):

- item 1
- item 2

Acá hay una lista numerada:

1. item 1
1. item 2

## Citas y otras formas de destacar

Citas:
> Esta es una cita

Alerta:
{% include alert.html text="Puedes incluir alertas" %}

Información:
{% include info.html text="Puedes destacar información" %}

## Imágenes

![]({{ site.baseurl }}/images/logo.png "fast.ai's logo")

## Código

Texto preformateado general:

    # Do a thing in a programming language
    do_thing()

Código de python y su salida:

```python
# Prints '2'
print(1+1)
```

    2


## Tablas

| Columna 1 | Columna 2 |
|-|-|
| Una cosa | Otra cosa |
| Una cosa más | Otra cosa más |


## Tweets

{% twitter https://twitter.com/jakevdp/status/1204765621767901185?s=20 %}


## Notas a pie de página

[^1]: Esta es la nota al pie de página.

