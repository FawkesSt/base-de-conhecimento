# Integração Paypal – Cursos (EAD)

Objetivo: mostrar como configurar a integração PayPal e leadlovers.\
Para que serve: essa integração realiza a ponte entre PayPal e leadlovers, para que quando houver uma compra no PayPal o cliente entre como aluno em seu produto EAD na leadlovers.\
Requisito(s) obrigatório(s): 1. Ter uma conta no [PayPal](https://paypal.com/) do tipo Empresa. 2. Possuir um [produto EAD](https://suporte.love/como-criar-um-produto/) criado na leadlovers.

Neste tutorial, te ensinaremos como fazer uma integração entre a plataforma PayPal, especializada em vendas, e o produto EAD da leadlovers. Com ela, você pode liberar um acesso à área de membros na leadlovers para os clientes que realizarem a compra do seu produto. Caso queira integrar o PayPal apenas com as suas máquinas aqui da leadlovers, pode fazer por meio do [Produto Integração](https://suporte.love/produto-integracao-com-produtos-externos-versao-4-0/).

### Trocando informações entre leadlovers e Paypal <a href="#trocando-informacoes" id="trocando-informacoes"></a>

Essa integração possui uma rotatividade entre configurações na leadlovers e no PayPal, é bacana deixar ambos abertos em abas separadas enquanto segue o tutorial. Antes de cada passo iremos dizer em qual plataforma é feito. Essa troca de informações é necessária para que a integração entre leadlovers e Paypal funcione.

Nº1–  No PayPal, clique na engrenagem no canto superior direito.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem1.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem1.png)

Nº2– Copie o **“**e-mail da conta”, é muito importante para a integração.

Nº3– Pegue também o **“**ID do vendedo**r”.** Sugerimos que salve ambos em um bloco de notas.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem2.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem2.png)

![⚠](https://s.w.org/images/core/emoji/13.0.0/svg/26a0.svg) **ATENÇÃO:**\


– Neste tutorial, iremos orientar como fazer as configurações na [Antiga](broken-reference) e na[ Nova Área de Produtos](broken-reference). A partir daqui, siga os passos de acordo com a área do Produto EAD que costuma utilizar.&#x20;

#### Antiga Área de Produtos <a href="#antiga-area" id="antiga-area"></a>

Nº4– Voltando para a leadlovers, acesse o produto em que fará a integração e vá até a aba **“**Integrações”.

Nº5– Localize a seção **“**Integração com o PayPal”. Iremos utilizar aqui os dados coletados anteriormente.

Nº6– Em **“**E-mail da sua conta do PayPal” cole o e-mail que copiamos no [passo 2](broken-reference).

Nº7– No campo **“**ID Conta do Comerciante” insira o ID do vendedor que foi apanhado no [passo 3](broken-reference) deste tutorial.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem3.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem3.png)

Nº8– Lembre-se de sempre salvar as configurações. Role toda a página para baixo e clique em **“**Salvar as Integrações”.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem4.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem4.png)

Nº9– Ainda em seu produto leadlovers, após salvar as configurações volte para a aba **“**Integrações”.

Nº10– Novamente localize a seção **“**Integrações com o PayPal”.

Nº11– Pegue a URL de notificação:

https://machine.leadlovers.com/payment/paypal.

Nº12– Copie o **“**ID do Produto ou Assinatura” e guarde-o, pois precisaremos informá-lo no PayPal. Siga agora para a etapa [Voltando ao PayPal](broken-reference).&#x20;

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem5.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem5.png)

#### Nova Área de Produtos <a href="#nova-area" id="nova-area"></a>

Nº4– Na Nova Área de Produtos da leadlovers, acesse o que deseja fazer a integração e vá até a aba **“**Integrações”.

Nº5– Localize o menu **“**PayPal”. Iremos utilizar aqui os dados coletados anteriormente.

Nº6– Em **“**E-mail da sua conta do PayPal” cole o e-mail que copiamos no [passo 2](broken-reference).

Nº7– No campo **“**ID Conta do Comerciante” insira o ID do vendedor que foi apanhado no [passo 3](broken-reference) deste tutorial.

