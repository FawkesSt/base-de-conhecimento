# Como saber se meu apontamento propagou?

**Objetivo:** Ensinar como consultar a propagação de domínio e subdomínio.\
**Para que serve:** Depois de fazer qualquer alteração na zona DNS do seu domínio ele passa pelo período de propagação, que é o tempo que leva para que os servidores ao redor do mundo atualizem as novas informações inseridas. É possível consultar o andamento dessas atualizações.\
**Requisitos obrigatórios: 1.** Ter um [domínio](https://suporte.love/o-que-e-um-dominio/) ou [subdomínio](https://suporte.love/o-que-e-um-subdominio/) apontado para a leadlovers.

### **Período de propagação** <a href="#periodo-propagacao" id="periodo-propagacao"></a>

Acabou de apontar o seu domínio ou subdomínio e quer saber se está tudo certo com as entradas criadas? Depois que são feitas quaisquer alterações na zona DNS, o domínio passa por aquilo que chamamos de _período de propagação_. Esse é o tempo que leva para os servidores ao redor do mundo atualizarem as informações que você inseriu na sua DNS e pode levar **até 24 horas** para propagarem totalmente.

Nesse tutorial, te ensinaremos duas maneiras de consultar se os apontamentos já estão propagando e se o seu domínio ou subdomínio foi apontado corretamente. Uma delas é usando o [**DNS Checker**](broken-reference), que permite consultar os apontamentos do tipo **A** e também do tipo **CNAME**. Além dessa forma, também é possível consultar pelo [**Prompt de Comando do Windows**](broken-reference) caso tenha feito as entradas pelo tipo **A**.

### **Como consultar o apontamento pela ferramenta DNS Checker** <a href="#dns-checker" id="dns-checker"></a>

**Nº1–** Acesse um site de consulta de zona DNS, eles são comumente chamados de “DNS Checker” e mostram as informações nos servidores ao redor do mundo. Nós sugerimos que a consulta seja feita em um dos indicados abaixo:

* [whatsmydns.net](https://www.whatsmydns.net/)
* [dnschecker.org](https://dnschecker.org/)

Caso tenha feito os apontamentos com o tipo de entrada **A** adicionando os nossos IPs na sua zona DNS, vá até o tópico: [**Consultando apontamento A**](broken-reference).

Já se a entrada foi criada por **CNAME**, siga para o tópico: [**Consultando apontamento CNAME**](broken-reference).

#### **Consultando apontamento A** <a href="#consultando-apontamento-a" id="consultando-apontamento-a"></a>

**Nº2–** Preencha o domínio que deseja consultar.

**Nº3–** Dentre as opções, escolha o tipo **“A”**.

**Nº4–** Clique em **“Search”** para iniciar a pesquisa.

**Nº5–** Se a pesquisa retornar todas as localidades com os nossos dois IPs (**213.136.68.210** ou **213.136.70.54**) e a grande maioria delas estiver com um check verde (✅), isso significa que os seus apontamentos propagaram.

[![](https://legado.leadlovers.site/wp-content/uploads/2016/06/passo1.png)](https://legado.leadlovers.site/wp-content/uploads/2016/06/passo1.png)

**Observação:** É muito importante que os apontamentos sejam feitos para os nossos **dois IPs**. Caso tenha feito somente para um deles, [consulte os nossos materiais e revise as entradas da sua zona DNS](https://suporte.love/o-que-e-um-dominio/).

Se algumas localidades estiverem retornando IPs diferentes dos nossos da leadlovers, aguarde mais algumas horas e então faça a consulta novamente. Enquanto dura o período de propagação, as informações antigas que estavam na sua zona DNS ainda podem aparecer na consulta. Esse período pode levar **até 24 horas**.

#### **Consultando apontamento CNAME** <a href="#consultando-apontamento-cname" id="consultando-apontamento-cname"></a>

**Nº2–** Preencha o domínio ou subdomínio que deseja consultar.

**Nº3–** Dentre as opções, escolha o tipo **“CNAME”**.

**Nº4–** Clique em **“Search”** para iniciar a pesquisa.

**Nº5–** Se a pesquisa retornar todas as localidades com o nosso domínio **cname.leadlovers.site** e a grande maioria delas estiver com um check verde (✅), isso significa que os seus apontamentos propagaram.

[![](https://legado.leadlovers.site/wp-content/uploads/2016/06/passo2.png)](https://legado.leadlovers.site/wp-content/uploads/2016/06/passo2.png)

Caso algumas localidades estejam retornando uma entrada diferente da nossa da leadlovers, aguarde mais algumas horas e então faça a consulta novamente. Enquanto dura o período de propagação, as informações antigas que estavam na sua zona DNS ainda podem aparecer na consulta. Esse período pode levar **até 24 horas**.

### **Como consultar o apontamento pelo Prompt de Comando** <a href="#prompt-de-comando" id="prompt-de-comando"></a>

![⚠](https://s.w.org/images/core/emoji/13.0.0/svg/26a0.svg) **ATENÇÃO:**\


**–** Recomendamos que a consulta pelo Prompt de Comando seja feita apenas caso tenha apontado o seu domínio com entradas do tipo **A**. Se fez as entradas por **CNAME** essa consulta pode retornar um IP diferente e, por isso, indicamos que ela seja feita por uma ferramenta própria para isso, como ensinamos no tópico: [**Como consultar o apontamento pela ferramenta DNS Checker?**](broken-reference)

**Nº1–** Clique no **ícone do Windows** no canto inferior esquerdo do seu computador.

**Nº2–** Na barra de busca digite: _cmd_.

**Nº3–** Selecione a opção **“Prompt de Comando”**.

[![](https://legado.leadlovers.site/wp-content/uploads/2016/06/passo3.png)](https://legado.leadlovers.site/wp-content/uploads/2016/06/passo3.png)

**Nº4–** Já com o Prompt de Comando aberto, escreva: _ping seudominio.com.br_, substituindo a informação **“seudominio.com.br”** pelo domínio que você deseja fazer a consulta. No nosso exemplo, escrevemos: _ping wikilovers.com.br_.

[![](https://legado.leadlovers.site/wp-content/uploads/2016/06/passo4.png)](https://legado.leadlovers.site/wp-content/uploads/2016/06/passo4.png)

**Nº5–** Aperte a tecla **“Enter”**. Se a resposta disparar um de nossos dois IPs (**213.136.68.210** ou **213.136.70.54**) conforme indicado na imagem, isso significa que os apontamentos estão corretos.

[![](https://legado.leadlovers.site/wp-content/uploads/2016/06/passo5.png)](https://legado.leadlovers.site/wp-content/uploads/2016/06/passo5.png)

**Observação:** É muito importante que os apontamentos sejam feitos para os nossos **dois IPs**. Caso tenha feito somente para um deles, [consulte os nossos materiais e revise as entradas da sua zona DNS.](https://suporte.love/o-que-e-um-dominio/)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor **entre em contato com o nosso suporte**!

**Artigos relacionados**

– [O que é um domínio](https://suporte.love/o-que-e-um-dominio/);\
– [O que é um subdomínio](https://suporte.love/o-que-e-um-subdominio/);\
– Como [descobrir o Painel de Controle](https://suporte.love/descobrir-cpanel/) do seu domínio;\
– Como [cadastrar um domínio/subdomínio](https://suporte.love/como-cadastrar-dominio-maquina/) em sua máquina.

🏁 **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
