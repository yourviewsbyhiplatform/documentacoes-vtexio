# Blocos Filhos - Barra Histograma

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-reviews-histogram` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20reviews.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

Nenhum
 
## Usabilidade

### Nome do bloco

O bloco `yv-histogram-bar`, tem como papel, exibir as barras de cada histograma

### Propriedades (props)

 - `className` - Texto para ser usado como classe do componente (handlers)

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-reviews-histogram": {
  "children": [
    "yv-histogram-title", 
+   "yv-histogram-bar", 
    "yv-histogram-total"
  ]
},
```

### Visual do Componente
![](https://i.imgur.com/IczKBCw.png)

<br>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2Njc2MjA5NTNdfQ==
-->