Nº8– Lembre-se de sempre salvar as configurações.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem6.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem6.png)

Nº9– Ainda em seu produto leadlovers, após salvar as configurações volte para a aba **“**Integrações”.

Nº10– Novamente localize a seção **“**PayPal”.

Nº11– Pegue a URL de notificação:

https://machine.leadlovers.com/payment/paypal

Para isso, basta clicar no ícone indicado na imagem abaixo.

Nº12– Copie o **“**ID do Produto ou Assinatura” e guarde-o, pois precisaremos informá-lo no PayPal. Siga agora para a etapa [Voltando ao PayPal](broken-reference).&#x20;

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem7.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem7.png)

#### Voltando ao PayPal <a href="#voltando-paypal" id="voltando-paypal"></a>

Nº13– Novamente no PayPal, clique na engrenagem no canto superior direito da tela.

Nº14– Agora acesse a aba **“**Ferramentas do Vendedor”.

Nº15– Na seção **“**Notificações instantâneas de pagamento” iremos atualizar os dados.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem8.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem8.png)

Nº16– Feito isso, você será redirecionado para a tela **“**Notificação Instantânea de Pagamento (NIP)”. Clique no botão **“**Escolher configurações de NIP”.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem9.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem9.png)

Nº17– Aqui iremos informar a URL de notificação, aquela que pegamos na leadlovers no [passo 11](broken-reference).

Nº18– É muito importante marcar a opção **“**Receber mensagens de NIP (ativado)”.

Nº19– Salve as configurações.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem10.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem10.png)

Após salvar, a sua tela aparecerá assim:

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem11.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem11.png)

Observação: para voltar para a página principal da plataforma, basta clicar na logo do PayPal no canto esquerdo superior da tela.

### Gerando o botão de pagamento no Paypal <a href="#gerando-botao" id="gerando-botao"></a>

A segunda etapa é gerar o botão de vendas de seu produto. Ele poderá ser usado em formato de link clicável ou botão que pode ser inserido via HTML em páginas, criadas na leadlovers ou não.

Agora iremos realizar configurações somente no PayPal.

Nº20– Na tela inicial do PayPal, clique na engrenagem no canto superior direito da tela.

Nº21– Acesse novamente a aba **“**Ferramentas do Vendedor”.

Nº22– Na seção **“**Botões do PayPal”, clique em **“**Gerenciar”.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem12.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem12.png)

Nº23– Selecione o botão que deseja inserir na sua página de acordo com a sua estratégia. Por enquanto, é possível integrar os botões **“**Comprar agora”, **“**Adicionar ao carrinho” e **“**Assinar”.&#x20;

Observação: ao usar o botão **“**Adicionar ao carrinho”, será possível que o cliente adicione mais de uma vez o mesmo produto no carrinho, mas isso irá gerar apenas um aluno no produto EAD porque a compra será feita com um único e-mail. Certifique-se de utilizar essa opção apenas se ela fizer sentido para a sua estratégia.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem13.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem13.png)

Nº24– No nosso exemplo, iremos configurar o botão **“**Comprar Agora”, mas você pode seguir essas mesmas etapas no botão de sua preferência, desde que seja um dos mencionados no [passo 23](broken-reference) deste tutorial.&#x20;

Nº25– Escolha um nome para o produto. Sugerimos utilizar o do Produto EAD leadlovers, pois facilita a segmentação e é o mesmo que aparecerá para o cliente no momento do checkout.

Nº26– Cole o **“ID do produto”** copiado na leadlovers no **passo 12** (da [Antiga ](broken-reference)ou da [Nova Área de Produtos](broken-reference)) deste tutorial.

Nº27– Defina o **“**Preço” e a **“**Moeda” de pagamento.

Nº28– Caso decida personalizar o botão, somente será possível inserir o botão de compra pelo código HTML. Se quiser gerar também um link para compra, não faça nenhuma alteração nesta seção.

Nº29– Preencha os dados de **“**Frete” e **“**Imposto” se precisar.

Nº30– Em **“**IDs da conta do vendedor”, selecione a opção **“**Utilizar meu e-mail principal”.

