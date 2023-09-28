# Apontamento de domínio no Hostinger

**Objetivo:** Mostrar o passo a passo de como utilizar o seu domínio que está no **Hostinger** dentro da leadlovers.\
**Para que serve:** O apontamento permite utilizar o seu domínio como endereço de acesso as páginas e/ou área de membro criadas dentro do sistema.\
**Requisito(s) necessário(s):** **1.** Ter um domínio próprio já comprado e **2.** ter acesso a Zona DNS do seu Hostinger.

&#x20;**IMPORTANTE:**\


**–** Os passos à seguir devem ser feitos **somente se o seu domínio for administrado pelo Hostinger**.\
Se ele estiver sob administração de outro serviço, é preciso que as configurações sejam realizadas no Painel de Controle específico deste segundo serviço. Nesse [artigo aqui](https://suporte.love/descobrir-cpanel/) nós mostramos como você pode confirmar qual é o painel do seu domínio.

**–** Caso seu domínio já seja utilizado para abrir um site feito em outra plataforma, apontá-lo para o nosso IP fará com que ele não abra mais estas páginas. **Seu site externo sairá do ar**.\
Se deseja manter seu domínio principal na forma como está, você pode criar uma entrada do tipo **subdomínio**. **Clique aqui e veja nosso passo a passo, ensinando a criar um subdomínio \[em breve]!**

### **Acessando o Cpanel de seu domínio** <a href="#zona-dns" id="zona-dns"></a>

Uma vez logado no [**Painel de membros do Hostinger**](https://www.hostinger.com.br/cpanel-login) você verá na Home uma lista com todos os seus domínios cadastrados por lá.

**Nº1–** Na parte de Hospedagem, localize o domínio que deseja usar em sua máquina aqui no leadlovers e clique no botão **Gerenciar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/hg1-1.png)

Você será redirecionado ao Painel de Controle (ou **Cpanel**) do domínio. Nele terão várias categorias e cada uma agrupa diversas opções.

**Nº2–** Localize o quadro da categoria Avançado. Dentre as opções disponíveis nele, clique sobre a opção **Editor de Zona DNS**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/hg2.png)

### **Salvando as informações necessárias** <a href="#salvar" id="salvar"></a>

Normalmente, a Zona DNS no Hostinger já vem com configurações nela e, por isso, antes de fazer qualquer apontamento precisamos primeiro salvar algumas informações! Ok?

![⚠](https://s.w.org/images/core/emoji/13.0.0/svg/26a0.svg) **ATENÇÃO:**\


– Essa forma de apontamento é muito sensível e deve ser feita com muita atenção!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

– Utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em um formato diferente da orientação e/ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 2 dias** para propagar e surtir seus efeitos. Caso, após este prazo, elas não tenham funcionado como deveriam, por favor **entre em contato com o nosso suporte**!

**Nº3–** Entre as entradas que já existem na sua Zona DNS, procure uma entrada do tipo **A**, cujo Nome seja **@**.\
**Copie o número de IP** para qual ela está apontada e salve essa informação (você pode usar o Bloco de Notas para isso, se quiser).

**Exemplo:** na imagem, a primeira entrada **tem o Nome @** e é do tipo **A**.\
Ela está apontada para o número **156.67.222.223**. Então, no caso do exemplo, salvarei este número.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/hg3.png)

**Nº4–** Localize todas as entradas que sejam do tipo **CNAME** e que estejam apontadas para o seu domínio principal, ou seja, na coluna de **Conteúdo** conterá somente o seu domínio como valor.\
Salve qual é o Nome dela (_novamente, o Bloco de Notas pode ser seu amigo aqui_).

_**Observação:**_ Para essa configuração, a entrada “www” não será levada em consideração. Ela pode ser mantida como está.

**Exemplo:** a entrada **ftp**, do tipo **CNAME**, está apontada para **wikilovers.com.br** (o domínio que estamos usando de exemplo).\
Então vou salvar o nome dela (**ftp**).

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/hg4.png)

Faça isso com **todas** as entradas do tipo **CNAME** que estejam nesse padrão.

_**Observação:**_ Caso não tenha localizado nenhuma entrada que se encaixe nos critérios informados pule essa etapa e vá para o [apontamento do domínio](broken-reference).

### **Editando as entradas** <a href="#editar" id="editar"></a>

Vamos **editar **_**somente**_** as entradas de CNAME** que localizamos (você salvou o nome de todas elas, certo?) com as devidas informações, mas em um novo tipo.

