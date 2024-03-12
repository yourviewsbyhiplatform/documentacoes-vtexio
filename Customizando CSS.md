# Customizando CSS

## Requisitos

Existem alguns passos muito importantes a serem seguidos para que a customização do elementos da Yourviews seja feita da maneira correta!

### Instalação do App Yourviews na Vtex Io

Um dos requisitos obrigatórios é possui o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:
[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)

## Instruções

Para poder editar o css das classes da app da Yourviews, a yourviews usa o CSS_HANDLES que a própria Vtex disponibiliza, e nesse caso precisamos descobrir qual bloco e classe queremos editar:

### Passo 0 - Acessar ambiente em modo inspect

Acesse o workspace desejado e na URL da página desejada, basta inserir uma **consulta** da VTEX de inspecionar

**Query:** `?__inspect`

**Exemplo:**  [https://workspacedev-minhaloja.myvtex.com/produto-x/p?__inspect](https://workspacedev-minhaloja.myvtex.com/produto-x/p?__inspect)

Help de ajuda da VTEX: [https://developers.vtex.com/docs/guides/how-to-interactively-inspect-blocks-on-a-store-framework-store](https://developers.vtex.com/docs/guides/how-to-interactively-inspect-blocks-on-a-store-framework-store)

Usando esse método, será possível passar o mouse sobre os componentes da loja e visualizar seus blocos e classes como no exemplo abaixo:

![](https://i.imgur.com/lmcFMDc.png)

É possível notar que as estrelas estão atribuídas à classe `.ratingStarsActive`

### Passo 1 - Personalizando as estrelas de forma exemplar

#### Passo 1

Criar o arquivo css, dentro da pasta `styles` da sua loja usando o nome `yourviews.yourviewsreviews.css`
![](https://i.imgur.com/jkSEV3s.png)

#### Passo 2
Criar a classe css e atribuir a propriedade `fill` como no exemplo abaixo:
![](https://i.imgur.com/poeVTo6.png)

#### Passo 3
Salve o arquivo e execute o comando `vtex link` para que essa alteração reflita no workspace.
![](https://i.imgur.com/LgJTwDp.png)

### Finalização

**Pronto!**

Agora a personalização do tema dos blocos da yourviews está finalizada ao seu gosto como desejar.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTY1MDkxODkxMV19
-->