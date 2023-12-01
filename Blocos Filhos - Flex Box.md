# Blocos Filhos - Flex Box

## Importante

Para utilizar esse bloco, é necessário verificar se o bloco pai a ser usado pode receber esse bloco como filho e quais são seus blocos filhos aceitos!

### Blocos pais aceitos:

 - Qualquer um

### Blocos filhos aceitos:

Os blocos filhos aceitos desse bloco serão os mesmos blocos filhos aceitos pelo bloco pai.

Exemplo: Se o `yv-flex` estiver como filho do `yv-testimonials`, então o `yv-flex` irá aceitar apenas os filhos do próprio `yv-testimonials`
 
 
## Usabilidade

### Nome do bloco

O bloco `yv-flex`, tem como papel, apenas englobar os blocos filhos e aumentar a possiblidade de personalização usando as propriedades flex do CSS.

### Propriedades (props)

O bloco de flex box pode receber diversas propriedades importantes para a personalização, são elas:

 - `className` - Texto para ser usado como classe do componente (handlers)
 - `direction` - Texto `row` ou `column` para apresentar o conteúdo interno em linha ou coluna respectivamente
 - `wrap` - Texto `wrap` ou `nowrap` para quebrar em mais de uma linha o conteúdo
 - `justifyContent` - Texto `center` | `flex-start` | `flex-end` | `space-between` | `space-around` | `space-evenly` para definir a posição e o espaçamento do conteúdo interno
 - `alignItems` - Texto `center` | `flex-start` | `flex-end` | `space-between` | `space-around` | `space-evenly` para definir a posição e o espaçamento do conteúdo interno
 - `alignContent` - Texto `center` | `flex-start` | `flex-end` | `space-between` | `space-around` | `stretch` para definir a posição e o espaçamento do conteúdo interno
 - `width` - Texto com o valor da largura do bloco
 - `height` - Texto com o valor da altura do bloco
 - `marginTop` - Texto com o valor margem superior do bloco
 - `marginBottom` - Texto com o valor margem inferior do bloco
 - `marginLeft` - Texto com o valor margem da esquerda do bloco
 - `marginRight` - Texto com o valor margem da direita do bloco
 - `paddingTop` - Texto com o valor margem interna do bloco
 - `paddingBottom` - Texto com o valor margem inferior do bloco
 - `paddingLeft` - Texto com o valor margem da esquerda do bloco
 - `paddingRight` - Texto com o valor margem da direita do bloco

### Exemplo de uso:

```jsonc
// yourviews-custom.jsonc
"yv-testimonials-content": {
  "children": ["yv-flex#slide"]
},
"yv-flex#slide": {
  "props": {
    "className": "testimonial-flex"
  },
  "children": [
    "yv-rating-stars",
    "yv-date",
    "yv-user-image",
    "yv-user-name#testimonial",
    "yv-user-localization#testimonial",
    "yv-comment",
    "yv-store-ratings"
  ]
},
```
```css
/* yourviews.yourviewsreviews.css */
.testimonial-flex {
  flex-direction: column;
  align-items: center;
  border-radius: 5px;
  padding: 20px;
  box-shadow: 1px 1px 10px -4px #000;
  margin: 10px;
  width: 100%;
  min-height: 232px;
}
```

<br>
<br>

**Pronto!**

<!--stackedit_data:
eyJoaXN0b3J5IjpbMzUxNzE4MzY1XX0=
-->