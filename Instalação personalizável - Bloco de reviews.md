# Instalação personalizável - Bloco de reviews

## Requisitos

Existem alguns passos muito importantes a serem seguidos antes de efetuar a inserção dos componentes da yourviews no tema da sua loja.

### Instalação do App Yourviews na Vtex Io

Um dos requisitos obrigatórios é possuir o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:
[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)
 
Ao seguir estes passos, você estará preparado para instalar e configurar o bloco noa VTEX IO de maneira eficaz, aproveitando ao máximo as funcionalidades oferecidas. 
 
## Instalação

### Nome do bloco

O bloco é identificado como `yv-product-reviews`. Ele é projetado para exibir as avaliações e comentários dos clientes sobre produtos específicos. Este bloco é particularmente valioso nas páginas de produtos, onde os clientes podem ler as opiniões e experiências de outros compradores antes de tomar uma decisão de compra.

### Localização do bloco

O bloco `yv-product-reviews` é normalmente posicionado no bloco pai **store.product**, que corresponde à página de cada produto individual. Este posicionamento permite que as avaliações dos clientes estejam diretamente associadas ao produto relevante.
```
"yv-product-reviews"
```

![Instalação do bloco Exemplo](https://imgur.com/FlrF78A.png)

### Personalização do bloco

O bloco `yv-product-reviews` pode ser personalizado recebendo alguns blocos filhos que irão compor a sua estrutura, isso é útil para quem deseja criar sua própria estrutura, segue abaixo dois prints padrão e um personalizado:

Padrão:
![](https://i.imgur.com/5eF7QGZ.png)

Personalizado pela loja:
![](https://i.imgur.com/qRE1ViB.png)

Para a personalização do bloco reviews, pode-se adicionar alguns blocos filhos para compor cada elemento interno que deseja que seja exibido, segue abaixo uma lista com cada bloco filho e suas devidas informações.

#### Blocos filhos (children)

O bloco de reviews aceita alguns blocos filhos, são eles:

 - `yv-title` (Título) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20T%C3%ADtulo.md)
 - `yv-reviews-details` (Detalhes) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Detalhes%20das%20avalia%C3%A7%C3%B5es.md)
 - `yv-reviews-field-summary` (Sumário) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Sum%C3%A1rio%20de%20campos.md)
 - `yv-orderby-select` (Ordenação) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Campo%20de%20Ordena%C3%A7%C3%A3o.md)
 - `yv-reviews-content` (Conteúdo) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Conte%C3%BAdo%20das%20Avalia%C3%A7%C3%B5es.md)
 - `yv-writereview-button` (Botão de escrever avaliação) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Bot%C3%A3o%20de%20Escrever%20Avalia%C3%A7%C3%A3o.md)
 - `yv-flex` (Flex Box) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)
 - `yv-rich-text` (Texto) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Texto.md)

#### Propriedades (props)

 - `hideButtonReview` - Recebe `true` ou `false` - Quando `true` remove o botão de escrever avaliação. (Útil para quando não existe personalização no bloco, ou seja, quando não possui blocos filhos)
 - `orderBy` - Recebe um número que indica o filtro inicial da ordenação das avaliações, escolha um numero inteiro entre 0 e 5, sendo:
	0 para Mais antigos primeiro (padrão)
	1 para Mais novos primeiro
	2 para Mais antigos primeiro
	3 para Melhores notas primeiro
	4 para Mais curtidas primeiro
	5 para Mais descurtidas primeiro

### Exemplo de uso:

```diff
// product.jsonc
"store.product": {
  "children": [
	...
+   "yv-product-reviews",
	...
  ]
},
```
```jsonc
// yourviews-custom.jsonc
"yv-product-reviews": {
  "children": [
    "yv-reviews-details",
    "yv-reviews-field-summary",
    "yv-orderby-select",
    "yv-title#reviews",
    "yv-reviews-content",
    "yv-writereview-button",
  ]
},
```

<br>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc3NjMwNTY1XX0=
-->
