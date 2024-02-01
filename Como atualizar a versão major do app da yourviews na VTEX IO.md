# Como atualizar a versão major do app da yourviews na VTEX IO

É importante sempre manter o app da yourviews atualizado em sua loja, recomendamos que seja mantido o app na versão major atualizada onde há diversas novas funcionalidades no app.

## Requisitos

Existem alguns passos muito importantes a serem seguidos antes de efetuar a inserção dos componentes da yourviews no tema da sua loja.

### Instalação do App Yourviews na Vtex Io

Um dos requisitos obrigatórios é possuir o app da yourviews instalado na sua loja vtexio, para isso, acesse o link abaixo para seguir com o passo a passo de instalação:
[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md](https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instalac%CC%A7a%CC%83o%20do%20App%20Yourviews%20na%20Vtex%20Io.md)

Outro requisito importantíssimo é possuir o CLI da vtex instalado em sua máquina: [https://developers.vtex.com/docs/guides/vtex-io-documentation-vtex-io-cli-install](https://developers.vtex.com/docs/guides/vtex-io-documentation-vtex-io-cli-install)

## Instruções para executar a atualização da versão major

Atualmente existem dois modelos de inserção dos blocos da yourviews, o modelo padrão, onde os blocos pais são inseridos normalmente e esses blocos renderizam os elementos da yourviews de acordo com o template/layout escolhido no processo de onboarding da hiplatform, e também o modelo personalizável, onde cada bloco pai, pode receber alguns blocos filhos que compõem o elemento, assim, podendo personalizar a sua estruturada para uma personalização mais elaborada.


### Passo a Passo

Antes de iniciar esse processo, saiba que é um processo delicado e pode ser um pouco cansativo. Faça com calma e atenção. Serão diversos passos a serem seguidos.

Com o repositório do tema da sua loja aberto e o CLI da vtex aberto na pasta raiz do projeto, siga os passos abaixo:	

**1 -** Crie um novo workspace de dev usando o comando `vtex use {nome}`

**1.1 -** Usando o comando `vtex ls` será possível ver alguns app já instalados

**1.2 -** Desinstale o app da Yourviews com a versão major antiga usando o comando `vtex uninstall yourviews.yourviewsreviews`

**1.3 -** Desinstale o app do tema da sua loja usando o comando `vtex uninstall {minhaloja.store-theme}`

**2 -** Altere o arquivo manifest.json do app tema da sua loja mudando as peerDependencies do app da Yourviews para a nova versão major, por exemplo:
```json
"peerDependencies": {
	"yourviews.yourviewsreviews": "1.x"
```

**3 -** **Atenção**: Caso você esteja saindo da  versão major “0.x” para uma maior como por exemplo “1.x” altere os nomes do blocos antigos inserido apenas um “yv-” antes dos mesmos nomes, exemplo:
-   testimonials  ->  `yv-testimonials`
-   product-reviews  ->  `yv-product-reviews`
-   product-questions-and-answers  ->  `yv-product-questions-and-answers`
-   product-rating-summary  ->  `yv-product-rating-summary`
-   product-rating-inline  ->  `yv-product-rating-inline`

Essa alteração nos nomes irá evitar que haja conflito com o app “vtex.reviews-and-ratings” e também lhe dará a possibilidade de personalizar os blocos da Yourviews na Vtex, basta seguir os exemplos e instruções passadas abaixo:
[https://github.com/yourviewsbyhiplatform/documentacoes/blob/master/Instala%C3%A7%C3%A3o%20dos%20blocos.md](https://github.com/luisfkandriolohi/vtexio-yourviews-store-theme-custom)

**4 -** Instale a nova versão do app da Yourviews executando o comando: `vtex install yourviews.yourviewsreviews`

**5 -** Verifique se a nova versão foi instalada usando o comando `vtex ls`

**6 -** Execute o comando `vtex link` com as devidas alterações no app do tema da sua loja

**6.1 -** Apos o link, nesse novo workspace criado, será necessário ir ate a pagina `....myvtex.com/admin/apps` e configurar o app da Yourviews novamente com as chaves necessárias de login e senha que é disponibilizado no painel da yourviews da sua loja, na seguinte url: [https://service.yourviews.com.br/admin/Account/StoreApi](https://service.yourviews.com.br/admin/Account/StoreApi)

**7 -** Verifique se está tudo certo no workspace usando o comando ”vtex browse”

**8 -** Após tudo verificado e validado, salve as alterações e suba um commit no seu repositório git (a Vtex obriga esse passo)

**9 -** Execute o comando para o release de uma nova versão major do app do tema da sua loja, sendo ele: `vtex release major stable` (A Vtex obriga que seja uma versão major devido a alteração do manifet.json no qual alteramos a versão major do app da Yourviews nas peerDependencies)

**10 -** Aguarde o release e execute o comando de deploy `vtex deploy {minhaloja-store-theme}`

**11 -** Crie um novo workspace, agora de produção usando o comando `vtex use {nome} –production`

**11.1 -** Usando o comando `vtex ls` será possível ver alguns app já instalados

**11.2 -** Desinstale o app da **Yourviews** com a versão major antiga usando o comando `vtex uninstall yourviews.yourviewsreviews`

**11.3 -** Desinstale o **app antigo do tema da sua loja** usando o comando `vtex uninstall {minhaloja.store-theme}`

**11.4 -** Instale a nova versão do app da **Yourviews** executando o comando: `vtex install yourviews.yourviewsreviews`

**11.5 -** Instale a nova versão do **app do tema da sua** loja executando o comando: `vtex install {minhaloja.store-theme}`

**11.6 -** Execute o comando `vtex ls` e verifique se as versões dos apps estão todas atualizadas

**12 -** Nesse novo workspace de produção criado, será necessário ir ate a pagina _`....myvtex.com/admin/apps`_ e configurar o app da Yourviews novamente com as chaves necessárias de login e senha que é disponibilizado no painel da Yourviews da sua loja, na seguinte url: [https://service.yourviews.com.br/admin/Account/StoreApi](https://service.yourviews.com.br/admin/Account/StoreApi)

**13 -** Estando tudo atualizado, use o comando `vtex browse` e verifique se tudo está correto no ambiente.

**14 -** Após a verificação, execute o comando `vtex promote` e aguarde!

**15 -** Após o promote, o repositório atual de produção será removido pela Vtex e as devidas alterações já estarão no ambiente de produção / workspace master.

**16 -** Após todo o processo concluído é necessário seguir um passo a passo passado pela VTEX quando é feita uma atualização major do app tema da loja: [https://developers.vtex.com/docs/guides/vtex-io-documentation-migrating-cms-settings-after-major-update](https://developers.vtex.com/docs/guides/vtex-io-documentation-migrating-cms-settings-after-major-update)

<hr>
<br>

**Pronto!**
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTYzMDc5NzI4OV19
-->