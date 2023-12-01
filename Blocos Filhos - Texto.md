# Blocos Filhos - Texto

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - Qualquer um

### Blocos filhos aceitos:

- Nenhum
 
 
## Usabilidade

### Nome do bloco

O bloco `yv-rich-text`, tem como papel, apenas retornar um texto que seja desejado apresentar em seu site.,

### Propriedades (props)

O bloco de flex box pode receber diversas propriedades importantes para a personalização, são elas:

 - `text` - Texto que será exibido pelo componente
 - `className` - Texto para ser usado como classe do componente (handlers)

### Exemplo de uso:

```jsonc
// yourviews-custom.jsonc
"yv-store-comment": {
  "children": [
    "yv-rich-text#storeCommentTitle", 
    ...
  ]
},
"yv-rich-text#storeCommentTitle": {
  "props": {
    "text": "Comentário da loja: ",
    "className": "storeCommentTitle"
  }
},
```
```css
/* yourviews.yourviewsreviews.css */
.storeCommentTitle {
  font-weight: bold;
  display: block;
  margin-bottom: 15px;
}
```

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbOTYyOTgyNDEwXX0=
-->