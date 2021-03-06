---
$title: Incluir Iframes
---
[TOC]

Aprenda cómo mostrar contenido multimedia en sus páginas y cómo utilizar iframes
para mostrar contenido avanzado fuera de las limitaciones de AMP.

## Lo básico

Muestra un iframe en tu página usando el elemento 
[`amp-iframe`](/es/docs/reference/components/amp-iframe.html).

Los iframes son especialmente útiles en AMP para mostrar contenido no
soportado en el contexto de la página principal, como el contenido que requiere JavaScript.

### Requerimientos del elemento `amp-iframe`

* Debe ser al menos de **600px** o **75%** de la primera ventana de visualización lejos de la parte superior.
* Solo puede solicitar recursos a través de HTTPS, y no deben estar en el mismo origen que el contenedor, a menos que no especifique allow-same-origin.

{% call callout('Read on', type='read') %}
Aprende más sobre [lista de especificación para <code>amp-iframe</code>](/es/docs/reference/components/amp-iframe.html).
{% endcall %}

### Incluir el script

Para incluir `amp-iframe` en tu página,
primero incluye el siguiente script en `<head>`, que cargará código 
adicional para el componente extendido:

[sourcecode:html]
<script async custom-element="amp-iframe"
  src="https://cdn.ampproject.org/v0/amp-iframe-0.1.js"></script>
[/sourcecode]

### Escribir el marcado

Un ejemplo de `amp-iframe`:


```html
<amp-iframe width="200" height="100"
    sandbox="allow-scripts allow-same-origin"
    layout="responsive"
    src="https://www.google.com/maps/embed/v1/place?key=AIzaSyDG9YXIhKBhqclZizcSzJ0ROiE0qgVfwzI&q=europe">
</amp-iframe>
```

Renders as: 

<amp-iframe width="200" height="100"
    sandbox="allow-scripts allow-same-origin"
    layout="responsive"
    src="https://www.google.com/maps/embed/v1/place?key=AIzaSyDG9YXIhKBhqclZizcSzJ0ROiE0qgVfwzI&q=europe">
</amp-iframe>

## Ejemplos

Hay ejemplos más avanzados que puedes encontrar en nuestra [página demo avanzada](https://ampbyexample.com/components/amp-iframe/).
