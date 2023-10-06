# Apontamento de domínio no GoDaddy

**Objetivo:** Mostrar o passo a passo de como utilizar o seu domínio que está no **GoDaddy** dentro da leadlovers.\
**Para que serve:** O apontamento permite utilizar o seu domínio como endereço de acesso as páginas e/ou área de membro criadas dentro do sistema.\
**Requisito(s) necessário(s):** **1.** Ter um domínio próprio já comprado e **2.** ter acesso a Zona DNS do seu GoDaddy.

&#x20;**IMPORTANTE:**\


**–** Os passos à seguir devem ser feitos **somente se o seu domínio for administrado pelo GoDaddy**.\
Se ele estiver sob administração de outro serviço, é preciso que as configurações sejam realizadas no Painel de Controle específico deste segundo serviço. Nesse [artigo aqui](https://suporte.love/descobrir-cpanel/) nós mostramos como você pode confirmar qual é o painel do seu domínio.

**–** Caso seu domínio já seja utilizado para abrir um site feito em outra plataforma, apontá-lo para o nosso IP fará com que ele não abra mais estas páginas. **Seu site externo sairá do ar**.\
Se deseja manter seu domínio principal na forma como está, você pode criar uma entrada do tipo **subdomínio**. [**Clique aqui e veja nosso passo a passo, ensinando a criar um subdomínio!**](https://suporte.love/como-criar-uma-entrada-de-subdominio-na-godaddy/)

### **Acessando a Zona DNS** <a href="#zona-dns" id="zona-dns"></a>

Após acessar seu [**GoDaddy**](https://sso.godaddy.com/?realm=idp\&path=%2fproducts\&app=account) você verá uma tela mostrando os seus Produtos.

**Nº1–** Na categoria Domínios, localize o quadrado do domínio que deseja utilizar aqui no leadlovers e clique nos **3 pontinhos**.\
**Nº2–** E em seguida, clique na opção **Gerenciar DNS**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/gd1.png)

### **Salvando as informações necessárias** <a href="#salvar" id="salvar"></a>

Dentro da próxima tela, chamada **Registros**, você vai ver diversas entradas já criadas e que direcionam o funcionamento das diversas funções de seu domínio.\
Como a Zona DNS do GoDaddy já vem com configurações nela antes de fazer qualquer apontamento precisamos primeiro salvar algumas informações! Ok?

&#x20;**ATENÇÃO:**\


– Essa forma de apontamento é muito sensível e deve ser feita com muita atenção!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

– Utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em um formato diferente da orientação e/ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 2 dias** para propagar e surtir seus efeitos. Caso, após este prazo, elas não tenham funcionado como deveriam, por favor **entre em contato com o nosso suporte**!

**Nº3–** Entre as entradas que já existem na sua Zona DNS, procure uma entrada do tipo **A**, cujo Nome seja **@**.\
**Copie o número de IP** para qual ela está apontada e salve essa informação (você pode usar o Bloco de Notas para isso, se quiser).

**Exemplo:** na imagem, a primeira entrada **tem o Nome @** e é do tipo **A**.\
Ela está apontada para o número **160.153.53.32**. Então, no caso do exemplo, salvarei este número.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/gd3.png)

**Nº4–** Localize todas as entradas que sejam do tipo **CNAME** e que estejam apontadas para o seu domínio principal, ou seja, na coluna **Valor** conterá somente um **@** como conteúdo.\
Salve qual é o Nome delas (_novamente, o Bloco de Notas pode ser seu amigo aqui_).

_**Observação:**_ Para essa configuração, a entrada “www” não será levada em consideração. Ela pode ser mantida como está.

**Exemplo:** a entrada **ftp**, do tipo **CNAME**, está com o **@** no campo Valor.\
Então vou salvar o nome dela (**ftp**).

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/gd4.png)

Faça isso com **todas** as entradas do tipo **CNAME** que estejam nesse padrão.

_**Observação:**_ Caso não tenha localizado nenhuma entrada que se encaixe nos critérios informados pule essa etapa e vá para o [apontamento do domínio](broken-reference).

### **Excluindo entradas** <a href="#excluir" id="excluir"></a>

Depois que já salvou as informações, você precisa remover as entradas CNAMEs apontadas para seu domínio.

**Nº5–** No lado direito da entrada, clique no **ícone de lápis para Editar**

**Nº6–** E então clique na **Lixeira**

**Nº7–** Abrirá um pop-up confirmando se deseja remover o registro, clique em **Excluir**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/gd5.png)

