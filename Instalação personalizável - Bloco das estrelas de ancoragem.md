# Instalação personalizável - Bloco das estrelas de ancoragem

## Requisitos

Existem alguns passos muito importantes a serem seguidos antes de efetuar a inserção dos componentes da yourviews no tema da sua loja.

### Instalação do App Yourviews na Vtex Io

Um dos requisitos obrigatórios é possuir o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:
[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)
 
Ao seguir estes passos, você estará preparado para instalar e configurar o bloco noa VTEX IO de maneira eficaz, aproveitando ao máximo as funcionalidades oferecidas. 
 
## Instalação

### Nome do bloco

Conhecido como `yv-product-rating-summary`. Esse bloco é essencial para exibir um resumo das avaliações de produtos em forma de estrelas, uma ferramenta chave para impulsionar a confiança e auxiliar na decisão de compra dos clientes. O bloco é comumente posicionado na página de cada produto, oferecendo uma visão rápida e clara das avaliações que o produto recebeu.

### Localização do bloco

O bloco yv-product-rating-summary é normalmente inserido no bloco pai store.product, que corresponde à página de cada produto. Esta localização estratégica permite que os clientes vejam rapidamente a avaliação do produto em questão.
```
"yv-product-rating-summary"
```

![Instalação do bloco Exemplo](https://i.imgur.com/48VoM5p.png)

### Personalização do bloco

O bloco `yv-product-rating-summary` pode ser personalizado recebendo alguns blocos filhos que irão compor a sua estrutura, isso é útil para quem deseja criar sua própria estrutura, segue abaixo dois prints padrão e um personalizado:

Padrão:
![](https://i.imgur.com/8HOy0DJ.png)

Personalizado pela loja:
![](https://i.imgur.com/tIKdxE7.png)

Para a personalização do bloco de estrelas de ancoragem, pode-se adicionar alguns blocos filhos para compor cada elemento interno que deseja que seja exibido, segue abaixo uma lista com cada bloco filho e suas devidas informações.

#### Blocos filhos (children)

O bloco de das estrelas de ancoragem aceita alguns blocos filhos, são eles:

 - `yv-rating-stars` (Estrelas) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Estrelas.md)
 - `yv-rating-average` (Nota Média) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Nota%20M%C3%A9dia.md)
 - `yv-total-rating` (Total de avaliações) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Total%20de%20Avalia%C3%A7%C3%B5es.md)
 - `yv-flex` (Flex Box) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)
 - `yv-rich-text` (Texto) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Texto.md)

#### Propriedades (props)

O bloco das estrelas de ancoragem não recebe nenhuma propriedade diretamente

### Exemplo de uso:

```jsonc
// yourviews-custom.jsonc
"yv-product-rating-summary": {
  "children": ["yv-flex#rating-summary"]
},
```
```diff
// product.jsonc
"flex-layout.col#right-col": {
  ...
  "children": [
    "flex-layout.row#product-name",
+   "yv-product-rating-summary",
    ...
  ]
},
```

<br>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc4OTI4MDA1OCwyNTk1MjUyNDddfQ==
-->