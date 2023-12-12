# Instalação personalizável - Bloco de perguntas e respostas

## Requisitos

Existem alguns passos muito importantes a serem seguidos antes de efetuar a inserção dos componentes da yourviews no tema da sua loja.

### Instalação do App Yourviews na Vtex Io

Um dos requisitos obrigatórios é possuir o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:
[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)
 
Ao seguir estes passos, você estará preparado para instalar e configurar o bloco noa VTEX IO de maneira eficaz, aproveitando ao máximo as funcionalidades oferecidas. 
 
## Instalação

### Nome do bloco

Conhecido como `yv-product-questions-and-answers`. Esse bloco é essencial para exibir perguntas e respostas relacionadas a produtos específicos, fornecendo um canal direto de comunicação entre os clientes e a loja. É uma ferramenta poderosa para aumentar a transparência, esclarecer dúvidas dos clientes e auxiliar na decisão de compra.

### Localização do bloco

O bloco `yv-product-questions-and-answers` é normalmente posicionado no bloco pai store.product, que corresponde à página de cada produto individual. Este posicionamento permite que as perguntas e respostas dos clientes estejam diretamente associadas ao produto relevante.
```
"yv-product-questions-and-answers"
```

![Instalação do bloco Exemplo](https://imgur.com/NUS4JYT.png)

### Personalização do bloco

O bloco `yv-product-questions-and-answers` pode ser personalizado recebendo alguns blocos filhos que irão compor a sua estrutura, isso é útil para quem deseja criar sua própria estrutura, segue abaixo dois prints padrão e um personalizado:

Padrão:
![](https://i.imgur.com/wncw9Pb.png)

Personalizado pela loja:
![](https://i.imgur.com/oiNRZLN.png)

Para a personalização do bloco reviews, pode-se adicionar alguns blocos filhos para compor cada elemento interno que deseja que seja exibido, segue abaixo uma lista com cada bloco filho e suas devidas informações.

#### Blocos filhos (children)

O bloco de perguntas e respostas aceita alguns blocos filhos, são eles:

 - `yv-title` (Título) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20T%C3%ADtulo.md)
 - `yv-subtitle` (Sub título) [(documentação)](#)
 - `yv-question-button` (Botão para fazer pergunta) [(documentação)](#)
 - `yv-qa-content` (Conteúdo) [(documentação)](#)
 - `yv-flex` (Flex Box) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)
 - `yv-rich-text` (Texto) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Texto.md)

#### Propriedades (props)

Nenhuma

### Exemplo de uso:

```diff
// product.jsonc
"store.product": {
  "children": [
	...
+   "yv-product-questions-and-answers",
	...
  ]
},
```
```jsonc
// yourviews-custom.jsonc
"yv-product-questions-and-answers": {
  "children": [
    "yv-title#qa",
    "yv-subtitle",
    "yv-question-button",
    "yv-qa-content"
  ]
},
```

<br>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc0NDUzODA0NF19
-->