**Nº8–** Faça isso com todas as entradas CNAMEs das quais você guardou os dados.

### **Recriando as entradas** <a href="#recriar" id="recriar"></a>

Agora, vamos **recriar **_**somente**_** as entradas de CNAME** que localizamos (você salvou o nome de todas elas, certo?) com as devidas informações, mas em um novo tipo.

**Observação:** A entrada do domínio principal veremos daqui à pouco.

Vamos lá!

**Nº9–** Vá até o final de sua tela de Registros, ache e clique no botão **Adicionar**. Uma nova faixa de opções vai aparecer, que é utilizada para adição de novas entradas.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/gd9.png)

Os dados da nova entrada devem ser preenchidos com as seguintes informações:

**Tipo:** escolha a opção **A**. Os demais campos da entrada aparecerão logo em seguida.

**Host:** coloque o **nome da entrada** que você está recriando (exemplo: **ftp**).

**Aponta para:** cole o número de IP que você salvou, lá no [passo **03**](broken-reference).

**TTL:** este campo virá automaticamente como **1 hora**. Caso tenha alguma informação diferente, altere para 1 hora.

**Nº10–** Verifique todos os dados e clique em **Salvar**.\


![](https://legado.leadlovers.site/wp-content/uploads/2020/11/gd10.png)

**Nº11–** Repita os passos **09** e **10** e recrie **todas** as outras entradas da lista que você tinha salvado antes.

### **Apontamento do domínio principal** <a href="#apontamento" id="apontamento"></a>

Agora sim, iremos fazer o apontamento do seu domínio para o nosso servidor. Atualmente, **o apontamento para leadlovers é feito para **_**2 IPs**_.

**Nº12–** Localize a entrada do seu domínio principal, aquela do [passo 03](broken-reference), e clique **ícone de lápis para Editar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/gd12.png)

A entrada deve ser alterada da seguinte forma:

**Host:** deixe esse campo como está.

**Aponta para:** insira o número do IP primário do nosso servidor, **213.136.68.210**

**TTL:** deve ficar como **1 hora**.

**Nº13–** Verifique todos os dados e clique em **Salvar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/gd13.png)

**Nº14–** Ache novamente o botão **Adicionar** (o do [passo **09**](broken-reference)) e clique nele novamente.

E para inserir o nosso IP secundário (redundância/backup) basta repetir o processo.\
A diferença está na informação que você irá inserir no campo Dados.

**Tipo:** selecione o tipo **A**. Os demais campos da entrada aparecerão logo em seguida.

**Host:** insira o símbolo de **@** (arroba). É essa informação que irá indicar que aquela entrada é referente ao domínio principal.

Aponta para: o IP dessa vez será **213.136.70.54**

**TTL:** confirme se o campo está como **1 hora**.

**Nº15–** Salve para criar a nova entrada criada.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/gd15.png)

### **Entrada de WWW** <a href="#www" id="www"></a>

É preciso também fazer o apontamento da entrada de **www**. Assim, quem incluir estas letras na hora de digitar seu domínio no navegador, será direcionado normalmente para as suas páginas.

Se essa entrada já estiver na sua Zona de DNS você só precisa editá-la, agora, se ela não estiver será necessário criá-la.

**Nº16–** Clique em **Editar** _OU_ **Adicionar**.

As informações da entrada serão:

Host: coloque **www** (não inclua outros caracteres, letras, ou espaços em branco).

Aponta para: neste campo, inclua o **@**.

**TTL:** verifique se o campo está **1 hora**.

**Nº17–** Confira todos os dados inclusos e clique em **Salvar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/gd17.png)

### **Resultado** <a href="#resultado" id="resultado"></a>

Ao final, você deve ter 3 entradas totais: 2 dos IPs + 1 do www.\
As informações criadas ficarão similares às da imagem abaixo.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/gd-re.png)

Pronto! Agora seu domínio está corretamente apontado para o nosso servidor!

### **Cadastrando o domínio na máquina** <a href="#cadastrando-dominio" id="cadastrando-dominio"></a>

O próximo passo é adicionar este domínio na sua máquina! [**Clique aqui e veja o passo a passo**](https://suporte.love/como-cadastrar-dominio-maquina/).

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, entre em contato com o nosso suporte!

**Artigos sugeridos**

– Se você caiu aleatoriamente aqui e não sabe o que é um domínio e nem como pode usá-lo dentro do nosso sistema, confira primeiro este artigo: [**o que é um domínio**](https://suporte.love/o-que-e-um-dominio/).

**É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
