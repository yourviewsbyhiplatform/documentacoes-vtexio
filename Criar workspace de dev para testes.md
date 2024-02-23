# Criar workspace de dev para testes

Quando ocorrem certos problemas, bugs durante a instalação, é recomendado que a loja crie um workspace (ambiente) de desenvolvimento dentro da vtex io para que a Yourviews possa efetuar os testes corretamente e identificar o problema.

## Requisitos

Existem alguns passos muito importantes a serem seguidos para que a criação do ambiente seja feito corretamente.

### Liberação dos acessos
Um passo muito importante é efetuar a liberação de acessos para a hiplatform/yourviews, para isso acesse o link abaixo:

[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Libera%C3%A7%C3%A3o%20de%20Acessos.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Libera%C3%A7%C3%A3o%20de%20Acessos.md)

### Instalação do CLI da VTEX IO
Antes de tudo, é importante ressaltar que é necessário possuir o CLI da VTEX IO instalado e atualizado em sua máquina, para instalar o CLI da VTEX IO, acesse o link abaixo:

[https://developers.vtex.com/docs/guides/vtex-io-documentation-vtex-io-cli-install](https://developers.vtex.com/docs/guides/vtex-io-documentation-vtex-io-cli-install)

## Passo a Passo

Para criar o workspace de desenvolvimento interno na vtex io, basta usar o terminal de comandos do seu computador e executar os comandos abaixo:

Primeiramente efetuar o login na sua loja, com o comando `vtex login`, será exibir a confirmação de login e aberto uma aba no navegador para efetuar o login com sua conta.

Após o login efetuado, será necessário executar o comando `vtex workspace ls` para listar todos os ambientes já criados.
Verifique na lista se já existe um workspace chamado `yourviews` criado, caso já exista, remova o mesmo usando o comando `vtex workspace delete {nome_do_workspace}` caso seja possível, e crie novamente o mesmo workspace usando o comando `vtex use yourviews`

ou 

Crie um novo workspace chamado `yourviewstest` usando o comando `vtex use yourviewstest`

Exemplo:
![](https://i.imgur.com/8M4iHbg.png)

Após a criação do workspace:

Insira novamente todos os elementos e blocos da yourviews e instale corretamente o app da Yourviews apenas neste workspace de desenvolvimento.

Use o comando `vtex browse` para que uma aba no navegador seja aberta e copie a URL desse ambiente que será normalmente o nome 
`{nome_do_workspace}--{nome_da_loja}.myvtex.com`
e envie para a equipe de suporte da HiPlatform / Yourviews para que possamos fazer os devidos testes e análises dos devidos erros que possam estar ocorrendo.

### Finalização

**Pronto!**

O acesso para a yourviews está pronto junto com o workspace para testes
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTM3NTc1NzYyOF19
-->