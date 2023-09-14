# Curso (EAD):Integração Hotmart

Objetivo: Realizar integração com a Hotmart.\
Para que serve: Essa integração é feita entre uma venda de produto criado na Hotmart e o produto EAD feito aqui na leadlovers. Assim, quem fizer a compra pelo seu checkout na Hotmart, automaticamente vai ser adicionado como cliente na sua área de membros da leadlovers.\
Requisito Obrigatório: Ter uma conta de produtor na [Hotmart](https://app-vlc.hotmart.com/login).

### Realizando a integração <a href="#realizando-integracao" id="realizando-integracao"></a>

Neste tutorial, te ensinaremos como fazer uma integração entre a plataforma Hotmart, especializada em vendas de produtos digitais, e o produto EAD da leadlovers. Com essa integração, você pode liberar um acesso à área de membros na leadlovers para os leads que comprarem o seu produto. Caso queira integrar a Hotmart apenas com as suas máquinas aqui da leadlovers, pode fazer por meio da integração nativa acessando [esse link](https://suporte.love/como-integrar-listboss-do-hotmart-com-o-leadlovers/).

Nº1– Faça login em sua [conta Hotmart](https://app-vlc.hotmart.com/login).

Nº2– No menu lateral, clique em **“**Produtos”.

Nº3– Entre as opções que vão abrir logo abaixo, selecione: **“**Meus produtos”.

![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_4-1.png)

Nº4– Você será direcionado a uma tela com a lista dos seus produtos. Pesquise por aquele que deseja integrar com a leadlovers.

Nº5– Copie o **“**ID” de seu produto (somente os números) e salve-o em algum lugar porque logo iremos usá-lo, o Bloco de Notas pode ser um grande aliado.

![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_5-1.png)

Nº6– Agora no menu lateral, escolha a opção **“**Ferramentas”.

![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_6-1.png)

Nº7– Acesse a opção **“**Webhook (API e Notificações)”.

![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_7-1.png)

Nº8– Na próxima tela, clique em **“**Autenticação”

Nº9– Logo abaixo, copie o **“**código Hottok” (ele está em negrito) e salve em algum lugar, pois nos próximos passos ele será necessário também.

**Obs:** caso seja necessário, nessa mesma tela terá um botão **“documentação”** onde terá dicas e tutoriais de como criar um Webhook.

![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_8-1-1024x621.png)

#### Acessando a leadlovers <a href="#acessando-a-leadlovers" id="acessando-a-leadlovers"></a>

Mantenha a aba da Hotmart aberta no seu navegador e então abra uma nova (pode utilizar o atalho CTRL+T para isso) para acessar sua conta da leadlovers. Dentro dela, encontre o seu produto em **“**Cursos online EAD”.

![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_9-1.png)

Nº10– Ao acessá-lo, clique na aba **“**Integrações”.

Nº11– Encontre a opção **“**Integração com o Hotmart”. Nela copie a **“URL de notificação”** e salve em algum lugar, como por exemplo o Bloco de Notas. Iremos utilizá-la nos próximos passos.

![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_12-1-1024x351.png)

Nº12– Após isso, copie aquele token que reservamos no  [passo 9](broken-reference) e cole em Token de integração, na leadlovers.

Nº13– Insira também nessa mesma tela, o **ID** do seu Produto Hotmart, aquele que foi copiado no [passo 5](broken-reference).

![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_11-2-1024x279.png)

* Ainda nessa tela é possível liberar o produto por **emissão de boleto**
* E **bloquear o acesso** do cliente após cancelamento do produto, basta marcar a opção desejada.

\
![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_13-1.png)\


Nº14– Após fazer as alterações, role a tela para baixo e clique em **“Salvar** as Configurações”.

![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_14-1.png)

#### Retornando à Hotmart <a href="#retornando-a-hotmart" id="retornando-a-hotmart"></a>

Retorne a tela de Webhook da Hotmart, a mesma tela que copiou o token no [passo 9.](broken-reference)

Nº17– Clique em **“**Cadastrar Webhook” para criar uma nova configuração.

![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_15-1.png)

Nº19– Abrirá uma Popup,  neste campo, preencha as informações solicitadas.

\
![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_16-1.png)\


1. escreva o nome da configuração. Escolha o que achar melhor e que te ajude\
   a te lembrar do que ela se trata.
2. Selecione o seu produto no qual esta configuração será usada.
3. Agora cole a **“**URL de notificação” que você copiou no [passo 2](broken-reference) em seu produto na leadlovers.&#x20;
4. Em **versão**, Indicamos utilizar a versão 1, visto que versão 2 ainda possui algumas inconsistências.
5. Em eventos, Escolha a opção **“**Compra Aprovada” (caso deseje liberar acesso por emissão do boleto, marque também a opção **“**Aguardando pagamento”).![](https://suporte.love/wp-content/uploads/2020/07/Screenshot\_17.png)

Nº20– Clique na opção **“**Salvar”.

Pronto, sua integração Hotmart com seu produto criado no leadlovers já foi feita! Agora é só testar para garantir que tudo está funcionando corretamente.

### Testando a integração <a href="#testando-integracao" id="testando-integracao"></a>

Para testar será preciso que você simule uma compra de seu produto, então faça o seguinte:

– Marque a opção de **“**Liberar acesso na emissão do boleto” (que mostramos no [passo 13](broken-reference)) na leadlovers e clique em **“**Salvar as Configurações”.

– Após isso, compre o seu produto por boleto (não precisa fazer o pagamento, apenas gerar o boleto é o suficiente).

– Depois que simular a compra, aguarde alguns minutos e veja na aba **“**Clientes” em seu produto na leadlovers se o e-mail que utilizou entrou em seu produto como cliente.

Lembre-se de **desmarcar** a opção de liberar o acesso na emissão do boleto assim que concluir o seu teste.

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, **entre em contato com o nosso suporte**!

**Artigos relacionados**

– Como [integrar ListBoss da Hotmart com a leadlovers.](https://suporte.love/como-integrar-listboss-do-hotmart-com-o-leadlovers/)\
– Como criar um [Produto EAD](https://suporte.love/como-criar-um-produto/).

**É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
