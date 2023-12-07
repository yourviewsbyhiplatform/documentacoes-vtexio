# Blocos Filhos - Porcentagem de Recomendações
## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-reviews-details` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Detalhes%20das%20avalia%C3%A7%C3%B5es.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

Nenhum
 
## Usabilidade

### Nome do bloco

O bloco `yv-reviews-recommend`, tem como papel, exibir a portagem de avaliações que recomendam o produto

### Propriedades (props)

 - `className` - Texto para ser usado como classe do componente (handlers)

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-reviews-details": {
  "children": [
    "yv-reviews-histogram",
    "yv-flex#reviewsRating",
+   "yv-reviews-recommend"
  ]
},
```

### Visual do Componente
![](https://i.imgur.com/hVWiqTY.png)

<br>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTcxMTk4MzZdfQ==
-->