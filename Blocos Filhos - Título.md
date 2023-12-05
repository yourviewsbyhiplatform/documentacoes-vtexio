# Blocos Filhos - Título

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-testimonials` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20dos%20testemunhos.md)
 - `yv-reviews` [(documentação)](#)
 - `yv-questions-and-answers` [(documentação)](#)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

- Nenhum
 
 
## Usabilidade

### Nome do bloco

O bloco `yv-title`, tem como papel, apresentar um título dentro do bloco pai.

### Contextos
Normalmente quando usamos esse bloco, ele é usado mais de uma vez, porém na vtex io, não podemos declarar o mesmo bloco mais de uma vez, portanto recomendamos que você coloque uma `hashtag` com um nome após o nome do bloco para separar esse bloco filho para cada contexto diferente, exemplo:

```json
"yv-title#reviews": {
  "props": {
    "text": "Avaliações dos nossos clientes"
  }
},
"yv-title#qa": {
  "props": {
    "text": "Perguntas e respostas"
  }
},
```

### Propriedades (props)

O bloco de título pode receber duas propriedades importantes para a personalização, são elas:

 - `text` - Texto que será exibido pelo componente
 - `className` - Texto para ser usado como classe do componente (handlers)

### Exemplo de uso:

```jsonc
// yourviews-custom.jsonc
"yv-testimonials": {
  "props": {
    ...
  },
  "children": [
    "yv-title#testimonial", 
    ...
  ]
},

"yv-title#testimonial": {
  "props": {
    "text": "Avaliações da nossa loja"
    "className": "testimonialsTitle"
  }
},
```
```css
/* yourviews.yourviewsreviews.css */
.testimonialsTitle {
  color: red;
}
```

### Visual do Componente
![](https://i.imgur.com/wMSjjIU.png)

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3OTgwMzkxNTFdfQ==
-->