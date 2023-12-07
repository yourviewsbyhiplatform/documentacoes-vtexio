# Instalação personalizável - Bloco das estrelas de prateleira

## Requisitos

Existem alguns passos muito importantes a serem seguidos antes de efetuar a inserção dos componentes da yourviews no tema da sua loja.

### Instalação do App Yourviews na Vtex Io

Um dos requisitos obrigatórios é possuir o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:
[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)
 
Ao seguir estes passos, você estará preparado para instalar e configurar o bloco noa VTEX IO de maneira eficaz, aproveitando ao máximo as funcionalidades oferecidas. 
 
## Instalação

### Nome do bloco

Conhecido como `yv-product-rating-inline`. Esse bloco é projetado para mostrar as estrelas de avaliação nas prateleiras ou vitrines do site, oferecendo aos clientes uma visão rápida da popularidade e qualidade dos produtos ainda na fase de navegação inicial. Este recurso é especialmente útil nas páginas onde vários produtos são exibidos, como a página inicial ou categorias de produtos.

### Localização do bloco

Normalmente, o bloco `yv-product-rating-inline` é inserido no bloco pai **product-summary.shelf**. Esta é a configuração padrão para exibir as avaliações nas prateleiras ou vitrines do site, comumente localizadas na página inicial da loja.
```
"yv-product-rating-inline"
```

![Instalação do bloco Exemplo](https://i.imgur.com/JM8IKqI.png)

### Personalização do bloco

O bloco `yv-product-rating-inline` pode ser personalizado recebendo alguns blocos filhos que irão compor a sua estrutura, isso é útil para quem deseja criar sua própria estrutura, segue abaixo dois prints padrão e um personalizado:

Padrão:
![](https://i.imgur.com/8HOy0DJ.png)

Personalizado pela loja:
![](https://i.imgur.com/tIKdxE7.png)

Para a personalização do bloco de estrelas de prateleira, pode-se adicionar alguns blocos filhos para compor cada elemento interno que deseja que seja exibido, segue abaixo uma lista com cada bloco filho e suas devidas informações.

#### Blocos filhos (children)

O bloco de das estrelas de prateleira aceita alguns blocos filhos, são eles:

 - `yv-rating-stars` (Estrelas) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Estrelas.md)
 - `yv-rating-average` (Nota Média) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Nota%20M%C3%A9dia.md)
 - `yv-total-rating` (Total de avaliações) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Total%20de%20Avalia%C3%A7%C3%B5es.md)
 - `yv-flex` (Flex Box) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)
 - `yv-rich-text` (Texto) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Texto.md)

#### Propriedades (props)

O bloco das estrelas de prateleira não recebe nenhuma propriedade diretamente

### Exemplo de uso:

```jsonc
// yourviews-custom.jsonc
"yv-product-rating-inline": {
  "children": [
    "yv-total-rating", 
	"yv-rating-stars"
  ]
},
```
```diff
// product-summary.jsonc
"flex-layout.col#productRating": {
  ...
  "children": [
+   "yv-product-rating-inline"
  ]
},
```

<br>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbNDI1NTYwNTExXX0=
-->