**Observação:** A entrada do domínio principal veremos daqui à pouco.

Vamos lá!

**Nº5–** Clique em **Editar**

A entrada deve ser alterada da seguinte forma:

**Tipo:** altere para o tipo **A**.

**Nome:** deixe esse campo como está.

**Aponta para:** cole o número de IP que você salvou, lá no [passo **03**](broken-reference).

**TTL:** este campo virá automaticamente como **14400**. Caso tenha alguma informação diferente, altere para 14400.

**Nº6–** Verifique todos os dados e clique em **Atualizar**.\


![](https://legado.leadlovers.site/wp-content/uploads/2020/12/hg5.png)

**Nº7–** Repita os passos **05** e **06** e edite **todas** as outras entradas da lista que você tinha salvado antes.

### **Apontamento do domínio principal** <a href="#apontamento" id="apontamento"></a>

Agora sim, iremos fazer o apontamento do seu domínio para o nosso servidor.\
Algumas alterações aconteceram na forma de apontamento de domínios e no Hostinger o _**apontamento agora é por CNAME**_.

**Nº8–** Clique em **Editar**

A entrada deve ser alterada da seguinte forma:

**Tipo:** selecione o tipo **CNAME**.

**Nome:** novamente, deixe esse campo como está.

**TTL:** verifiquei se está como **14400**. Caso tenha alguma informação diferente, altere para 14400.

**Registro:** insira o nome do nosso servidor, **cname.leadlovers.site**

**Nº9–** Confira todos os dados e **Atualize** a entrada.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/hg8.png)

### **Entrada de WWW** <a href="#www" id="www"></a>

É preciso também fazer o apontamento da entrada de **www**. Assim, quem incluir estas letras na hora de digitar seu domínio no navegador, será direcionado normalmente para as suas páginas.

Se essa entrada já estiver na sua Zona de DNS você só precisa editá-la, agora, se ela não estiver será necessário criá-la.

**Entrada já está criada**

Muito provavelmente no seu Hostinger já existirá essa entrada do www.\
Localize a entrada cujo Nome é **www** e confirme se o Conteúdo está com o seu domínio sem o www. No exemplo, está somente wikilovers.com.br\
Caso a entrada já esteja configurada dessa forma, pule para conferir o [Resultado](broken-reference).

Agora, se o Tipo estiver como tipo A ou no Conteúdo estiver com qualquer outra informação, edite a entrada.

**Nº10–** Clique em **Editar**.

As informações da entrada serão:

Tipo: neste campo, selecione a opção **CNAME**.

Nome: coloque **www** (não inclua outros caracteres, letras, ou espaços em branco).

**TTL:** confirme se o campo está como **14400**.

Dados: no último campo campo, inclua o seu domínio **sem o www**. No exemplo, ficou somente wikilovers.com

**Nº11–** Confira todos os dados inclusos e clique em **Salvar** _OU_ **Adicionar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/hg10.png)

**Não tem a entrada**

**Nº12–** Vá para o topo da página, na parte de  Gerenciar registros DNS.

As informações da entrada serão:

Tipo: selecione a opção **CNAME**.

Nome: coloque **www** (não inclua outros caracteres, letras, ou espaços em branco).

Objeto: inclua o seu domínio **sem o www**. No exemplo, ficou somente wikilovers.com.br

**TTL:** verifiquei se está como **14400**.

**Nº13–** Confira todos os dados incluídos e clique em **Adicionar registro**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/hg13.png)

### **Resultado** <a href="#resultado" id="resultado"></a>

Ao final, você deve ter 2 entradas totais: 1 do domínio principal + 1 do www.\
As informações criadas ficarão similares às da imagem abaixo.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/hg-re.png)

Pronto! Agora seu domínio está corretamente apontado para o nosso servidor!

### **Cadastrando o domínio na máquina** <a href="#cadastrando-dominio" id="cadastrando-dominio"></a>

O próximo passo é adicionar este domínio na sua máquina! [**Clique aqui e veja o passo a passo**](https://suporte.love/como-cadastrar-dominio-maquina/).

**Artigos sugeridos**

– Se você caiu aleatoriamente aqui e não sabe o que é um domínio e nem como pode usá-lo dentro do nosso sistema, confira primeiro este artigo: [**o que é um domínio**](https://suporte.love/o-que-e-um-dominio/).

– Caso deseje entender melhor como funciona as entradas de uma Zona DNS **temos esse material aqui \[em breve]**.

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, **entre em contato com o nosso suporte**!

**É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
