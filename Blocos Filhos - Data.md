# Blocos Filhos - Data

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-testimonials-content` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Conte%C3%BAdo%20Testemunhos.md)
 - `yv-qa-content-question` [(documentação)](#)
 - `yv-qa-content-answer` [(documentação)](#)
 - `yv-content-review` [(documentação)](#)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

- Nenhum
 
## Usabilidade

### Nome do bloco

O bloco `yv-date`, tem como papel, apresentar a data acordo com o conteúdo dentro do bloco pai.

### Propriedades (props)

 - `className` - Texto para ser usado como classe do componente (handlers)
 - `showDifference` - Recebe `true` ou `false` - Quando `true` exibe "x dias/meses/anos atrás" ao invés da data padrão

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-flex#slide": {
  "props": {
    ...
  },
  "children": [
+   "yv-date",
    ...
  ]
},
```

### Visual do Componente
![](https://i.imgur.com/JDQF64F.png)
ou
![](https://i.imgur.com/mNtuwGf.png)

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIxMjQzOTQzOTVdfQ==
-->