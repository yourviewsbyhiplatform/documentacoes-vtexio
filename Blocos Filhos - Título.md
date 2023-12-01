# Blocos Filhos - Título

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-testimonials`
 - `yv-reviews`
 - `yv-questions-and-answers`
 - `yv-flex`

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
+    "yv-title#testimonial", 
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
eyJoaXN0b3J5IjpbLTIwNjM1OTI5ODNdfQ==
-->