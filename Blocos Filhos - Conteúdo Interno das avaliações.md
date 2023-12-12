# Blocos Filhos - Conteúdo interno das Avaliações

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-reviews-content` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20reviews.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

 - `yv-rating-stars` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Estrelas.md)
 - `yv-comment` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Coment%C3%A1rio.md) 
 - `yv-custom-fields` [(documentação)](#) 
 - `yv-user-image` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Imagem%20do%20Usu%C3%A1rio.md) 
 - `yv-user-name` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Nome%20do%20Usu%C3%A1rio.md) 
 - `yv-date` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Data.md) 
 - `yv-review-photo` [(documentação)](#)
 - `yv-store-comment` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Coment%C3%A1rio%20da%20Loja.md)
 - `yv-like-dislike-button` [(documentação)](#)

## Usabilidade

### Nome do bloco

O bloco `yv-content-review`, tem como papel, retornar os valores correto para cada bloco filho que envolve a estrutura da listagem das avaliações

### Propriedades (props)

Nenhuma

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-content-review": {
  "children": [
    "yv-flex#review-col-1",
    "yv-flex#review-col-2"
  ]
},
```

### Visual do Componente
![](https://i.imgur.com/fj3fdmW.png)

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbMzIzNzgxMTBdfQ==
-->