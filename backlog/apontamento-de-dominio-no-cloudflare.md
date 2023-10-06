# Apontamento de domínio no Cloudflare

**Objetivo:** Mostrar o passo a passo de como utilizar o seu domínio que está no Cloudflare dentro da leadlovers.\
**Para que serve:** O apontamento permite utilizar o seu domínio como endereço de acesso as páginas e/ou área de membro criadas dentro do sistema.\
**Requisito(s) necessário(s):** **1.** Ter um domínio próprio já comprado e **2.** ter acesso a Zona DNS do seu Cloudflare.

**IMPORTANTE:**\


**–** Os passos à seguir devem ser feitos **somente se o seu domínio for administrado pelo Cloudflare**.\
Se ele estiver sob administração de outro serviço, é preciso que as configurações sejam realizadas no Painel de Controle específico deste segundo serviço. Nesse [artigo aqui](https://suporte.love/descobrir-cpanel/) nós mostramos como você pode confirmar qual é o painel do seu domínio.

**–** Caso seu domínio já seja utilizado para abrir um site feito em outra plataforma, apontá-lo para o nosso IP fará com que ele não abra mais estas páginas. **Seu site externo sairá do ar**.\
Se deseja manter seu domínio principal na forma como está, você pode criar uma entrada do tipo **subdomínio**. [**Clique aqui e veja nosso passo a passo, ensinando a criar um subdomínio!**](https://suporte.love/como-criar-uma-entrada-de-subdominio-no-cloudflare/)

### **Acessando o Cpanel de seu domínio** <a href="#zona-dns" id="zona-dns"></a>

Após logar no seu [**Cloudflare**](https://dash.cloudflare.com/login) verá uma lista com todos os domínios cadastrados por lá.

**Nº1–** Clique sobre o domínio que deseja usar em sua máquina aqui no leadlovers.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/cl1.png)

**Nº2–** Você será redirecionado para a tela de gerenciamento do seu domínio.\
Nessa tela, na parte superior terá um conjunto de ícones azuis, clique sobre a opção **DNS**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/cl2.png)

### **Salvando as informações necessárias** <a href="#salvar" id="salvar"></a>

Normalmente, a Zona DNS no Cloudflare já vem com configurações nela e, por isso, antes de fazer qualquer apontamento precisamos primeiro salvar algumas informações! Ok?

&#x20;**ATENÇÃO:**\


– Essa forma de apontamento é muito sensível e deve ser feita com muita atenção!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

– Utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em um formato diferente da orientação e/ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 2 dias** para propagar e surtir seus efeitos. Caso, após este prazo, elas não tenham funcionado como deveriam, por favor **entre em contato com o nosso suporte**!

**Nº3–** Entre as entradas que já existem na sua Zona DNS, procure uma entrada do tipo **A**, cujo Nome esteja como o seu domínio. Essa é a entrada principal do seu domínio.\
**Copie o número de IP** para qual ela está apontada e salve essa informação (você pode usar o Bloco de Notas para isso, se quiser).

**Exemplo:** na imagem, a entrada **wikilovers.com.br** é do tipo **A** e o seu nome é somente o domínio.\
Ela está apontada para o número **192.185.217.220**. Então, no caso do exemplo, salvarei este número.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/cl3.png)

**Nº4–** Localize todas as entradas que sejam do tipo **CNAME** e que estejam apontadas para o seu domínio principal, ou seja, na coluna de Conteúdo conterá somente o seu domínio como valor.\
Salve qual é o Nome delas (_novamente, o Bloco de Notas pode ser seu amigo aqui_).

_**Observação:**_ Para essa configuração, a entrada “www” não será levada em consideração. Ela pode ser mantida como está.

**Exemplo:** a entrada **ftp**, do tipo **CNAME**, está apontada para **wikilovers.com.br** (o domínio que estamos usando de exemplo).\
Então vou salvar o Nome dela (**ftp**).

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/cl4.png)

Faça isso com **todas** as entradas do tipo **CNAME** que estejam nesse padrão.

_**Observação:**_ Caso não tenha localizado nenhuma entrada que se encaixe nos critérios informados pule essa etapa e vá para o [apontamento do domínio](broken-reference).

### **Excluindo entradas** <a href="#excluir" id="excluir"></a>

Depois que já salvou as informações, você precisa remover todas essas entradas (CNAMEs apontadas para seu domínio + a do domínio principal).

**Nº5–** Clique em **Editar**

**Nº6–** E então em **Excluir**

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/cl5.png)

