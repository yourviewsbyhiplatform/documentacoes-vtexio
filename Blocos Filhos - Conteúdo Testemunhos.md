# Blocos Filhos - Conteúdo dos testemunhos

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-testimonials` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20dos%20testemunhos.md)
 - `yv-reviews` [(documentação)](#)
 - `yv-questions-and-answers` [(documentação)](#)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

 - `yv-rating-stars` [(documentação)](#)
 - `yv-rating-average` [(documentação)](#)
 - `yv-date` [(documentação)](#)
 - `yv-user-image` [(documentação)](#)
 - `yv-user-name` [(documentação)](#)
 - `yv-user-localization` [(documentação)](#)
 - `yv-comment` [(documentação)](#)
 - `yv-store-ratings` [(documentação)](#)
 
 
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
eyJoaXN0b3J5IjpbMTYwMDY0OTI3OCw1NjczMDg1MDNdfQ==
-->