# Apontamento de domínio no WiX

**Objetivo:** Mostrar o passo a passo de como utilizar o seu domínio que está no **WiX** dentro da leadlovers.\
**Para que serve:** O apontamento permite utilizar o seu domínio como endereço de acesso as páginas e/ou área de membro criadas dentro do sistema.\
**Requisito(s) necessário(s):** **1.** Ter um domínio próprio já comprado e **2.** ter acesso a Zona DNS do seu WiX.

&#x20;**IMPORTANTE:**\


**–** Os passos à seguir devem ser feitos **somente se o seu domínio for administrado pelo WiX**.\
Se ele estiver sob administração de outro serviço, é preciso que as configurações sejam realizadas no Painel de Controle específico deste segundo serviço. Nesse [artigo aqui](https://suporte.love/descobrir-cpanel/) nós mostramos como você pode confirmar qual é o painel do seu domínio.

**–** Caso seu domínio já seja utilizado para abrir um site feito em outra plataforma, apontá-lo para o nosso IP fará com que ele não abra mais estas páginas. **Seu site externo sairá do ar**.\
Se deseja manter seu domínio principal na forma como está, você pode criar uma entrada do tipo **subdomínio**. [**Clique aqui e veja nosso passo a passo, ensinando a criar um subdomínio!**](https://suporte.love/como-criar-uma-entrada-de-subdominio-no-wix/)

### **Acessando a Zona DNS** <a href="#zona-dns" id="zona-dns"></a>

Após acessar seu [**WiX**](https://users.wix.com/signin) você verá uma lista com todos os sites cadastrados por lá.

**Nº1–** Localize o quadrado do domínio que deseja utilizar aqui no leadlovers e clique em **Selecionar e Editar Site**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx1.png)

**Nº2–** Você pode acessar o gerenciamento do seu domínios por meio de 2 caminhos: passando o mouse em cima da opção **Configurações** e então clicando em **Domínios** que tem no menu à esquerda OU na nas informações do seu site, clique em **Gerenciar domínio**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx2.png)

**Nº3–** Você será redirecionado para uma tela com a lista dos seus domínios cadastrados no WiX.\
Mais uma vez, encontre o domínio que deseja usar nas páginas da leadlovers e clique nos **3 pontinhos**.

**Nº4–** E então em **Gerenciar registros DNS** para acessar a Zona de DNS.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx3.png)

### **Salvando as informações necessárias** <a href="#salvar" id="salvar"></a>

Dentro da próxima tela você verá diversas entradas já criadas e que direcionam o funcionamento das diversas funções de seu domínio. Essas entradas estão organizadas por **Tipos**.\
Como a Zona DNS do WiX já vem com configurações nela antes de fazer qualquer apontamento precisamos primeiro salvar algumas informações! Ok?

![⚠](https://s.w.org/images/core/emoji/13.0.0/svg/26a0.svg) **ATENÇÃO:**\


– Essa forma de apontamento é muito sensível e deve ser feita com muita atenção!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

– Utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em um formato diferente da orientação e/ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 2 dias** para propagar e surtir seus efeitos. Caso, após este prazo, elas não tenham funcionado como deveriam, por favor **entre em contato com o nosso suporte**!

**Nº5–** Nas entradas do **A (Host)** que já existem na sua Zona DNS, procure uma entrada cujo nome seja somente o seu domínio, ou seja, ela não possui o primeiro nome.\
**Copie o número de IP** para qual ela está apontada e salve essa informação (você pode usar o Bloco de Notas para isso, se quiser).

**Exemplo:** na imagem, a entrada **wikilovers.com.br** não tem primeiro nome.\
Ela está apontada para o número **23.236.62.147**. Então, no caso do exemplo, salvarei este número.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx5.png)

**Nº6–** Agora, nas entradas da categoria **Registro CNAME (Aliases)**, localize todas as entradas que estejam apontadas para o seu domínio principal, ou seja, na coluna **Valor** conterá somente o **seu domínio** como conteúdo.\
Salve qual é o primeiro nome delas (_novamente, o Bloco de Notas pode ser seu amigo aqui_).

_**Observação:**_ Para essa configuração, a entrada “www” não será levada em consideração. Ela pode ser mantida como está.

**Exemplo:** a entrada **ftp.wikilovers.com.br**, do tipo **CNAME**, está com o **wikilovers.com.br** (o domínio que estamos usando de exemplo).\
Então vou salvar o primeiro nome dela (**ftp**).

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx6.png)

Faça isso com **todas** as entradas do tipo **CNAME** que estejam nesse padrão.

