# Blocos Filhos - Estrelas

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-testimonials-content` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Conte%C3%BAdo%20Testemunhos.md)
 - `yv-product-rating-inline` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20das%20estrelas%20de%20prateleira.md)
 - `yv-product-rating-summary` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20das%20estrelas%20de%20ancoragem.md)
 - `yv-reviews-details` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Detalhes%20das%20avalia%C3%A7%C3%B5es.md)
 - `yv-reviews-field-summary` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Sum%C3%A1rio%20de%20campos.md)
 - `yv-content-review` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Conte%C3%BAdo%20Interno%20das%20avalia%C3%A7%C3%B5es.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

- Nenhum
 
## Usabilidade

### Nome do bloco

O bloco `yv-rating-stars`, tem como papel, apresentar as estrelas de acordo com a nota dentro do bloco pai.

### Propriedades (props)

 - `className` - Texto para ser usado como classe do componente (handlers)

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-flex#slide": {
  "props": {
    ...
  },
  "children": [
+   "yv-rating-stars",
    ...
  ]
},
```

### Visual do Componente
![](https://i.imgur.com/okMRHqX.png)

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTU4MDI3ODE2N119
-->