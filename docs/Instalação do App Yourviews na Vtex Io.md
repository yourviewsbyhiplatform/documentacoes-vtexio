# Instalação do App Yourviews na Vtex Io

## Requisitos

Existem alguns passos muito importantes a serem seguidos para que a instalação do aplicativo da Yourviews seja executada da maneira correta!

### Liberação dos acessos
Um passo muito importante é efetuar a liberação de acessos para a hiplatform/yourviews, para isso acesse o link abaixo:

[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/docs/Libera%C3%A7%C3%A3o%20de%20Acessos.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/docs/Libera%C3%A7%C3%A3o%20de%20Acessos.md)

### Instalação do CLI da VTEX IO
Antes de tudo, é importante ressaltar que é necessário possuir o CLI da VTEX IO instalado e atualizado em sua máquina, para instalar o CLI da VTEX IO, acesse o link abaixo:

[https://developers.vtex.com/docs/guides/vtex-io-documentation-vtex-io-cli-install](https://developers.vtex.com/docs/guides/vtex-io-documentation-vtex-io-cli-install)

## Passo a Passo

### Passo 0 - Login

Antes de tudo precisamos fazer o login na sua conta da vtex usando o CLI da vtex que instalamos, para isso, temos que executar o seguinte comando no terminal / cmd
```
vtex use {sua_conta}
```
Após executar o comando acima, o seu navegador será aberto solicitando que você adicione seu email e senha da sua conta da vtex para que o login seja efetuado com sucesso.

Exemplo do comando: 
![Vtex CLI Login Exemplo](https://i.imgur.com/cXgewp9.png)

### Passo 1 - Criando workspace de desenvolvimento

Para continuar com a instalação do app da yourviews na sua loja, recomendamos que seja criado um novo workspace da vtex (ambiente de desenvolvimento interno) para depois movermos isso para produção.

Para isso, no terminal, e execute o comando abaixo:
```
vtex use {nome_do_workspace}
```
Após executar o comando acima, o CLI da vtex irá verificar se esse workspace já não existe, caso não exista, irá perguntar se deseja criar um novo, para isso, devemos digitar "y" para confirmar a criação do workspace.
Caso já exista, a vtex apenas irá mudar automaticamente para esse workspace existente. Recomendamos que seja usado um workspace novo. Quando criamos um novo workspace, a vtex faz uma cópia do workspace master que seria o de produção.

Exemplo do comando: 
![VTEX CLI Novo workspace exemplo](https://i.imgur.com/WM5vY4L.png)

### Passo 2 - Instalado o app da yourviews

Para instalar o app da yourviews na VTEX IO no workspace que você acabou de criar, basta executar o comando abaixo:
```
vtex install yourviews.yourviewsreviews
```
Exemplo:
![Vtex CLI exemplo install](https://i.imgur.com/O1oqbyF.png)

### Passo 3 - Adicionando a dependência do app da yourviews no arquivo manifest.json

Nesse passo, será necessário acessarmos a pasta raiz do repositório onde ficam os arquivos do aplicativo do tema da sua loja, e editar o arquivo manifest.json, exemplo:

![Print pasta raiz do app tema da loja](https://i.imgur.com/uJWhHD7.png)

Dentro do arquivo manifest.json, devemos procurar pela seção `peerDependencies`, caso não possua, criá-la, e adicionar a dependência do app da yourviews no tema da sua loja, como no código abaixo
```
"peerDependencies": {
	"yourviews.yourviewsreviews":  "1.x"
},
```

Exemplo:
![Exemplo peerDependencies](https://i.imgur.com/Kws4pcT.png)

### Passo 4 - Configurando o app da yourviews

É necessário configurar o app da yourviews com as chaves da sua conta da yourviews, que ficam em nosso painel, para isso, primeiro acesse o painel da yourviews, na seção das informações de código da loja:
Link: [https://service.yourviews.com.br/admin/Account/StoreApi](https://service.yourviews.com.br/admin/Account/StoreApi) 

Salve o código, usuário e senha da sua loja: 
![enter image description here](https://i.imgur.com/SLdMp8q.png)

Agora, acesse o painel administrativo dos apps da vtex:
Link: [https://{sualoja}.myvtex.com/admin/apps](https://%7Bsualoja%7D.myvtex.com/admin/apps)
E procure pelo app da yourviews:
![](https://i.imgur.com/7ThmLS2.png)

Clique em "configurações" e adicione as respectivas chaves que você salvou, exemplo:
![](https://i.imgur.com/QBRZyXy.png)

Habilite ou não a geração de dados estruturados de aggregateRating e review para o Google Search Console, escolha a linguagem do app, e clique em salvar. 

### Finalização

**Pronto!**

O Aplicativo da yourviews está instalado no seu workspace com sucesso.

**Mas calma!**

Agora o próximo passo é inserir cada elemento / bloco dentro do código do tema da sua loja, para que os componentes de avaliações, estrelinhas, perguntas e etc sejam exibidos em seu site.
Para isso, [clique aqui](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/docs/Libera%C3%A7%C3%A3o%20de%20Acessos.md), o passo a passo de como inserir cada elemento no tema da sua loja.
