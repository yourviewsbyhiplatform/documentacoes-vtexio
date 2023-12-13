# Blocos Filhos - Subtítulo

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - `yv-product-questions-and-answers` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20personaliz%C3%A1vel%20-%20Bloco%20de%20perguntas%20e%20respostas.md)
 - `yv-flex` [(documentação)](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Blocos%20Filhos%20-%20Flex%20Box.md)

### Blocos filhos aceitos:

- Nenhum
 
## Usabilidade

### Nome do bloco

O bloco `yv-subtitle`, tem como papel, apresentar um subtítulo dentro do bloco pai.

```diff
"yv-product-questions-and-answers": {
  "children": [
	...
+   "yv-subtitle",
	..
  ]
},
"yv-subtitle": {
  "props": {
    "text": "Tire sua duvida aqui!"
  }
},
```

### Propriedades (props)

O bloco de título pode receber duas propriedades importantes para a personalização, são elas:

 - `text` - Texto que será exibido pelo componente
 - `className` - Texto para ser usado como classe do componente (handlers)

### Exemplo de uso:

```jsonc
// yourviews-custom.jsonc
"yv-testimonials": {
  "props": {
    ...
  },
  "children": [
    "yv-title#testimonial", 
    ...
  ]
},

"yv-title#testimonial": {
  "props": {
    "text": "Avaliações da nossa loja"
    "className": "testimonialsTitle"
  }
},
```

### Visual do Componente
![](https://i.imgur.com/wMSjjIU.png)

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQ3ODE5ODk1MV19
-->