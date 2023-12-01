# Blocos Filhos - Título

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho.

Os blocos que podem receber esse bloco como filho são:

 - `yv-testimonials`
 - `yv-reviews`
 - `yv-questions-and-answers`
 - `yv-flex`
 
 
## Usabilidade

### Nome do bloco

O bloco `yv-title`, tem como papel, apresentar um título dentro do bloco pai, normalmente quando usamos esse bloco, ele é usado mais de uma vez, por exemplo, usamos ele nas avaliações e nas perguntas

Porém na vtex io, não podemos declarar o mesmo bloco mais de uma vez, portanto recomendamos que você coloque uma `hashtag` após o nome do bloco para separar esse bloco filho para cada contexto diferente, exemplo:

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

 - `text`
 - `className`

A propriedade `text` recebe um texto, esse texto é o texto que será apresentado pelo bloco na renderização da página.

A propriedade `className` recebe um texto, esse texto no caso será usado como uma class no css handlers da vtex para personalizações no CSS.

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

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbMjI4NDMyODAwXX0=
-->