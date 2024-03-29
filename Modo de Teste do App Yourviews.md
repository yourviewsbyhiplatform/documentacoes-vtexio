# Modo de Testes do App Yourviews (DEBUG)
  
No processo de instalação da sua loja, ou quando necessário, é possível solicitar ao time de suporte da Hi Platform para ativar ou desativar o modo de testes da sua loja yourviews, isso faz com que o app da vtexio não apresente nenhum elemento sem antes passar um parâmentro da URL.

Pode ser muito útil em diversas ocasiões.

Usamos esse modo para evitar que os elementos sejam exibidos de maneira quebrada enquanto a loja personaliza os elementos mesmo que o app esteja instalado em produção.
  

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
eyJoaXN0b3J5IjpbMTkwNzgwNzA5OF19
-->