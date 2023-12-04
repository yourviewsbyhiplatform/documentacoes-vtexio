# Instalação padrão - Bloco das estrelas de ancoragem
## Requisitos
Antes de prosseguir com a instalação do bloco das estrelas de produto, é essencial que você tenha completado alguns passos preliminares fundamentais para garantir uma integração bem-sucedida e eficiente.
 ### Instalação do App Yourviews na Vtex Io

Um dos requisitos obrigatórios é possuir o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:  [https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)

Ao seguir estes passos, você estará preparado para instalar e configurar o bloco na VTEX IO de maneira eficaz, aproveitando ao máximo as funcionalidades oferecidas.
  ## Instalação
   ### Nome do bloco
Conhecido como `yv-product-rating-summary`. Esse bloco é essencial para exibir um resumo das avaliações de produtos em forma de estrelas, uma ferramenta chave para impulsionar a confiança e auxiliar na decisão de compra dos clientes. O bloco é comumente posicionado na página de cada produto, oferecendo uma visão rápida e clara das avaliações que o produto recebeu.
### Localização do bloco
O bloco `yv-product-rating-summary` é normalmente inserido no bloco pai **store.product**, que corresponde à página de cada produto. Esta localização estratégica permite que os clientes vejam rapidamente a avaliação do produto em questão.

    "yv-product-rating-summary"

![Instalação do bloco Exemplo](https://i.imgur.com/48VoM5p.png)
### Exemplo
```diff
// product.jsonc
"flex-layout.col#right-col": {
   "children": [
      ...
      "yv-product-rating-summary",
      ...
   ]
}, 
```

### Finalização
**Pronto!**

O bloco das estrelas âncora foi instalado com sucesso!
![Instalação do bloco Exemplo](https://i.imgur.com/Qhazjwz.png)

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTI2NDI5NzA4M119
-->