**Nº7–** Abrirá um pop-up confirmando se deseja remover o registro, clique novamente em **Excluir**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/cl7.png)

**Nº8–** Faça isso com todas as entradas das quais você guardou os dados.

### **Recriando as entradas** <a href="#recriar" id="recriar"></a>

Agora, vamos **recriar **_**somente**_** as entradas de CNAME** que apagamos (você salvou o nome de todas elas, certo?) com as devidas informações, mas em um novo tipo.

**Observação:** A entrada do domínio principal veremos daqui à pouco.

Vamos lá!

**Nº9–** Clique no botão **+Adicionar registro**.

A entrada deve ser preenchida com as seguintes informações:

**Tipo:** neste campo, verifique se está o tipo **A**.

**Nome:** aqui, coloque o **nome da entrada** que você salvou (exemplo: **ftp**).

**Registro/Endereço IPv4:** já neste campo, cole o número de IP que você guardou lá no passo **03**.

**TTL:** este campo virá automaticamente como **Auto**, o mantenha assim.

**Status do proxy:** virá como **Com proxy** automaticamente (a nuvenzinha estará laranja), deixe como está.

**Nº10–** Verifique todos os dados e clique em **Salvar**.\


![](https://legado.leadlovers.site/wp-content/uploads/2020/11/cl9.png)

**Nº11–** Repita os passos **09** e **10** e recrie **todas** as outras entradas da lista que você tinha salvado as informações antes.

### **Apontamento do domínio principal** <a href="#apontamento" id="apontamento"></a>

Agora sim, iremos fazer o apontamento do seu domínio para o nosso servidor.\
Algumas alterações aconteceram na forma de apontamento de domínios e no Cloudflare o _**apontamento agora é por CNAME**_.

**Nº12–** Clique no botão **+Adicionar registro**.

A entrada deve ser criada da seguinte forma:

**Tipo:** selecione o tipo **CNAME**.

**Nome:** aqui você irá preencher com o símbolo **@** (arroba). É essa informação que irá indicar que aquela entrada é referente ao domínio principal.

**Destino:** insira o nome do nosso servidor, **cname.leadlovers.site**

**TTL:** deixe como **Auto**.

**Status do proxy**: clique em cima da nuvenzinha para desabilitar essa opção, a nuvem deve ficar cinza e com a informação de **Somente DNS (only DNS)**.

**Nº13–** Verifique todos os dados e clique em **Salvar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/cl12.png)

### **Entrada de WWW** <a href="#www" id="www"></a>

É preciso também conferir como está o apontamento da entrada de **www**. Assim, quem incluir estas letras na hora de digitar seu domínio no navegador, será direcionado normalmente para as suas páginas.

Se essa entrada já estiver na sua Zona de DNS você só precisa editá-la, agora, se ela não estiver será necessário criá-la.

**ENTRADA JÁ ESTÁ CRIADA**

Muito provavelmente, no seu Cloudflare já existirá essa entrada do www.\
Nesse caso, a configuração necessária é bem simples.

**Nº14–** Localize a entrada cujo Nome é **www** e confirme se o Conteúdo está com o seu domínio sem o www. No exemplo, está somente wikilovers.com.br\
Se no Conteúdo estiver com qualquer outra informação, prossiga para editar o registro igual mostramos abaixo para o pessoal que [não tem a entrada](broken-reference).

**Nº15–** Se estiver tudo ok com a entrada a única configuração necessária é **desativar o proxy**.\
Clique em cima da nuvenzinha para desabilitar essa opção, a nuvem deve ficar cinza e com a informação de **Somente DNS (only DNS)**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/cl15.png)

**NÃO TEM A ENTRADA**

**Nº16–** Clique em **+Adicionar registro** _OU_ **Editar**.

As informações da entrada serão:

Tipo: selecione a opção **CNAME**.

Nome: coloque **www** (não inclua outros caracteres, letras, ou espaços em branco).

Destino: inclua o seu domínio **sem o www**. No exemplo, ficou somente wikilovers.com.br

**TTL:** deixe como **Auto**.

**Status do proxy**: clique em cima da nuvenzinha para desabilitar essa opção, a nuvem deve ficar cinza e com a informação de **Somente DNS (only DNS)**.

**Nº17–** Confira todos os dados inclusos e clique em **Salvar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/cl16.png)

### **Resultado** <a href="#resultado" id="resultado"></a>

Ao final, você deve ter 2 entradas totais: 1 do domínio principal + 1 do www.\
As informações criadas ficarão similares às da imagem abaixo.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/cl-re.png)

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
