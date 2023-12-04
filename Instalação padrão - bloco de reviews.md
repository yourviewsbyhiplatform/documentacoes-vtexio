# Instalação padrão - Bloco de reviews
## Requisitos
Antes de prosseguir com a instalação do bloco de reviews, é essencial que você tenha completado alguns passos preliminares fundamentais para garantir uma integração bem-sucedida e eficiente.


 ### Instalação do App Yourviews na Vtex Io

Um dos requisitos obrigatórios é possuir o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:  [https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)

Ao seguir estes passos, você estará preparado para instalar e configurar o bloco na VTEX IO de maneira eficaz, aproveitando ao máximo as funcionalidades oferecidas.

 ## Instalação
   ### Nome do bloco
   O bloco é identificado como `yv-product-reviews`. Ele é projetado para exibir as avaliações e comentários dos clientes sobre produtos específicos. Este bloco é particularmente valioso nas páginas de produtos, onde os clientes podem ler as opiniões e experiências de outros compradores antes de tomar uma decisão de compra.
   ### Localização do bloco
   O bloco `yv-product-reviews` é normalmente posicionado no bloco pai **store.product**, que corresponde à página de cada produto individual. Este posicionamento permite que as avaliações dos clientes estejam diretamente associadas ao produto relevante.
   

    "yv-product-reviews"
    
![Instalação do bloco Exemplo](https://imgur.com/FlrF78A.png)
### Exemplo
```diff
// product.jsonc
"store.product": {
    "children": [
       ...
       "yv-product-reviews",
       ...
    ]
  },
```
### Finalização
**Pronto!**

O bloco de perguntas e respostas foi instalado com sucesso!
![Instalação do bloco Exemplo](https://imgur.com/OI83A3S.png)
![Instalação do bloco Exemplo](https://imgur.com/1Bmza3V.png)
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEwMjkyODAzODhdfQ==
-->