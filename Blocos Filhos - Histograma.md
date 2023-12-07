# Blocos Filhos - Histograma

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-reviews-details` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20reviews.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)
 - `yv-rich-text` (Texto) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Texto.md)

### Blocos filhos aceitos:

 - `yv-histogram-title` (Titulo do Histograma) [(documentação)](#)
 - `yv-histogram-bar` (Barra do Histograma) [(documentação)](#)
 - `yv-histogram-total` (Valor Total do Histograma) [(documentação)](#)
 - `yv-flex` (Flex box) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)
 - `yv-rich-text` (Texto) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Texto.md)

 
## Usabilidade

### Nome do bloco

O bloco `yv-reviews-histogram`, tem como papel, apenas englobar todo os blocos filhos que ele aceita, e retornar informações importantes sobre os detalhes do histograma

### Propriedades (props)

 - `className` - Texto para ser usado como classe do componente (handlers)

### Exemplo de uso:

```jsonc
// yourviews-custom.jsonc
"yv-reviews-histogram": {
  "children": [
    "yv-histogram-title", 
    "yv-histogram-bar", 
    "yv-histogram-total"
  ]
},
```

### Visual do Componente
![](https://i.imgur.com/oBH1GtM.png)

<br>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQ3MDI2MzQxNl19
-->