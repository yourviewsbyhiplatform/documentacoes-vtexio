# Blocos Filhos - Detalhes das avaliações

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-product-reviews` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20reviews.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

 - `yv-reviews-histogram` (Histograma) [(documentação)](#)
 - `yv-rating-stars` (Estrelas) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Estrelas.md)
 - `yv-rating-average` (Nota Média) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Nota%20M%C3%A9dia.md)
 - `yv-total-rating` (Total de avaliações) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Total%20de%20Avalia%C3%A7%C3%B5es.md)
 - `yv-reviews-recommend` (Recomendações) [(documentação)](#)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)
 
## Usabilidade

### Nome do bloco

O bloco `yv-reviews-details`, tem como papel, apenas englobar todo os blocos filhos que ele aceita, e retornar informações importantes sobre os detalhes de forma resumida das avaliações

### Propriedades (props)

Nenhuma

### Exemplo de uso:

```jsonc
// yourviews-custom.jsonc
"yv-reviews-details": {
  "children": [
    "yv-reviews-histogram",
    "yv-flex#reviewsRating",
    "yv-reviews-recommend"
  ]
},
```

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwODM1Njc3MTIsLTE4NTMwMzAxMzBdfQ
==
-->