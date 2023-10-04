# O que é um Domínio?

**Objetivo:** aprender o que é um domínio e como usá-lo dentro da leadlovers.\
**Para que serve:** o domínio é um endereço, ele pode ser utilizado para acessar seu site ou enviar uma mensagem para seu e-mail. É também uma Marca e identificação profissional, sua ou de sua empresa.\
**Requisito(s) Obrigatórios:** **1.** para utilizar o domínio, é preciso adquirir um domínio em sites de compra e registro de domínios.

### **O que é um Domínio?** <a href="#o-que-e" id="o-que-e"></a>

Domínio é um registro que serve para localizar e identificar você ou sua empresa na Internet através de seu site. O domínio é a parte principal de toda a sua identificação profissional, pois é o “nome” do seu site e dos seus e-mails na internet. Ele é composto por um nome e uma extensão, exemplo:

**seunegocio.com.br**

**Nome:** seunegocio\
**Extensão:** .com.br

### **Domínio próprio** <a href="#dominio-proprio" id="dominio-proprio"></a>

Dentro da leadlovers, disponibilizamos alguns domínios nossos, que chamamos de “públicos”, para que nossos clientes possam usar. Por isso, denominamos como “domínio próprio” todo domínio profissional do _próprio_ cliente/empresa.

É altamente recomendado que utilize um domínio próprio para personalização da sua Marca, tanto nos endereços das páginas criadas aqui quanto no e-mail de comunicação com os leads.

#### **Como posso adquirir um domínio?** <a href="#registrar" id="registrar"></a>

