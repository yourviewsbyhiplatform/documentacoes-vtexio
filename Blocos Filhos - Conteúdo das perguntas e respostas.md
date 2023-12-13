
# Blocos Filhos - Conteúdo das perguntas e respostas

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-product-questions-and-answers` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20perguntas%20e%20respostas.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

- `yv-qa-content-question` (Conteúdo das perguntas) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Conte%C3%BAdo%20das%20Perguntas.md)
- `yv-qa-content-answer` (Conteúdo das respostas) [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Conte%C3%BAdo%20das%20respostas.md)
 
## Usabilidade

### Nome do bloco

O bloco `yv-qa-content`, tem como papel, retornar dados importantes sobre as perguntas e as respostas para seus filhos.

### Propriedades (props)

Nenhum

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-product-questions-and-answers": {
  "children": [
    "yv-title#qa",
    "yv-subtitle",
    "yv-question-button",
+   "yv-qa-content"
  ]
},
```

### Visual do Componente
![](https://i.imgur.com/JAOMtx8.png)

<br>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQ0Njg1NDA1N119
-->