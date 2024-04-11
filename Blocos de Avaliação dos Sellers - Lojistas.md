# Instalação dos blocos de lojista / sellers na VTEX IO

## Requisitos

Existem alguns passos muito importantes a serem seguidos antes de efetuar a inserção dos componentes da yourviews no tema da sua loja.

### Instalação do App Yourviews na Vtex Io

Um dos requisitos obrigatórios é possui o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:
[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)

## Instruções de inserção dos blocos

Este recurso dentro da VTEX tem como função retornar as avaliações resumidas e detalhadas dos lojistas/sellers da VTEX IO.

A Yourviews possui **2 blocos** para exibir as avaliações do lojista: 
o bloco `product-seller-rating-inline`
e o bloco `product-seller-infos`. 

Confira-os detalhadamente a seguir:

<hr>

### Bloco: Estrelas da avaliação média e total do lojista ou seller (`product-seller-rating-inline`)

Geralmente esse bloco se encontra na PDP, acompanhado do nome do lojista e o buy-button, exemplo:
![](https://i.imgur.com/2IcEEmp.png)

#### Inserção do bloco `product-seller-rating-inline`

A Yourviews precisa obter o **Id do Lojista** via `prop` pelo React, sendo assim é necessário ser criado um bloco pelo cliente usando o builder React na VTEX e passar uma propriedade com o  **sellerId**  (visualize nos exemplos abaixo).

Existe também uma documentação da VTEX para ajuda, de como passar uma prop para um componentes, basta  [clicar aqui](https://developers.vtex.com/docs/guides/vtex-io-documentation-composition).
E Também como criar uma um bloco em react na vtex usando o buildar React, para isso [clique aqui](https://developers.vtex.com/docs/guides/vtex-io-documentation-4-declaring-a-theme-block)

Após tudo pronto, poderá seguir o passo a passo abaixo:

##### 1 -  Cria o bloco no React e passa a propriedade sellerId para o componente filho (Estrelas) que é o bloco da yourviews:
**Importante: a propriedade precisa ser exatamente “sellerId”:** e precisa ter o valor que seria o Id do lojista, normalmente sendo um texto ou número

Componente:
```jsx
// LojistaEstrelas.js
const LojistaEstrelas = ({Estrelas}) => {
  const { sellerId } = useLojistaAtual() //obtem o Id do lojista
  return (
    <Estrelas sellerId={sellerId} />
  )
export default LojistaEstrelas
```
![](https://i.imgur.com/2f7OD45.png)
<br>
##### 2 - Adiciona o novo bloco novo nas interfaces do app:
No arquivo `interfaces.json` crie uma nova interface como no exemplo abaixo:
```json
"lojista-estrelas": {
  "component": "LojistaEstrelas",
  "composition": "children"
}
```
![](https://i.imgur.com/9OAOS5Y.png)
<br>
##### 3 -  Insere o novo bloco criado no local desejado, como por exemplo na listagem dos sellers na PDP:
```diff
"linha-infos-lojista": {
  "children": [
+   "lojista-estrelas",
	"lojista-preco",
	"lojista-entrega",
	"buy-button"
  ]
}
```
![](https://i.imgur.com/MzJOJIU.png)
<br>
##### 4 -  Passa como props do bloco criado o bloco da yourviews `product-seller-rating-inline:`
Geralmente essa declaração fica no mesmo arquivo de onde foi inserido o bloco.
```json
"lojista-estrelas":{
  "props": {
    "Estrelas": "product-seller-rating-inline"
  }
}
```
![](https://i.imgur.com/EbwWYYo.png)

<hr>

### Bloco: Estrelas da avaliação detalhada do lojista ou seller (`product-seller-infos`)

O segundo bloco são as notas de cada informação configuradas no formulário da Yourviews:
![](https://i.imgur.com/NUtVC2S.png)

Essas informações e textos são retornadas no bloco de informações do lojista aqui do APP da Yourviews, e a sua inserção é parecida com o bloco anterior, e geralmente esse bloco é inserido na página do lojista, ou via popup por exemplo:
![](https://i.imgur.com/g8RuPib.png)

<hr>

#### Inserção do bloco `product-seller-infos`

Para inserir esse bloco, é necessário que na seção de blocos da seu APP da VTEX seja necessário adicionar o bloco `product-seller-infos` e também segue o mesmo funcionamento do bloco anterior.

### Variações do sellerId para esse bloco

#### Via Querie Parameter
Esse bloco pode receber o sellerId via URL usando **querie paramenter**
Exemplo:
![](https://i.imgur.com/5WY8aiX.png)

**Importante** O querie parameter deve ser exatamente `sellerId`

Usando a querie paramenter, basta inserir o bloco no children da página que ele será carregado automáticamente.

Exemplo:
```diff
"store.custom#seller": {
    "blocks": [
      ...
+     "product-seller-infos",
      ...
    ]
  },
```

<hr>

#### Via prop
Para isso é necessário a criação de um bloco pelo cliente usando o builder React na VTEX passando uma propriedade com o sellerId, como nos exemplos abaixo:  
Existe uma documentação da VTEX para ajuda aqui: [https://developers.vtex.com/docs/guides/vtex-io-documentation-composition](https://developers.vtex.com/docs/guides/vtex-io-documentation-composition)

Exemplo: 
![](https://i.imgur.com/Buu4rzS.png)

O segundo componente onde será exibido as avaliações detalhadas do seller, pode ser dentro de um **popup** ou então em uma **nova pagina** que seria a pagina do próprio Lojista/Seller

#### Segue abaixo o passo a passo de exemplo:

##### 1 -  Cria a pagina ou popup no React e passa a propriedade sellerId para o componente filho (SellerInfos) que é o bloco da Yourviews :
Exemplo:
```jsx
const SellerPopup = ({ SellerInfos }) => {
  const { sellerId } = useLojistaAtual() //obtem o Id do lojista
  return (
    <>
      ...
      <SellerInfos sellerId={sellerId} />
      ...
    </>
  );
};
```
**Importante: a propriedade precisa ser exatamente “sellerId”** 
O sellerId precisa ter o valor que seria o Id do lojista, normalmente sendo um texto ou número
<br>

##### 2 - Adiciona o bloco novo nas interfaces da loja:
No arquivo `interfaces.json` crie uma nova interface como no exemplo abaixo:
```json
"seller-popup": {
  "component": "SellerPopup",
  "composition": "children"
}
```
<br>

##### 3 - Insere o novo bloco criado no local desejado:
Exemplo:
```diff
"seller-row": {
  "children": [
+   "seller-popup",
    "seller-price",
    "seller-shipping",
    "buy-button"
  ]
},
```
<br>

##### 4 - Passa como props do bloco criado o bloco da yourviews `product-seller-infos`:

Exemplo:
```json
"seller-popup": {
  "props": {
    "SellerInfos": "product-seller-infos"
  }
},
```
<br>

<br>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwODE4OTUxNjBdfQ==
-->