No Brasil, existe o [**Registro.br**](https://registro.br/%20target=), um site em que você pode checar se o nome do domínio está disponível para uso e realizar o registro. Depois de feito, é necessário o pagamento de taxas para que você mantenha a posse do mesmo.

É possível, também, buscar e registrar seu domínio diretamente com um serviço de Hospedagem de Sites, como **HostGator**, **GoDaddy**, **Locaweb**, entre outros. Estes serviços são conhecidos por, além de permitir o registro, também disponibilizar diversas ferramentas (servidor FTP para armazenamento de arquivos, serviço de e-mail profissional, etc). Cada um deles tem seus pacotes de assinaturas, com seus devidos valores.

### **Eu já tenho um Domínio! Como posso utilizar na leadlovers?** <a href="#usar-na-leadlovers" id="usar-na-leadlovers"></a>

Quando falamos apenas do domínio principal, o endereço que registrou, é possível utilizá-lo dentro da leadlovers para personalizar o link de acesso das páginas que criar por aqui.\
Para isso, é preciso fazer o que chamamos de _apontamento_.

O **apontamento** é o direcionamento do seu domínio para os nossos servidores.\
Ele é formado por algumas configurações, que são feitas na Zona DNS do seu domínio registrado, na intenção de que ele seja usado nas páginas criadas dentro da leadlovers.

Você também pode utilizar seu domínio “indiretamente” – ou seja, não usar o domínio _principal_ – através de **subdomínios** do mesmo ou em uma conta de **e-mail profissional** que tiver. _**Para esses usos indiretos,**_ _**não é necessário realizar o apontamento do domínio principal**_.

![📢](https://s.w.org/images/core/emoji/13.0.0/svg/1f4e2.svg) **IMPORTANTE:**\


**–** Um mesmo domínio não pode ser usado em mais de uma máquina ao mesmo tempo, aqui na leadlovers.

**–** Caso seu domínio já seja utilizado para abrir um site feito em outra plataforma, apontá-lo para o nosso IP fará com que ele não abra mais estas páginas. **Seu site externo sairá do ar**. Se deseja manter seu domínio principal na forma como está, você pode criar uma entrada do tipo **subdomínio**. [**Clique aqui e veja nosso passo a passo ensinando a criar um subdomínio!**](https://suporte.love/o-que-e-um-subdominio/)

**–** O apontamento do domínio para leadlovers _não migra_ o gerenciamento do mesmo para a leadlovers. Esse seguirá sendo no seu Painel de Controle externo.

### **Passo a passo das configurações** <a href="#tutoriais" id="tutoriais"></a>

Temos materiais com instruções específicas para várias hospedagens diferentes, e sempre estamos criando artigos novos. Se você não tem certeza de qual é o Painel de Controle do seu domínio, [**confira esse material aqui onde te ensinamos como descobrir isso**](https://suporte.love/descobrir-cpanel/).

#### **Índice** <a href="#indice" id="indice"></a>

Verifique, se dentre os links abaixo sua hospedagem já está listada:

[**Registro.BR**](https://suporte.love/apontamento-dominio-registro-br/)

[**CPanel**](https://suporte.love/apontamento-dominio-cpanel/)

[**Cloudflare**](https://suporte.love/apontamento-dominio-cloudflare/)

[**Hostgator**](https://suporte.love/apontamento-dominio-hostgator/)

[**GoDaddy**](https://suporte.love/apontamento-dominio-godaddy/)

[**Locaweb**](https://suporte.love/apontamento-dominio-locaweb/)

[**Hostinger**](https://suporte.love/apontamento-dominio-hostinger/)

[**KingHost**](https://suporte.love/apontamento-dominio-kinghost/)

[**Uolhost**](https://suporte.love/apontamento-dominio-uolhost/)

[**WiX**](https://suporte.love/apontamento-dominio-wix/)

[**Umbler**](https://suporte.love/apontamento-dominio-umbler/)

#### **Realizando o apontamento** <a href="#configurando" id="configurando"></a>

Se você não encontrou o Painel de Controle (CPanel) do seu domínio na lista acima, abaixo iremos descrever como as configurações precisam ser feitas.

**Por CNAME**

Algumas alterações aconteceram na forma de apontamento de domínios, o _**apontamento agora é por CNAME**_ e a maioria das hospedagem não aceitam esse tipo de apontamento.\
Entre em contato com nosso suporte para que seja verificado a possibilidade de utilizar seu domínio principal.

**OBSERVAÇÃO:** Nem todos os painéis de controle de Zona DNS solicitam a informação **TLL**. Caso o painel de seu domínio solicite, utilize o valor **14400**.

**Nº1–** Acesse o Painel de Controle da Zona DNS de seu domínio principal. É nela que fica as entradas tipo A, TXT, MX e CNAME (entre outros tipos).

**Nº2–** Crie uma _nova_ entrada, seguindo os dados abaixo:

**Tipo da Entrada:** CNAME

**Nome da Entrada\*:** @

**Aponte sua entrada CNAME para :** cname.leadlovers.site

Confira todos os dados e salve!

_**\*Observação:**_ O nome da entrada deve atribuir ao domínio principal e a forma como essa referência será feita varia entre cada Painel de Controle (CPanel). As referências mais comuns são ” @ ” (arroba), ” . ” (ponto) ou apenas deixar em branco.\
Se você não sabe dizer qual é a atribuição do seu Painel de Controle recomendamos deixar em branco que então o próprio CPanel irá te informar como a entrada deve ficar.

Após a criação da entrada é preciso [validar o apontamento e incluir seu domínio em sua máquina](broken-reference)!

**Via tipo A**

Como mencionado acima nem todos os Painéis de Controle permitem fazer o apontamento **via CNAME**, que **é a maneira como recomendamos que seja feito**.\
Mas, mesmo o seu CPanel não permitindo que a configuração seja feita como orientado anteriormente, ainda sim, é possível apontar o seu domínio para nós!

![⚠](https://s.w.org/images/core/emoji/13.0.0/svg/26a0.svg) **ATENÇÃO:**\


– Essa forma de apontamento é muito sensível e deve ser feita com muita atenção!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

– Se qualquer informação for inserida em um formato diferente da orientação e/ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 2 dias** para propagar e surtir seus efeitos. Caso, após este prazo, elas [não tenham funcionado como deveriam](broken-reference), por favor **entre em contato com o nosso suporte**!

**Nº1–** Dentro do Painel de Controle do seu domínio, acesse a Zona DNS do mesmo.

**Nº2–** Entre as entradas que já existem na sua Zona DNS, procure uma entrada do **tipo A**, com o Nome/host de  ” **@** ”  ou apenas  ” **.** “, que esteja em branco ou que tenha no Nome somente o seu domínio principal. Essa é a entrada principal do seu domínio.\
Copie a informação que aparece em Valor/conteúdo/aponta para, esse é o **número de IP** para qual ela está apontada e guarde esses dados em algum lugar (você pode usar o Bloco de Notas para isso, se quiser).

Exemplos de entradas principais:

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/dominios1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/dominios1.png)

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/dominios2.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/dominios2.png)

**📣 CUIDADO:** os passos 3, 4 e 5 são **muito importantes**! A _falta_ dessa etapa pode impactar nas demais configurações feitas no Painel, como acesso ao webmail, disparos do seu Provedor de E-mail ou até mesmo o acesso ao próprio CPanel.

**Nº3–**Agora, **procure todas as entradas que sejam do tipo CNAME e localize as que tenham ” @ ” ou ” . ” ou espaço em branco na parte de Valor/Conteúdo/Aponta para.**\
Mais uma vez, guarde em algum lugar qual é o nome delas (novamente, o Bloco de Notas pode ser seu amigo aqui).

_**Observação:**_ A entrada cujo nome/host é “www” não será levada em consideração. Ela pode ser mantida como está.

**Exemplo:** as entradas **webmail** e **cpanel**, do tipo **CNAME**, estão com o domínio principal (wikilovers.com.br) no campo “Aponta para”. Então salve o primeiro nome delas (webmail e cpanel).

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/dominios3.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/dominios3.png)

**Lembre-se:** é preciso fazer isso com **todas** as entradas do tipo **CNAME** que estejam nesse padrão.

**Nº4–** Depois de salvar as informações das entradas que você localizou, **exclua essas mesmas entradas** da sua Zona DNS.

**Nº5–** Em seguida, você irá **recriar as entradas** que acabou de remover com as informações que salvou anteriormente.

**Tipo da entrada:** A

**Nome da entrada:** coloque o **nome da entrada** que você está recriando

**Dados, valor ou aponta para:** insira o número de IP que você salvou no passo **Nº2**.

Confira todos os dados e salve!

Repita esse procedimento até recriar todas as entradas CNAME excluídas.

_Observação:_ Nem todos os painéis de controle de Zona DNS solicitam a informação **TLL**. Caso o painel de seu domínio solicite, utilize o valor **14400**.

**Nº6–** Agora sim, **volte a entrada principal do seu domínio** (localizada como informado no passo Nº2) e a **edite**.\
Você irá alterar o IP dela para o nosso IP primário:

**Dados, valor ou aponta para:** 213.136.68.210

As demais informações da entrada permanecem como estavam.

Confira todos os dados e salve!

**Nº7–** **Crie uma **_**nova**_** entrada** com os dados abaixo para inserir nosso IP secundário (redundância/backup).

**Tipo da Entrada:** A

**Nome da Entrada:** @

**Dados, valor ou aponta para:** 213.136.70.54

Confira todos os dados e salve!

#### **Configurando a entrada de WWW** <a href="#entrada-www" id="entrada-www"></a>

É preciso também conferir como está o apontamento da entrada de www. Assim, quem incluir estas letras na hora de digitar seu domínio no navegador, será direcionado normalmente para as suas páginas.

Se essa entrada já estiver na sua Zona de DNS, você só precisa conferir se será possível mantê-la como está ou se precisará editá-la. Agora, se ela não estiver, será necessário criar uma nova entrada.

**Nº8–** Localize a entrada cujo **Nome** é **www** e confirme se os seus **Dados, valor ou aponta para** está com o seu domínio principal sem o www na frente. No nosso exemplo, está somente wikilovers.com.br:

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/dominio-www.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/dominio-www.png)

Se estiver com o seu domínio principal, _**mantenha a entrada como está**_. Caso em **Dados, valor ou aponta** para tiver qualquer outra informação, prossiga para editar o registro igual mostramos no próximo passo.

**Nº9–** Crie uma **nova entrada** _ou_ **edite a já existente.**

As informações dela serão:

**Tipo da entrada:** CNAME.

**Nome da entrada:** coloque **www** (não inclua outros caracteres, letras, ou espaços em branco).

**Dados, valor ou aponta para:** inclua o **seu domínio** sem o www. No exemplo, ficou somente wikilovers.com.br

Confirme todos os dados inseridos e salve as configurações!

**Resultado**

Ao final do processo, você terá 2 entradas tipo A apontadas para os nossos 2 IPs e uma entrada do tipo CNAME apontada para o seu domínio principal.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/dominios-resultado.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/dominios-resultado.png)

### **Próximos passos** <a href="#proximos-passos" id="proximos-passos"></a>

Depois de configurado o apontamento, você precisa [**validar se o mesmo aconteceu com sucesso**](https://suporte.love/como-saber-se-meu-apontamento-propagou/).

E então, adicionar seu domínio em sua máquina. Para maiores detalhes, [**clique aqui e veja nosso tutorial, explicando como incluir seu domínio em uma máquina**](https://suporte.love/como-cadastrar-dominio-maquina/)!

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, **entre em contato com o nosso suporte**!

**Artigos relacionados**

– [O que é um subdomínio?](https://suporte.love/o-que-e-um-subdominio/)\
– Como [descobrir o Painel de Controle](https://suporte.love/descobrir-cpanel/) do seu domínio.\
– [Validando o apontamento.](https://suporte.love/como-saber-se-meu-apontamento-propagou/)\
– Como [cadastrar um domínio/subdomínio](https://suporte.love/como-cadastrar-dominio-maquina/) em sua máquina.

**É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
