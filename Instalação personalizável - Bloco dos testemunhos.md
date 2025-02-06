# Instalação personalizável - Bloco dos testemunhos

## Requisitos

Existem alguns passos muito importantes a serem seguidos antes de efetuar a inserção dos componentes da yourviews no tema da sua loja.

### Instalação do App Yourviews na Vtex Io

Um dos requisitos obrigatórios é possuir o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:
[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)
 
 Ao seguir estes passos, você estará preparado para instalar e configurar o bloco noa VTEX IO de maneira eficaz, aproveitando ao máximo as funcionalidades oferecidas. 
 
## Instalação

### Nome do bloco

Conhecido como `yv-testimonials`, desempenha um papel crucial na experiência de compra online. Esse bloco é especificamente projetado para apresentar as avaliações e opiniões dos clientes sobre a loja, após a conclusão de uma compra. 

### Localização do bloco

O bloco de testemunhos é geralmente inserido no código fonte do app tema da sua loja, no arquivo `home.json` dentro do bloco `store.home`, que normalmente corresponde à página home da loja.
```
"yv-testimonials"
```

![Instalação do bloco Exemplo](https://yv-misc.s3.us-east-1.amazonaws.com/help/yv-help-docs/80%20-%20Tetsimonials.png)

Embora o bloco de testemunhos seja comumente inserido na página inicial isso não quer dizer que você obrigatoriamente deverá inseri-lo na página home do site, é apenas o usual. Fique a vontade para incluir o componente onde quiser.

### Personalização do bloco

O bloco `yv-testimonials` pode ser personalizado recebendo alguns blocos filhos que irão compor a sua estrutura, isso é útil para quem deseja criar sua própria estrutura, segue abaixo dois prints padrão e um personalizado:

Padrão:
![](https://i.imgur.com/As4ZBwO.png)

Personalizado pela loja:
![](https://i.imgur.com/W5QSqRd.png)

Para a personalização do bloco de testemunhos, pode-se adicionar alguns blocos filhos para compor cada elemento interno que deseja que seja exibido, segue abaixo uma lista com cada bloco filho e suas devidas informações.

#### Blocos filhos (children)

O bloco de testemunhos aceita alguns blocos filhos, são eles:

 - `yv-title` (Título) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20T%C3%ADtulo.md)
 - `yv-testimonials-content` (Conteúdo) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Conte%C3%BAdo%20Testemunhos.md)
 - `yv-flex` (Flex Box) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)
 - `yv-rich-text` (Texto) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Texto.md)

#### Propriedades (props)

O bloco de testemunhos pode receber uma propriedade importantes para a sua personalização.

A propriedade `slidesToShow` recebe um quatro informações, que especificam quantos slides serão exibidos por tamanho de tela, são elas:

 - `tinyMobile` (para telas menores que 375px)
 - `mobile` (para telas menores que 600px)
 - `desktop` (para telas menores que 990px)
 - `bigDesktop` (para telas maiores que 990px)

### Exemplo de uso:

```jsonc
// yourviews-custom.jsonc
"yv-testimonials": {
  "props": {
    "slidesToShow": {
      "tinyMobile": 1,
      "mobile": 1,
      "desktop": 3,
      "bigDesktop": 3
    }
  },
  "children": [
    ...
  ]
},
```
```diff
// home.jsonc
"store.home": {
    "blocks": [
      ...
     "yv-testimonials"
    ]
  },
```

<br>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbOTE0ODcyNzMzLDE2NDE0MjgyOTBdfQ==
-->