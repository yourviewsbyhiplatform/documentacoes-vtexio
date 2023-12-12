# Blocos Filhos - Botão de Escrever Avaliação

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-product-reviews` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20reviews.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

- Nenhum
 
## Usabilidade

### Nome do bloco

O bloco `yv-writereview-button`, tem como papel, ao clicar, carregar o formulário de avaliação.

**Importante ->** O botão de escrever avaliação deve ser usando juntamente com o bloco do formulário `yv-reviewform-component`, pois ao clicar no botão, o mesmo irá sumir o formulário será carregado. 

Deixamos a opção de inserir cada um dos blocos separadamente para dar a possibilidade de inserir o botão onde desejar e de poder carregar o formulário onde desejar também, por exemplo no início ou fim do conteúdo das avaliações.

`yv-reviewform-component` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Formul%C3%A1rio%20de%20Avalia%C3%A7%C3%A3o.md)

### Propriedades (props)

Nenhuma

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-product-reviews": {
  "children": [
    "yv-reviews-details",
    "yv-reviews-field-summary",
    "yv-orderby-select",
    "yv-title#reviews",
    "yv-reviews-content",
+   "yv-writereview-button",
    "yv-reviewform-component"
  ]
},
```

### Visual do Componente
![](https://i.imgur.com/Uuo0P1a.png)

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbODAzNTU3OTE5XX0=
-->