---
$title: Modificar a apresentação e o layout
---

## Modificar a apresentação

AMPs são páginas da Web; qualquer estilo adicionado à página e a seus elementos é feito usando propriedades CSS comuns. Adicione estilos aos elementos usando os seletores de classe ou elemento em uma folha de estilo do `<head>`, que se chama `<style amp-custom>`:

[sourcecode:html]
<style amp-custom>
  /* any custom style goes here */
  body {
    background-color: white;
  }
  amp-img {
    background-color: gray;
    border: 1px solid black;
  }
</style>
[/sourcecode]

Cada página AMP pode ter apenas uma folha de estilo incorporada e há certos seletores que você não tem permissão para usar. [Saiba tudo sobre estilos](/pt_br/docs/guides/author-develop/responsive/style_pages.html).

## Controlar o layout

O AMP segue regras mais restritas para o layout dos elementos na página. Em uma página HTML normal, você usa CSS quase que exclusivamente para criar o layout. No entanto, por razões de desempenho, o AMP exige que todos os elementos tenham um conjunto de tamanhos explícito desde o início.

Saiba mais sobre como o AMP renderiza e faz o layout de uma página e como você pode modificá-lo em [Como controlar o layout](/pt_brdocs/guides/author-develop/responsive/control_layout.html).

<a class="go-button button" href="/pt_br/docs/tutorials/create/preview_and_validate.html">Continuar para a etapa 4</a>
