# Integração Webinarjam/Everwebinar via Zapier

Para integrar o Webinarjam ou o Everwebinar com o Leadlovers via Zapier, siga os passos abaixo:

### 1ª Etapa: Configurando o Zapier

**1) Criando o Zap**\
**a.** Crie um Zap para WebinarJam/Everwebinar automaticamente [clicando aqui](broken-reference).\
**b.** Depois, clique em **Create this Zap**.

**2) Selecione o evento desejado.**\
**a.** Clicando em **Show Less common options** você poderá ver todas as ações do visitante para as quais podemos criar um Zap (**imagem 1**). Para esse tutorial, utilizaremos a ação **New Registration**.\
**b.** Escolha seu evento e clique em **Save and Continue**.



**3) Conecte a sua conta do WebinarJam/Everwebinar.**\
**a.** Clique no botão **Connect an Account**.\
**b.** Uma tela solicitando uma chave API (API Key) aparecerá (**imagem 2**). [Siga esse tutorial](https://help.genesisdigital.co/017125-Where-do-I-find-my-WebinarJam-API-Key) para obter a sua.\
**c.** Clique em **Test** para testar a conexão de sua conta no WebinarJam/Everwebinar.\
**d.** Clique em **Continue**.



**4) Escolhendo o Webinar**\
**a.** Escolha o Webinar que você quer integrar. (**imagem 3**)\
**b.** Clique em **Continue**



**5) Testando a integração**\
**a.** Para ter a certeza que tudo o que fizemos até aqui está correto, cheque novamente se o Webinar que mostra na tela é o que você quer integrar. (**imagem 4**)\
**b.** Após isso, clique em **Fetch & Continue**.\
**c.** Depois do teste ser concluído, clique em **Continue**.



**6) Criando uma ação**\
**a.** Selecione o ícone **Webhooks**. (**imagem 5**)\
**b.** Selecione o método POST.\
**c.** Clique em **Continue**.



### 2ª Etapa: Configurando o Leadlovers

**7) Criando o Webhook**\
**a.** [Clique aqui para criar um novo Webhook](https://suporte.love/como-criar-um-webhook/)\
**b.** Preencha o Nome do Webhook e selecione a ação **Inserir novo lead**.\
**c.** Selecione a máquina, funil e nível em que você quer que o lead seja inserido.\
**d.** Caso queira aplicar uma Tag na inscrição do lead, selecione a Tag.\
**e.** Clique em **Gerar link Webhook**. Uma tela com suas informações aparecerá**\***. (**imagem 6**)

[![imagem 6](https://legado.leadlovers.site/wp-content/uploads/2020/09/img-221648-20180131154813.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/img-221648-20180131154813.png)_**imagem 6**_\
**\***: _Cada Webhook tem um Token diferente. Assim como cada máquina e cada funil tem um código único._&#x20;

### 3ª Etapa: Finalizando a configuração

**8) Votando ao Zapier** (**imagem 7**)\
**a.** No campo **URL** no Zapier, preencha o dado que é mostrado em **Endereço do WebHook** no Leadlovers (**imagem 6**).\
**b.** Em **Payload Type**, selecione **Json**.\
**c.** Em **Data**, você deve colocar os dados de código da máquina, código do funil e código do email que são encontrados no Webhook que criamos.\
**d.** Depois de preencher esses 3 dados, crie mais 2 campos: **Name** e **Email**.\
**e.** Clique no símbolo para selecionar os dados oriundos do WebinarJam/Everwebinar. ![](https://legado.leadlovers.site/wp-content/uploads/2020/09/img-221648-20180131155312.png)\
**f.** No campo **Headers** (**imagem 8**), insira **Authorization** no primeiro campo e os dados encontrados no campo 5 (**imagem 6**) no segundo campo.\
**g.** Clique em **Continue**.





**9) Testando via Zapier**\
**a.** Agora na tela de teste (**imagem 9**), clique no botão azul **Send Test To Webhooks by Zapier**.\
**b.** Em poucos segundos um lead de testes (**\[email protected]**) entrará em sua maquina e funil desejados no Leadlovers.\
**c.** Clique em **Finish**.



**10) Ativando o Zap**\
**a.** Ative seu Zap mudando a chave para **ON** (**imagem 10**)



Pronto, a integração do WebinarJam/Everwebinar com o Leadlovers está completa!\
[Acesse o link de inscrição do seu Webinar](https://help.genesisdigital.co/938578-Where-are-my-links-in-WebinarJam) e inscreva-se. Após alguns segundos, verifique se o email com o qual você se inscreveu entrou no funil e email desejado.

***

Qualquer dúvida ou problema, contate nosso time do suporte via ticket ou chat online\
Você já conhece o [leadlovers na prática](https://www.youtube.com/leadloversnapratica)? É o nosso canal do [Youtube](https://www.youtube.com/leadloversnapratica). Nele postamos vídeos tutoriais, ta esperando o que pra se [inscrever](https://www.youtube.com/leadloversnapratica)?
