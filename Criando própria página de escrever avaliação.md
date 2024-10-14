


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
## Segundo passo: Criar rota
O próximo passo é criar uma rota dedicada para a página de "escrever avaliação". Essa rota será adicionada ao arquivo JSON de rotas (```routes.json```) do repositório da loja, permitindo que os clientes acessem a página de avaliação diretamente.
  
![Instalação do bloco Exemplo](https://i.imgur.com/7uVh54i.png)
## Terceiro passo: Envolver o formulário com o header e o footer do seu site


![Instalação do bloco Exemplo](https://i.imgur.com/XwTaPFj.png)
**Pronto!**  
<!--stackedit_data:
eyJoaXN0b3J5IjpbMzYwMzIzNDI1LDEyNzI5NDU1MTRdfQ==
-->