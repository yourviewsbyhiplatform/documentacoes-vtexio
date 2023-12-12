# Blocos Filhos - Imagens do usuário
## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-content-review` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20reviews.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

Nenhum

## Usabilidade

### Nome do bloco

O bloco `yv-review-photo`, tem como papel, retornar as imagens enviadas pelo usuário no momento da avaliação.

### Propriedades (props)

 - `className` - Texto para ser usado como classe do componente (handlers)

### Exemplo de uso:

```diff
// yourviews-custom.jsonc
"yv-flex#review-row-5": {
  "props": {
    ...
  },
+ "children": ["yv-review-photo"]
},
```

### Visual do Componente
![](https://i.imgur.com/yoJzvBQ.png)

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5NzAxMDM2NjNdfQ==
-->