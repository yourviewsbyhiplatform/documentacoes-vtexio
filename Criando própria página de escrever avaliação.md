


# Como criar sua própria página de Write Review na VTEXIO


Nosso aplicativo da YourViews na VTEX IO já cria automaticamente um formulário padrão na rota ```new-review```. No entanto, alguns clientes utilizam header e footer personalizados, o que pode resultar na não exibição correta desse formulário.

Para resolver essa questão, o cliente tem a opção de criar uma nova rota de formulário, vinculando-a ao bloco fornecido pela YourViews. Isso garante que o formulário será exibido corretamente, respeitando os elementos de customização aplicados no header e footer do cliente.
  
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
## Segundo passo: Criar rota
O próximo passo é criar uma rota dedicada para a página de "escrever avaliação". Essa rota será adicionada ao arquivo JSON de rotas (```routes.json```) do repositório da loja, permitindo que os clientes acessem a página de avaliação diretamente.
  
![Instalação do bloco Exemplo](https://i.imgur.com/7uVh54i.png)
## Terceiro passo: Envolver o Formulário com o Header e o Footer

Para tornar o formulário mais atrativo e consistente com o visual do site, o cliente pode envolver o formulário com o header e o footer do próprio site. Isso permitirá que o formulário se integre de forma mais harmônica ao layout existente.

####  Como Fazer
Para envolver o formulário com o header e o footer, o cliente deve abrir novamente o arquivo JSON do bloco do formulário (```write-review.json```) e fazer o seguinte:

1. Localize o JSON do formulário já criado.
2. Envolva o conteúdo do formulário com os blocos correspondentes ao header e ao footer da loja.


![Instalação do bloco Exemplo](https://i.imgur.com/XwTaPFj.png)

### Por fim, temos o resultado
![Instalação do bloco Exemplo](https://i.imgur.com/UM4XNu7.png)
**Pronto!**  
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwNjY5NzMyNTcsLTE3Mzg3ODUwODksMz
YwMzIzNDI1LDEyNzI5NDU1MTRdfQ==
-->