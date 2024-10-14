


# Como criar sua própria página de Write Review na VTEXIO
  
## Primeiro Passo: Criação do JSON do Bloco de Formulário

O primeiro passo para integrar o bloco de formulário no repositório da loja do cliente é criar o arquivo JSON que servirá como estrutura do formulário.
![Instalação do bloco Exemplo](https://i.imgur.com/4Trl5pf.png)

### Estrutura do JSON
Certifique-se de seguir a estrutura abaixo como exemplo:

```json
{
	"store.custom#write-review": {
		"blocks": [
			"yv-product-review-form",
		]
	},
}

```
Isso garantirá que o formulário será carregado.
## Primeiro Passo: Criação do JSON do Bloco de Formulário

  

## Requisitos  

Existem alguns passos muito importantes a serem seguidos antes de efetuar a inserção dos componentes da yourviews no tema da sua loja.    

### Instalação do App Yourviews na Vtex Io  
  
Um dos requisitos obrigatórios é possuir o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:  
[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)  
  

## Instruções

### Como identificar
Para poder saber se o modo debug está ativo ou não em sua loja, abrir uma nova aba em seu navegador com a url da sua loja seja em produção ou em um workspace da vtex, mas que possua o app instalado, com a aba aberta e o conteúdo carregado, abra as ferramentas de desenvolvedor (DevTools) normalmente utilizando a tecla F12, após isso, aba o `console`, como no exemplo abaixo:

![](https://i.imgur.com/J6q4aX3.png)

### Como ver os elementos quando ativo

Caso o modo debug esteja ativo, basta inserir o parâmetro `yv-debug=true` no fim da URL, que os elementos passarão a serem exibidos como no exemplo abaixo:

![](https://i.imgur.com/mRUDiiT.png)

### Solicitar a ativação/desativação do modo debug

Para alterar o modo, quando vem diretamente dos servidores da yourviews, caso deseje desativar esse modo para que não seja necessário o parâmetro na URL para exibir os elementos ou vice-versa, basta encaminhar um email para o suporte da Hi Platform solicitando a alteração do modo debug.

servicedesk@hiplatform.com

<hr>  
<br>  
  

**Pronto!**  
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc3ODQ3NTU4NSwxMjcyOTQ1NTE0XX0=
-->