# Blocos Filhos - Conteúdo dos testemunhos

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-testimonials` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20dos%20testemunhos.md)
 - `yv-reviews` [(documentação)](#)
 - `yv-questions-and-answers` [(documentação)](#)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

 - `yv-rating-stars` (Estrelas) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Estrelas.md)
 - `yv-rating-average` (Nota média) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Nota%20M%C3%A9dia.md)
 - `yv-date` (Data) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Data.md)
 - `yv-user-image` (Imagem do usuário) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Imagem%20do%20Usu%C3%A1rio.md)
 - `yv-user-name` (Nome do usuário) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Nome%20do%20Usu%C3%A1rio.md)
 - `yv-user-localization` (Localização do usuário)[(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Localiza%C3%A7%C3%A3o%20do%20Usu%C3%A1rio.md)
 - `yv-comment` (Comentário) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Coment%C3%A1rio.md)
 - `yv-store-ratings` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Avalia%C3%A7%C3%B5es%20da%20Loja.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)
 
 
## Usabilidade

### Nome do bloco

O bloco `yv-testimonials-content`, tem como papel, apenas englobar todo os blocos filhos que ele aceita, e tem como papel retornar informações importantes sobre cada avaliação de loja.

### Propriedades (props)

Esse bloco não aceita nenhuma propriedade específica.

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-testimonials": {
  ...
  "children": [
    ...
    "yv-testimonials-content"
  ]
},
 "yv-testimonials-content": {
   "children": ["yv-flex#slide"]
 },
```

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0MzE1OTgxOTQsLTIwMTM0OTY1ODZdfQ
==
-->