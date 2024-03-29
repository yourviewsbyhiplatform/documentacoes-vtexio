# Blocos Filhos - Campo de Ordenação

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-product-reviews` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20reviews.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

- Nenhum
 
## Usabilidade

### Nome do bloco

O bloco `yv-orderby-select`, tem como papel, dar a possibilidade de ordenar as avaliações de acordo com a opção selecionado.

### Propriedades (props)

 - `orderBy` - Recebe um número que indica o filtro inicial da ordenação das avaliações, escolha um numero inteiro entre 0 e 5, sendo:
	 - **0** para Mais antigos primeiro (padrão)
	 - **1** para Mais novos primeiro
	 - **2** para Mais antigos primeiro
	 - **3** para Melhores notas primeiro
	 - **4** para Mais curtidas primeiro
	 - **5** para Mais descurtidas primeiro

![](https://i.imgur.com/QjHmvrl.png)

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-product-reviews": {
  "children": [
    "yv-reviews-details",
    "yv-reviews-field-summary",
+   "yv-orderby-select",
    "yv-title#reviews",
    "yv-reviews-content",
    "yv-writereview-button",
  ]
},
"yv-orderby-select": {
  "props": {
    "orderBy": 2
  }
},
```

### Visual do Componente
![](https://i.imgur.com/e5MJNmo.png)

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzNDIyMTQ1MDVdfQ==
-->