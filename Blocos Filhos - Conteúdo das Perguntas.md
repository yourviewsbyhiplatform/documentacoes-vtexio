
# Blocos Filhos - Conteúdo das perguntas

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-qa-content` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Conte%C3%BAdo%20das%20perguntas%20e%20respostas.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

 - `yv-comment` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Coment%C3%A1rio.md) 
 - `yv-user-image` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Imagem%20do%20Usu%C3%A1rio.md) 
 - `yv-user-name` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Nome%20do%20Usu%C3%A1rio.md) 
 - `yv-date` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Data.md) 
 - `yv-like-dislike-button` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Like%20e%20Dislike.md)
 
## Usabilidade

### Nome do bloco

O bloco `yv-qa-content-question`, tem como papel, retornar dados importantes sobre as perguntas para seus filhos.

### Propriedades (props)

Nenhum

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-qa-content": {
  "children": [
+   "yv-qa-content-question", 
    "yv-qa-content-answer"
  ]
},
"yv-qa-content-question": {
  "children": ["yv-flex#question-row"]
},
"yv-flex#question-row": {
  "props": {
    "width": "100%",
    "direciton": "column",
    "className": "qa-flex-row"
  },
  "children": [
    "yv-flex#question-col-left", 
    "yv-flex#question-col-right"
  ]
},
"yv-flex#question-col-left": {
  "props": {
    "width": "5%",
    "className": "qa-flex-col-left"
  },
  "children": ["yv-user-image"]
},
"yv-flex#question-col-right": {
  "props": {
    "width": "95%",
    "direction": "column",
    "className": "qa-flex-col-right",
    "justifyContent": "center"
  },
  "children": [
    "yv-flex#question-row-1",
    "yv-comment",
    "yv-like-dislike-buttons"
  ]
},
"yv-flex#question-row-1": {
  "props": {
    "width": "30%",
    "className": "qa-flex-row-1"
  },
  "children": ["yv-user-name", "yv-date#diff"]
},
"yv-date#diff": {
  "props": {
    "showDifference": true
  }
},
```

### Visual do Componente
![](https://i.imgur.com/xqmOYwc.png)

<br>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTkxNTcxNTE4NF19
-->