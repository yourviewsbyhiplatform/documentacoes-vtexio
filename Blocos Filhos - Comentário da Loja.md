# Blocos Filhos - Comentário da Loja
## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-content-review` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20reviews.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

 - `yv-comment` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Coment%C3%A1rio.md) 
 - `yv-date` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Data.md) 

## Usabilidade

### Nome do bloco

O bloco `yv-store-comment`, tem como papel, retornar o comentário e data do comentário feito pela loja sobre aquela avaliação específica.

### Propriedades (props)

 - `className` - Texto para ser usado como classe do componente (handlers)

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-flex#review-row-6": {
  "props": {
    "direction": "row",
    "justifyContent": "space-between"
  },
  "children": [
+   "yv-store-comment"
  ]
},
"yv-rich-text#storeCommentTitle": {
  "props": {
    "text": "Comentário da loja: ",
    "className": "storeCommentTitle"
  }
},
"yv-store-comment": {
  "children": [
    "yv-rich-text#storeCommentTitle", 
    "yv-comment", 
    "yv-date"
  ]
},
```

### Visual do Componente
![](https://i.imgur.com/1noyCUb.png)

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTcxNTUwNDEwN119
-->