# Apontamento de domínio no KingHost

**Objetivo:** Mostrar o passo a passo de como utilizar o seu domínio que está no **KingHost** dentro da leadlovers.\
**Para que serve:** O apontamento permite utilizar o seu domínio como endereço de acesso as páginas e/ou área de membro criadas dentro do sistema.\
**Requisito(s) necessário(s):** **1.** Ter um domínio próprio já comprado e **2.** ter acesso a Zona DNS do seu KingHost.

&#x20;**IMPORTANTE:**\


**–** Os passos à seguir devem ser feitos **somente se o seu domínio for administrado pelo KingHost**.\
Se ele estiver sob administração de outro serviço, é preciso que as configurações sejam realizadas no Painel de Controle específico deste segundo serviço. Nesse [artigo aqui](https://suporte.love/descobrir-cpanel/) nós mostramos como você pode confirmar qual é o painel do seu domínio.

**–** Caso seu domínio já seja utilizado para abrir um site feito em outra plataforma, apontá-lo para o nosso IP fará com que ele não abra mais estas páginas. **Seu site externo sairá do ar**.\
Se deseja manter seu domínio principal na forma como está, você pode criar uma entrada do tipo **subdomínio**. [**Clique aqui e veja nosso passo a passo, ensinando a criar um subdomínio!**](https://suporte.love/como-criar-uma-entrada-de-subdominio-na-kinghost/)

### **Acessando a Zona DNS** <a href="#zona-dns" id="zona-dns"></a>

Após acessar seu [**KingHost**](https://painel.kinghost.com.br/login.php) você  verá uma dashboard.

**Nº1–** Em **Produtos configurados** localize o quadrado do domínio que deseja utilizar aqui no leadlovers e **clique em cima do domínio**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg1.png)

**Nº2–** Você será redirecionado para a tela de gerenciamento do domínio.\
Role para baixo e na parte de **Site**, clique na opção **Gerenciar DNS**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg2.png)

### **Salvando as informações necessárias** <a href="#salvar" id="salvar"></a>

Dentro da próxima tela terá diversas entradas já criadas e que direcionam o funcionamento das diversas funções de seu domínio.\
Como a Zona DNS do KingHost já vem com configurações nela antes de fazer qualquer apontamento precisamos primeiro salvar algumas informações! Ok?

![⚠](https://s.w.org/images/core/emoji/13.0.0/svg/26a0.svg) **ATENÇÃO:**\


– Essa forma de apontamento é muito sensível e deve ser feita com muita atenção!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

– Utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em um formato diferente da orientação e/ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 2 dias** para propagar e surtir seus efeitos. Caso, após este prazo, elas não tenham funcionado como deveriam, por favor **entre em contato com o nosso suporte**!

**Nº3–** Entre as entradas que já existem na sua Zona DNS, procure uma entrada do tipo **A**, cujo Host seja **@**.\
**Copie o número de IP** para qual ela está apontada e salve essa informação (você pode usar o Bloco de Notas para isso, se quiser).

**Exemplo:** na imagem, a primeira entrada **tem o Host @** e é do tipo **A**.\
Ela está apontada para o número **191.6.204.77**. Então, no caso do exemplo, salvarei este número.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg3.png)

**Nº4–** Localize todas as entradas que sejam do tipo **CNAME** e que estejam apontadas para o seu domínio principal, ou seja, na coluna **Destino** conterá somente um **@** _ou_ o seu domínio como conteúdo.\
Salve qual é o Host delas (_novamente, o Bloco de Notas pode ser seu amigo aqui_).

_**Observação:**_ Para essa configuração, a entrada “www” não será levada em consideração. Ela pode ser mantida como está.

**Exemplo:** a entrada **ftp**, do tipo **CNAME**, está com o **domínio principal** no campo Valor.\
Então vou salvar o nome dela (**ftp**).

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg4.png)

Faça isso com **todas** as entradas do tipo **CNAME** que estejam nesse padrão.

_**Observação:**_ Caso não tenha localizado nenhuma entrada que se encaixe nos critérios informados pule essa etapa e vá para o [apontamento do domínio](broken-reference).

### **Excluindo entradas** <a href="#excluir" id="excluir"></a>

Depois que já salvou as informações, você precisa remover as entradas CNAMEs apontadas para seu domínio.

**Nº5–** No lado direito da entrada, clique no **ícone X** para remover

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg5.png)

**Nº6–** No topo da página, abrirá um pop-up confirmando se deseja remover o registro, clique em **OK**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg6.png)

