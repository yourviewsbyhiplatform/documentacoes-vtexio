# Instalação padrão - Bloco das estrelas de prateleira
## Requisitos
Antes de prosseguir com a instalação do bloco das estrelas de prateleira, é essencial que você tenha completado alguns passos preliminares fundamentais para garantir uma integração bem-sucedida e eficiente.


 ### Instalação do App Yourviews na Vtex Io

Um dos requisitos obrigatórios é possuir o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:  [https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)

Ao seguir estes passos, você estará preparado para instalar e configurar o bloco na VTEX IO de maneira eficaz, aproveitando ao máximo as funcionalidades oferecidas.
   ## Instalação
   ### Nome do bloco
 Conhecido como `yv-product-rating-inline`. Esse bloco é projetado para mostrar as estrelas de avaliação nas prateleiras ou vitrines do site, oferecendo aos clientes uma visão rápida da popularidade e qualidade dos produtos ainda na fase de navegação inicial. Este recurso é especialmente útil nas páginas onde vários produtos são exibidos, como a página inicial ou categorias de produtos.
 ### Localização do bloco
 Normalmente, o bloco `yv-product-rating-inline` é inserido no bloco pai **product-summary.shelf**. Esta é a configuração padrão para exibir as avaliações nas prateleiras ou vitrines do site, comumente localizadas na página inicial da loja.
 

    “yv-product-rating-inline”
![Instalação do bloco Exemplo](https://yv-misc.s3.us-east-1.amazonaws.com/help/yv-help-docs/76%20-%20productSummary.png)
### Exemplo
```diff
// product-summary.jsonc
"product-summary.shelf": {
      "children": [
         ...
         "flex-layout.col#productRating",
         ...
      ]
},

"flex-layout.col#productRating": {
   "props": {
      "blockClass":  "productRating"
   },
   "children": ["yv-product-rating-inline"]
},
```
### Finalização
**Pronto!**

O bloco das estrelas de prateleira foi instalado com sucesso!
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQ0NDM4NzMwNywtOTUzODIyOTgzXX0=
-->