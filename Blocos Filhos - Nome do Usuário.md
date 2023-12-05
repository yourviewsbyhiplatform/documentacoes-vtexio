# Blocos Filhos - Nome do Usuário

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

O bloco `yv-user-name`, tem como papel, apresentar o nome do usuário acordo com o conteúdo dentro do bloco pai.

### Propriedades (props)

 - `className` - Texto para ser usado como classe do componente (handlers)
 - `initialsOnly` - Recebe `true` ou `false` - Quando `true` exibe apenas as iniciais do nome

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-flex#slide": {
  "props": {
    ...
  },
  "children": [
+   "yv-user-name",
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
eyJoaXN0b3J5IjpbNzM3NzI0NDc2LC0xMjA5NDI1MjI1XX0=
-->