**Nº7–** Faça isso com todas as entradas CNAMEs das quais você guardou os dados.

### **Recriando as entradas** <a href="#recriar" id="recriar"></a>

Agora, vamos **recriar **_**somente**_** as entradas de CNAME** que localizamos (você salvou o nome de todas elas, certo?) com as devidas informações, mas em um novo tipo.

**Observação:** A entrada do domínio principal veremos daqui à pouco.

Vamos lá!

**Nº8–** Vá ao início de sua tela, na parte de **Inserir DNS**.&#x20;

Os dados da nova entrada devem ser preenchidos com as seguintes informações:

**Host:** coloque o **nome da entrada** que você está recriando (exemplo: **ftp**).

**Tipo:** escolha a opção **Address (A)**.

**Destino:** cole o número de IP que você salvou, lá no [passo **03**](broken-reference).

**Nº9–** Verifique todos os dados e clique em **Inserir DNS**.\


![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg9.png)

**Nº10–** Repita os passos **08** e **09** e recrie **todas** as outras entradas da lista que você tinha salvado antes.

### **Apontamento do domínio principal** <a href="#apontamento" id="apontamento"></a>

Agora sim, iremos fazer o apontamento do seu domínio para o nosso servidor. Atualmente, **o apontamento para leadlovers é feito para **_**2 IPs**_.

**Nº11–** Localize a entrada do seu domínio principal, aquela do [passo 03](broken-reference), e clique **em cima dos campos** para editá-los.

A entrada deve ser alterada da seguinte forma:

**Host:** deixe esse campo como está.

**Destino:** insira o número do IP primário do nosso servidor, **213.136.68.210**

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg11.png)

**Nº12–** Verifique todos os dados, role para baixo e clique em **Alterar DNS**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg12.png)

**Nº13–** Ache novamente a opção de **Inserir DNS** (a do [passo **08**](broken-reference)) no topo da página.

E para inserir o nosso IP secundário (redundância/backup) basta repetir o processo.\
A diferença está na informação que você irá inserir no campo Dados.

**Host:** insira o símbolo de **@** (arroba). É essa informação que irá indicar que aquela entrada é referente ao domínio principal.

**Tipo:** selecione o tipo **Address (A)**.

Destino: o IP dessa vez será **213.136.70.54**

**Nº14–** Insira o DNS para criar a nova entrada.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg13.png)

### **Entrada de WWW** <a href="#www" id="www"></a>

É preciso também fazer o apontamento da entrada de **www**. Assim, quem incluir estas letras na hora de digitar seu domínio no navegador, será direcionado normalmente para as suas páginas.

Se essa entrada já estiver na sua Zona de DNS você só precisa editá-la, agora, se ela não estiver será necessário criá-la.

**Entrada já está criada**

Muito provavelmente no seu KingHost já existirá essa entrada do www.\
Localize a entrada cujo Host é **www** e confirme se o Destino está com o seu domínio sem o www. ou com um @.\
Se a entrada já estiver configurada dessa forma, pule para conferir o [Resultado](broken-reference).

_Observação: Caso_ no Tipo estiver como tipo A, exclua a entrada e prossiga para criar o registro igual mostramos abaixo para o pessoal que [não tem a entrada](https://legado.leadlovers.site/apontamento-dominio-locaweb/#sem-entrada).

Agora, se no Destino estiver com qualquer outra informação, edite a entrada.

**Nº15–** Clique **em cima dos campos** para editar.

As informações da entrada serão:

Host: confirme se está somente como **www** (sem outros caracteres, letras, ou espaços em branco).

Destino: neste campo, inclua o o seu domínio **sem o www**. No exemplo, ficou somente wikilovers.com.br

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg15.png)

**Nº16–** Role a tela para baixo e clique em **Alterar DNS**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg16.png)

**Não tem a entrada**

**Nº17–** Vá para o topo da página, na parte de  Inserir DNS.

As informações da entrada serão:

Host: coloque **www** (não inclua outros caracteres, letras, ou espaços em branco).

Tipo: selecione a opção **CNAME**.

Destino: inclua o seu domínio **sem o www**. No exemplo, ficou somente wikilovers.com.br

**Nº18–** Confira todos os dados inclusos e clique em **Inserir DNS**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg18.png)

### **Resultado** <a href="#resultado" id="resultado"></a>

Ao final, você deve ter 3 entradas totais: 2 dos IPs + 1 do www.\
As informações criadas ficarão similares às da imagem abaixo.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/kg-re.png)

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