Nº31– Se quiser, edite a **“**Etapa 2: Rastreie inventário, lucros e perdas” e **“**Etapa 3: Personalize os recursos avançados.

Nº32– Assim que terminar as configurações, clique em **“**Criar Botão”.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem14.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem14.png)

#### Copiando o código HTML do botão <a href="#copiando-html" id="copiando-html"></a>

Nº33– Já na próxima página, caso queira adicionar o botão de compra pelo código HTML, selecione a opção **“**Site”. Lembrando que se o botão tiver sido personalizado no [passo 28](broken-reference) deste tutorial, essa será a única opção disponível. É possível ver uma prévia de como o mesmo será exibido para o comprador no canto direito da tela.&#x20;

Nº34– Clique em **“**Selecionar código” e então o copie para a sua área de transferência. Para isso, pode usar um atalho no teclado (CTRL+C para Windows, CMD+C para Mac) ou clicar com o botão direito do mouse e escolher a opção **“**Copiar”.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/imagem15.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/imagem15.png)

![📢](https://s.w.org/images/core/emoji/13.0.0/svg/1f4e2.svg) **IMPORTANTE:**\


**–** Se deseja montar a sua página de divulgação do produto aqui na **leadlovers** e colocar o botão do PayPal direto por código HTML, é necessário adicionar logo após a tag _\<form_ do código a informação: _formulario-externo=””_. Por exemplo:

\<form formulario-externo=”” action=”https://www.paypal.com/cgi-bin/webscr” method=”post” target=”\_top”>\
\<input type=”hidden” name=”cmd” value=”\_s-xclick”>\
\<input type=”hidden” name=”hosted\_button\_id” value=”00XXXX0X0X0X0″>\
\<input type=”image” src=”https://www.paypalobjects.com/pt\_BR/BR/i/btn/btn\_buynowCC\_LG.gif” border=”0″ name=”submit” alt=”PayPal – A maneira fácil e segura de enviar pagamentos online!”>\
\<img alt=”” border=”0″ src=”https://www.paypalobjects.com/pt\_BR/i/scr/pixel.gif” width=”1″ height=”1″>\
\</form>

#### Copiando o link <a href="#copiando-link" id="copiando-link"></a>

Nº35– Se quiser apenas pegar o link para inserir em um botão de sua página, selecione a opção **“**E-mail”.

Nº36– Clique em **“**Selecionar código” e então o copie para a sua área de transferência. Para isso, pode usar um atalho no teclado (CTRL+C para Windows, CMD+C para Mac) ou clicar com o botão direito do mouse e escolher a opção **“**Copiar”.

[![](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem16.png)](https://legado.leadlovers.site/wp-content/uploads/2018/07/Imagem16.png)

Prontinho! Agora com o código HTML ou o link em mãos, basta [inserir em sua página construída aqui na leadlovers](https://suporte.love/como-inserir-um-botao-do-paypal-nas-paginas-da-leadlovers/) ou em uma plataforma externa e testar a integração.

### Como posso testar a integração? <a href="#testando-integracao" id="testando-integracao"></a>

Para testar será preciso simular uma compra de seu produto, então recomendamos que faça o seguinte:

* Crie um botão de venda com um valor menor possível, insira na sua página e efetue a compra com uma conta diferente do PayPal, pois não é possível realizar a compra com a conta do vendedor do produto.&#x20;
* Depois que realizá-la, aguarde alguns minutos e veja em seu produto na leadlovers na aba **“**Clientes” se o e-mail que utilizou para comprar o produto foi cadastrado com sucesso como aluno.
* Assim que confirmar que está tudo certo, edite o botão inserindo o valor real do produto novamente (não é necessário fazer a reinserção do código ou do link do botão depois de editar, pois o valor será automaticamente atualizado) e já pode divulgar a sua página para os seus clientes!&#x20;

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, entre em contato com o nosso suporte!

**Artigos relacionados**

– Como [inserir o botão do PayPal](https://suporte.love/como-inserir-um-botao-do-paypal-nas-paginas-da-leadlovers/) nas páginas da leadlovers?\
– Como integrar pelo [Produto Integração](https://suporte.love/produto-integracao-com-produtos-externos-versao-4-0/)?

🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™
