# O que são as configurações de DNS de E-mail?

**Objetivo:** Explicar o que são as configurações de DNS de e-mail e apresentar uma visão geral de como criar cada uma das entradas.\
**Para que serve:** A principal função dessas configurações é auxiliar a entregabilidade de suas mensagens, disparadas pela automação de sua conta. A ausência das entradas pode causar diversos comportamentos indesejados no momento do envio dos e-mails. Entre eles, os principais são: seus e-mails serem entregues como spam ou até mesmo não chegarem aos destinatários.\
**Requisitos obrigatórios:** **1.** Ter uma conta de e-mail profissional. **2.** Ter essa conta [cadastrada e ativa](https://suporte.love/adicionar-e-ativar-e-mail-para-disparos/) nas Contas de E-mail na leadlovers.

### **O que são as configurações de DNS de E-mail?** <a href="#o-que-e" id="o-que-e"></a>

As configurações de DNS de e-mail são essenciais para autenticação do seu domínio. São elas que irão permitir que os provedores de e-mail identifiquem que o seu domínio é confiável e que a plataforma está autorizada a realizar envios em seu nome. Com essas configurações feitas, é menos provável que os provedores identifiquem os seus e-mails como spam ou até mesmo não os entreguem aos seus destinatários.

Nos tópicos seguintes deste artigo, falaremos um pouco mais sobre o assunto e também traremos um passo a passo geral de como fazer essas configurações no painel de controle do seu domínio.

### **Quais entradas irei criar?** <a href="#tipo-de-entrada" id="tipo-de-entrada"></a>

**– MX (Mail eXchanger record)**: Esta entrada permite que o sistema da leadlovers use sua conta de e-mail para realizar os disparos de mensagens e garantir a identificação correta desta operação.

**– DKIM (DomainKeys Identified Mail):** É um mecanismo para autenticação de e-mail baseado em criptografia de chaves públicas. Com ele, todas as mensagens enviadas serão assinadas digitalmente, colocando no cabeçalho do e-mail informações de identificação. Com isso, o servidor de destino consegue confirmar se o e-mail enviado partiu de um servidor autorizado ou não.

**– SPF (Sender Policy Framework):** É um sistema que especifica quais servidores estão autorizados a enviar e-mails do seu domínio. Isso evita que enviem e-mails não autorizados utilizando seu domínio profissional.

**– DMARC:** É um padrão técnico que foi criado com o intuito de reduzir as fraudes e os abusos via e-mail, validando as mensagens enviadas e padronizando o modo com que os provedores fazem a leitura e a autenticação dos e-mails recebidos.

**– LINK DE REDIRECT:** O link redirect é um link de redirecionamento que está presente em todos os seus e-mails. Quando um lead clicar em algum link em seu e-mail ele aparecerá ao redirecionar a página. Criando o link redirect personalizado, além de padronizar o link de direcionamento, ele aumenta a visibilidade em relação aos provedores de e-mail. Visto que os links incluídos no conteúdo do e-mail são verificados por todos os provedores, obtendo um link próprio melhora as suas entregas e reduz o risco de inclusões em blacklists.

### **O que é uma conta de e-mail profissional?** <a href="#email-profissional" id="email-profissional"></a>

Uma conta de e-mail profissional é criada com o seu domínio próprio, para comunicações mais profissionais da sua empresa. Dessa forma, é possível configurar um endereço de e-mail personalizado, por exemplo:

\[email protected]

Ainda, você terá uma caixa de e-mail em que poderá ter recebimentos e fazer envios.

#### **Já tenho domínio, mas não tenho um e-mail profissional. E agora?** <a href="#nao-tem-email" id="nao-tem-email"></a>

Caso já tenha um serviço de hospedagem de sites contratado, alguns deles já oferecem caixas de e-mail junto com os seus planos (até mesmo com os mais básicos). Consulte a equipe da plataforma contratada para verificar se está disponível no pacote que adquiriu.

Além disso, é possível também contratar serviços de e-mail profissional separadamente, por exemplo o G Suite ou Titan, ou até mesmo criar uma caixa de entrada gratuita. Para isso, nós sugerimos a plataforma [Zoho](https://www.zoho.com/pt-br/).

#### **Mas por que eu não posso fazer essas configurações no meu e-mail de domínio público, por exemplo o Gmail?** <a href="#dominio-publico" id="dominio-publico"></a>

Nós chamamos de e-mail de domínio público todo aquele que é possível criar para uso pessoal, por exemplo o Gmail, Hotmail, Outlook, entre outros. Com eles, **não é possível fazer as configurações de DNS de e-mail** porque não são de domínio próprio e, portanto, não pertencem a quem está usando e também não tem como finalidade o disparo em volumes maiores. Além disso, um e-mail profissional com a sua marca passa aos seus leads mais credibilidade no momento de receber as suas comunicações.

### **Como usar meu e-mail profissional como conta remetente na leadlovers?** <a href="#conta-remetente-leadlovers" id="conta-remetente-leadlovers"></a>

Para usar o seu e-mail profissional como conta remetente na leadlovers, primeiramente é necessário adicioná-lo em **Contas de E-mail**. Se ainda não sabe como fazer esse procedimento, [consulte esse material](https://suporte.love/adicionar-e-ativar-e-mail-para-disparos/). Depois que adicionar e fazer as configurações de DNS, basta escolher a conta de disparo antes de fazer o envio dos seus e-mails.

É possível escolher a conta **a nível de máquina**, nas **Configurações** da mesma:

[![](https://legado.leadlovers.site/wp-content/uploads/2017/06/img-1.png)](https://legado.leadlovers.site/wp-content/uploads/2017/06/img-1.png)

Também pode escolher a conta antes de disparar os seus e-mails no formato de **Sequência de E-mails**:

[![](https://legado.leadlovers.site/wp-content/uploads/2017/06/img-2.png)](https://legado.leadlovers.site/wp-content/uploads/2017/06/img-2.png)

E por último, mas não menos importante, no formato de **Automação**:

[![](https://legado.leadlovers.site/wp-content/uploads/2017/06/img-3.png)](https://legado.leadlovers.site/wp-content/uploads/2017/06/img-3.png)

### **Passo a passo das configurações** <a href="#tutoriais" id="tutoriais"></a>

Temos materiais com instruções específicas para várias hospedagens diferentes, e sempre estamos criando artigos novos. Se você não tem certeza de qual é o Painel de Controle do seu domínio, [confira esse material aqui onde te ensinamos como descobrir isso.](https://suporte.love/descobrir-cpanel/)

#### **Índice** <a href="#indice" id="indice"></a>

Verifique, se dentre os links abaixo sua hospedagem já está listada:

[**Registro.br**](https://suporte.love/dns-registrobr/)

[**cPanel**](https://suporte.love/configurar-dkim-spf-mx-no-cpanel/)

[**Cloudflare**](https://suporte.love/configurar-dkim-spf-mx-no-cloudflare/)

[**Hostgator**](https://suporte.love/configurar-dkim-spf-mx-no-hostgator/)

[**GoDaddy**](https://suporte.love/configurar-dkim-spf-mx-no-godaddy/)

[**Locaweb**](https://suporte.love/como-fazer-as-configuracoes-de-dns-de-e-mail-na-locaweb/)

[**Hostinger**](https://suporte.love/como-fazer-as-configuracoes-de-dns-de-e-mail-no-hostinger/)

[**KingHost**](https://suporte.love/como-fazer-as-configuracoes-de-dns-de-e-mail-na-kinghost/)

[**UolHost**](https://suporte.love/como-fazer-as-configuracoes-de-dns-de-e-mail-na-uolhost/)

[**WiX**](https://suporte.love/dns-de-email-wix/)

[**Umbler**](https://suporte.love/como-fazer-as-configuracoes-de-dns-de-e-mail-no-umbler/)

### **Realizando as configurações** <a href="#configuracoes" id="configuracoes"></a>

Se você não encontrou o Painel de Controle do seu domínio na lista acima, abaixo iremos descrever como as configurações precisam ser feitas.

#### **Utilizando as entradas em formato MX** <a href="#via-mx" id="via-mx"></a>

**Observação:** nem todos os painéis de controle de Zona DNS solicitam a informação **TTL**. Caso o painel de seu domínio solicite, utilize o valor **14400** para todas as entradas abaixo.

**Entrada MX (Mail eXchanger record)**

**Nº1–** Acesse o Painel de Controle da Zona DNS de seu domínio principal. É nela que ficam as entradas tipo A, TXT, MX e CNAME (entre outros tipos).

**Nº2–** Crie uma **nova entrada** com os dados abaixo:

**Tipo da Entrada:** MX

**Nome da Entrada:** mailsg

**Prioridade:** 0

**Dados, valor ou aponta para:** mx.sendgrid.net

![⚠](https://s.w.org/images/core/emoji/13.0.0/svg/26a0.svg) **ATENÇÃO:**\


**–** Algumas hospedagens não permitem a inserção da entrada **MX**. Se esse for o caso, é necessário fazer as entradas por **CNAME**, então pode prosseguir para o tópico: [**Utilizando as entradas em formato CNAME**](broken-reference).

Confira as informações e salve!

**Entrada DKIM (DomainKeys Identified Mail)**

**Nº3–** Ainda na zona DNS do seu domínio, crie **mais uma entrada** com os seguintes dados:

**Tipo da Entrada:** TXT

**Nome da Entrada:** m1.\_domainkey

**Dados, valor ou aponta para:** k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB

Antes de salvar, confira se está tudo certo e então prossiga para o próximo passo.

**Entrada SPF (Sender Policy Framework)**

**Nº4–** Depois que salvar a última entrada, vá até a opção de **criar uma nova** e insira os dados a seguir:

**Tipo da Entrada:** TXT

**Nome da Entrada:** mailsg

**Dados, valor ou aponta para:** v=spf1 include:sendgrid.net \~all

Conferiu se está tudo certo? Já pode salvar!

**Entrada DMARC**

**Nº5–** A penúltima entrada a ser criada é a DMARC. Para ela, use os dados:

**Tipo da Entrada:** TXT

**Nome da Entrada:** \_dmarc

**Dados, valor ou aponta para:** v=DMARC1; p=none; rua=mailto:\[email protected]

![⚠](https://s.w.org/images/core/emoji/13.0.0/svg/26a0.svg) **ATENÇÃO:**\


**–** Substitua a parte **seudominio.com** pelo domínio o qual é usado pelo seu e-mail profissional e no qual você está inserindo estas informações. No exemplo das imagens, o domínio usado é **wikilovers.com.br**. Por isso, a entrada ficou:

**v=DMARC1; p=none; rua=mailto:\[email protected]**

Se certifique de que os dados foram inseridos corretamente – especialmente se a informação “seudominio.com” foi substituída pelo domínio que está sendo configurado – e salve.

**Entrada do Link de Redirect**

**Nº6–** Por fim, crie a entrada do Link de Redirect:

**Tipo da Entrada:** CNAME

**Nome da Entrada:** aqui você pode determinar alguma palavra de sua preferência, normalmente nós configuramos como _click_.

**Dados, valor ou aponta para:** cname.leadlovers.site

Confira os dados e salve!

**Observação:** As informações inseridas na sua zona DNS podem levar **até 24 horas** para propagarem totalmente.

Após inserir estas cinco entradas, você deve [validá-las em sua conta leadlovers.](broken-reference)

#### **Utilizando as entradas em formato CNAME** <a href="#via-cname" id="via-cname"></a>

![📢](https://s.w.org/images/core/emoji/13.0.0/svg/1f4e2.svg) **IMPORTANTE:**\


**–** Se você **já criou as entradas por MX** seguindo as orientações anteriores, vá direto até o tópico [**Próximos Passos**](broken-reference). As próximas entradas devem ser criadas **somente se na zona DNS do seu domínio não tenha sido possível criar as entradas por MX.**

Algumas hospedagens não permitem, de forma alguma, a inclusão de uma entrada do tipo **MX**. Nestes casos, utilizamos três das entradas no formato **CNAME** (o DMARC continua sendo em formato TXT). Para poder validá-las mais tarde, é necessário alterar aqui na plataforma essas entradas na sua Conta de E-mail. [Acesse esse tutorial](https://suporte.love/como-alterar-de-mx-para-cname/) para saber como fazer esse procedimento e então retorne aqui para criar os apontamentos.

Segue abaixo as informações de como inserir cada uma das entradas.

**Observação:** nem todos os painéis de controle de Zona DNS solicitam a informação TLL. Caso o painel de seu domínio solicite, utilize o valor 14400 para todas as entradas abaixo.

**Nº1–** Acesse o Painel de Controle da Zona DNS de seu domínio principal. É nela que ficam as entradas tipo A, TXT, MX e CNAME (entre outros tipos).

**Nº2–** Crie uma **nova entrada** com os dados abaixo:

**Tipo da Entrada:** CNAME

**Nome da Entrada:** mailsg

**Dados, valor ou aponta para:** u2316725.wl226.sendgrid.net

Confira as informações e salve!

**Nº3– Ainda na zona DNS do seu domínio, crie mais uma entrada com os seguintes dados:**

**Tipo da Entrada:** CNAME

**Nome da Entrada:** s1.\_domainkey

**Dados, valor ou aponta para:** s1.domainkey.u2316725.wl226.sendgrid.net

Antes de salvar, confira se está tudo certo e então prossiga para o próximo passo.

**Nº4– Depois que salvar a última entrada, vá até a opção de criar uma nova e insira os dados a seguir:**

**Tipo da Entrada:** CNAME

**Nome da Entrada:** s2.\_domainkey

**Dados, valor ou aponta para:** s2.domainkey.u2316725.wl226.sendgrid.net

Conferiu se está tudo certo? Já pode salvar!

**Nº5–** A penúltima entrada a ser criada é a DMARC. Para ela, use os dados:

**Tipo da Entrada:** TXT

**Nome da Entrada:** \_dmarc

**Dados, valor ou aponta para:** v=DMARC1; p=none; rua=mailto:\[email protected]

![⚠](https://s.w.org/images/core/emoji/13.0.0/svg/26a0.svg) **ATENÇÃO:**\


**–** Substitua a parte **seudominio.com** pelo domínio o qual é usado pelo seu e-mail profissional e no qual você está inserindo estas informações. No exemplo das imagens, o domínio usado é **wikilovers.com.br.** Por isso, a entrada ficou:

**v=DMARC1; p=none; rua=mailto:\[email protected]**

Se certifique de que os dados foram inseridos corretamente – especialmente se a informação “seudominio.com” foi substituída pelo domínio que está sendo configurado – e salve.

**Nº6–** Por fim, crie a entrada do Link de Redirect:

**Tipo da Entrada:** CNAME

**Nome da Entrada:** aqui você pode determinar alguma palavra de sua preferência, normalmente nós configuramos como _click_.

**Dados, valor ou aponta para:** cname.leadlovers.site

Confira os dados e salve!

**Observação:** As informações inseridas na sua zona DNS podem levar **até 24 horas** para propagarem totalmente.

Após inserir estas cinco entradas, você deve [validá-las em sua conta leadlovers.](broken-reference)

### **Arquivos com as entradas** <a href="#arquivos" id="arquivos"></a>

Se quiser solicitar para que o suporte da hospedagem do seu domínio faça as configurações, disponibilizamos dois arquivos com as entradas MX e CNAME para download:

* [Entradas MX](https://legado.leadlovers.site/wp-content/uploads/2017/06/Entradas-MX.txt)
* [Entradas CNAME (Utilize somente se não for possível criar as entradas por MX)](https://legado.leadlovers.site/wp-content/uploads/2017/06/Entradas-CNAME.txt)

Mesmo solicitando que a criação das entradas seja feita por terceiros, não esqueça de [validá-las aqui na leadlovers](https://legado.leadlovers.site/validando-dns-no-leadlovers) assim que forem concluídas.

### **Próximos passos** <a href="#proximos-passos" id="proximos-passos"></a>

Depois de feitas as configurações, é necessário fazer a validação de cada uma delas. [Clique aqui e siga este passo a passo!](https://suporte.love/validando-dns-no-leadlovers/)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor **entre em contato com o nosso suporte**!

**Artigos relacionados**

– Como [validar as configurações de DNS de E-mail](https://suporte.love/validando-dns-no-leadlovers/) na leadlovers?\
–[ O que é um domínio?](https://suporte.love/o-que-e-um-dominio/)\
– Como[ descobrir o Painel de Controle](https://suporte.love/descobrir-cpanel/) do seu domínio?

🏁 **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