_**Observação:**_ Caso não tenha localizado nenhuma entrada que se encaixe nos critérios informados pule essa etapa e vá para o [apontamento do domínio](broken-reference).

### **Excluindo entradas** <a href="#excluir" id="excluir"></a>

Depois que já salvou as informações, você precisa remover as entradas CNAMEs apontadas para seu domínio.

**Nº7–** No lado direito da entrada, clique nos **3 pontinhos**

**Nº8–** E então clique em **Excluir**

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx7.png)

**Nº9–** Abrirá um pop-up confirmando se deseja remover o registro, clique em **Excluir Registro**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx9.png)

**Nº10–** Faça isso com todas as entradas CNAMEs das quais você guardou os dados.

### **Recriando as entradas** <a href="#recriar" id="recriar"></a>

Agora, vamos **recriar **_**somente**_** as entradas de CNAME** que localizamos (você salvou o nome de todas elas, certo?) com as devidas informações, mas em um novo tipo.

**Observação:** A entrada do domínio principal veremos daqui à pouco.

Vamos lá!

**Nº11–** Vá na categoria **A (Host)** e clique no botão **+ Adicionar registro** que terá no final da mesma.

Os dados da nova entrada devem ser preenchidos com as seguintes informações:

**Nome do Host:** coloque o **nome da entrada** que você salvou e está recriando (exemplo: **ftp**).

**Valor:** cole o número de IP que você salvou lá no [passo **05**](broken-reference).

**TTL:** este campo virá automaticamente como **1 hora**. Caso tenha alguma informação diferente, altere para 1 hora.

**Nº12–** Verifique todos os dados e clique em **Salvar**.\


![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx11.png)

**Nº13–** Repita os passos 11 e **12** e recrie **todas** as outras entradas da lista que você tinha salvado antes.

### **Apontamento do domínio principal** <a href="#apontamento" id="apontamento"></a>

Agora sim, iremos fazer o apontamento do seu domínio para o nosso servidor. Atualmente, **o apontamento para leadlovers é feito para **_**2 IPs**_.

**Nº14–** Localize a entrada do seu domínio principal, aquela do [passo 05](broken-reference), passe o mouse em cima da mesma e clique no botão **Editar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx14.png)

A entrada deve ser alterada da seguinte forma:

**Nome do Host:** esse campo deve ficar **vazio**.

**Valor:** insira o número do IP primário do nosso servidor, **213.136.68.210**

**TTL:** deve ficar como **1 hora**.

**Nº15–** Verifique todos os dados e clique em **Salvar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx15.png)

**Nº16–** Clique no botão **+ Adicionar registro**.

E para inserir o nosso IP secundário (redundância/backup) basta repetir o processo.\
A diferença está na informação que você irá inserir no campo Valor.

**Nome do Host:** novamente, o campo deve ficar **vazio**.

Aponta para: o IP dessa vez será **213.136.70.54**

**TTL:** confirme se o campo está como **1 hora**.

**Nº17–** Salve para criar a nova entrada criada.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx16.png)

### **Entrada de WWW** <a href="#www" id="www"></a>

É preciso também fazer o apontamento da entrada de **www**. Assim, quem incluir estas letras na hora de digitar seu domínio no navegador, será direcionado normalmente para as suas páginas.

Geralmente, essa entrada está na categoria **Registro CNAME (Aliases)**, mas pode ser que esteja na A (Host). Então lembre de verificar essas 2 categorias, beleza?

_**Observação:**_ Caso esteja na categoria tipo A, exclua a entrada que tiver ali e prossiga com a configuração pela categoria do tipo CNAME.

Se essa entrada já estiver junto as entradas de CNAME você só precisa editá-la, agora, se ela não estiver será necessário criá-la.

**Nº18–** Passe o mouse por cima da entrada e clique em **Editar** _OU_ no final da categoria, clique em **+ Adicionar registro**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx18.png)

As informações da entrada serão:

Nome do Host: coloque **www** (não inclua outros caracteres, letras, ou espaços em branco).

Valor: neste campo, inclua o **seu domínio** **sem o www**. No exemplo, ficou somente wikilovers.com.br .

**TTL:** verifique se o campo está **1 hora**.

**Nº19–** Confira todos os dados inclusos e clique em **Salvar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx19.png)

### **Resultado** <a href="#resultado" id="resultado"></a>

Ao final, você deve ter 3 entradas totais: 2 dos IPs + 1 do www.\
As informações criadas ficarão similares às da imagem abaixo.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx-re.png)

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
