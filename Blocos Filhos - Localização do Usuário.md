# Blocos Filhos - Localização do Usuário

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-testimonials-content` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Conte%C3%BAdo%20Testemunhos.md)
 - `yv-content-review` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Conte%C3%BAdo%20Interno%20das%20avalia%C3%A7%C3%B5es.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

- Nenhum
 
## Usabilidade

### Nome do bloco

O bloco `yv-user-localization`, tem como papel, apresentar a localização do usuário de acordo com o conteúdo dentro do bloco pai.

### Propriedades (props)

 - `className` - Texto para ser usado como classe do componente (handlers)
 - `cityOnly` - Recebe `true` ou `false` - Quando `true` exibe a cidade
 - `stateOnly` - Recebe `true` ou `false` - Quando `true` exibe apenas o estado

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-flex#slide": {
  "props": {
    ...
  },
  "children": [
+   "yv-user-localization",
    ...
  ]
},
```

### Visual do Componente
![](https://i.imgur.com/xsLjzyD.png)

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTM5OTk3MTA3Ml19
-->