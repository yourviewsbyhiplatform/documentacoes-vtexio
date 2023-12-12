# Blocos Filhos - Conteúdo das Avaliações

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-product-reviews` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20reviews.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

 - `yv-content-review` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Conte%C3%BAdo%20Interno%20das%20avalia%C3%A7%C3%B5es.md) 

## Usabilidade

### Nome do bloco

O bloco `yv-reviews-content`, tem como papel, apenas envolver o conteúdo de cada avaliação

### Propriedades (props)

 - `className` - Texto para ser usado como classe do componente (handlers)

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-product-reviews": {
  "children": [
    "yv-reviews-details",
    "yv-reviews-field-summary",
    "yv-orderby-select",
    "yv-title#reviews",
+   "yv-reviews-content",
    "yv-writereview-button",
    "yv-reviewform-component"
  ]
},
+ "yv-reviews-content": {
+   "children": ["yv-content-review"]
+ },
```

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbODU3ODExMjQ4XX0=
-->