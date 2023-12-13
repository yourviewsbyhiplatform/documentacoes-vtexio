# Blocos Filhos - Botão de pergunta

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-product-questions-and-answers` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20perguntas%20e%20respostas.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

- Nenhum
 
## Usabilidade

### Nome do bloco

O bloco `yv-question-button`, tem como papel, apresentar botão que ao clicar, abre um formulário para que o usuário possa realizar uma pergunta sobre o produto.

### Propriedades (props)

Nenhum

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-product-questions-and-answers": {
  "children": [
    "yv-title#qa",
    "yv-subtitle",
+   "yv-question-button",
    "yv-qa-content"
  ]
},
```

### Visual do Componente
![](https://i.imgur.com/DrHJLba.png)

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQ0Nzk5NzcxNV19
-->