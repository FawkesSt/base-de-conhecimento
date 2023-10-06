# Apontamento de domínio no UolHost

**Objetivo:** Mostrar o passo a passo de como utilizar o seu domínio que está no **Uolhost** dentro da leadlovers.\
**Para que serve:** O apontamento permite utilizar o seu domínio como endereço de acesso as páginas e/ou área de membro criadas dentro do sistema.\
**Requisito(s) necessário(s):** **1.** Ter um domínio próprio já comprado e **2.** ter acesso a Zona DNS do seu Uolhost.

&#x20;**IMPORTANTE:**\


**–** Os passos à seguir devem ser feitos **somente se o seu domínio for administrado pelo Uolhost**.\
Se ele estiver sob administração de outro serviço, é preciso que as configurações sejam realizadas no Painel de Controle específico deste segundo serviço. Nesse [artigo aqui](https://suporte.love/descobrir-cpanel/) nós mostramos como você pode confirmar qual é o painel do seu domínio.

**–** Caso seu domínio já seja utilizado para abrir um site feito em outra plataforma, apontá-lo para o nosso IP fará com que ele não abra mais estas páginas. **Seu site externo sairá do ar**.\
Se deseja manter seu domínio principal na forma como está, você pode criar uma entrada do tipo **subdomínio**. [**Clique aqui e veja nosso passo a passo, ensinando a criar um subdomínio!**](https://suporte.love/9729-2/)

### **Acessando a Zona DNS** <a href="#zona-dns" id="zona-dns"></a>

Após acessar seu [Painel do cliente](https://conta.uol.com.br/login?dest=http%3A%2F%2Fpainel.uol.com.br%2FmyProducts.html\&t=default) você verá uma tela inicial mostrando os seus produtos.

**Nº1–** Você pode acessar seus Domínios por meio de 2 caminhos: clicando na opção **Domínios** que tem no menu à esquerda OU na categoria Domínios, clique em **Administrar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/uh1.png)

**Nº2–** Também através de 2 caminhos é possível acessar a Zona DNS do seu domínio: clique na opção **Alterar Zona de DNS** no menu superior OU\
em **Seus domínios**, localize o domínio desejado, clique no botão de **Gerenciar** e então em **Alterar Zona de DNS**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/uh2.png)

**Nº3–** Agora sim, na tela de Alterar Zona de DNS, localize mais uma vez o domínio em questão e clique em **Gerenciar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/uh3.png)

### **Salvando as informações necessárias** <a href="#salvar" id="salvar"></a>

Dentro da próxima tela você verá diversas entradas já criadas e que direcionam o funcionamento das diversas funções de seu domínio. Essas entradas estão organizadas por **Tipos**.\
Como a Zona DNS do UolHost já vem com configurações nela antes de fazer qualquer apontamento precisamos primeiro salvar algumas informações! Ok?

&#x20;**ATENÇÃO:**\


– Essa forma de apontamento é muito sensível e deve ser feita com muita atenção!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

– Utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em um formato diferente da orientação e/ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 2 dias** para propagar e surtir seus efeitos. Caso, após este prazo, elas não tenham funcionado como deveriam, por favor **entre em contato com o nosso suporte**!

**Nº4–** Acesse as entradas do **tipo A** e localize uma entrada cujo nome seja somente o seu domínio, ou seja, ela não possui o primeiro nome.\
**Copie o número de IP** para qual ela está apontada e salve essa informação (você pode usar o Bloco de Notas para isso, se quiser).

**Exemplo:** na imagem, a entrada **wikilovers.com.br** não tem primeiro nome.\
Ela está apontada para o número **192.168.0.1**. Então, no caso do exemplo, salvarei este número.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/uh4.0.png)

_**Observação:**_ Se nas categoria do tipo A não constar nenhuma entrada, verifiquei o IP que consta na frase de introdução dessa tipo.\
Salve o IP que estiver ali e prossiga para o próximo passo.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/uh4.1.png)

**Nº5–** Agora, acesse a categoria do **tipo CNAME** e localize todas as entradas que estejam apontadas para o seu domínio principal, ou seja, na coluna **Destino** conterá somente o **seu domínio** como conteúdo.\
Salve qual é o primeiro nome delas (_novamente, o Bloco de Notas pode ser seu amigo aqui_).

_**Observação:**_ Para essa configuração, a entrada “www” não será levada em consideração. Ela pode ser mantida como está.

**Exemplo:** a entrada **ftp.wikilovers.com.br**, do tipo **CNAME**, está apontada para **wikilovers.com.br** (o domínio que estamos usando de exemplo).\
Então vou salvar o primeiro nome dela (**ftp**).

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/uh5.png)

Faça isso com **todas** as entradas do tipo **CNAME** que estejam nesse padrão.

_**Observação:**_ Caso não tenha localizado nenhuma entrada que se encaixe nos critérios informados pule essa etapa e vá para o [apontamento do domínio](broken-reference).

### **Excluindo entradas** <a href="#excluir" id="excluir"></a>

Depois que já salvou as informações, você precisa remover todas essas entradas (CNAMEs apontadas para seu domínio + a do domínio principal).

**Nº6–** No lado direito da entrada, clique no **ícone de lista**&#x20;

**Nº7–** E então clique na opção **Excluir**

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/uh6.png)

**Nº8–** Abrirá um pop-up confirmando se deseja remover o registro, clique em **Sim**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/12/uh8.png)

**Nº9–** Faça isso com todas as entradas das quais você guardou os dados.

### **Recriando as entradas** <a href="#recriar" id="recriar"></a>

Agora, vamos **recriar **_**somente**_** as entradas de CNAME** que localizamos (você salvou o nome de todas elas, certo?) com as devidas informações, mas em um novo tipo.

**Observação:** A entrada do domínio principal veremos daqui à pouco.

Vamos lá!

**Nº10–** Vá na categoria **Tipo A** e clique no botão **Criar nova entrada**. Uma nova faixa de opções vai aparecer, que é utilizada para adição de novas entradas.

Os dados da nova entrada devem ser preenchidos com as seguintes informações:

**Entrada:** coloque o **nome da entrada** que você salvou e está recriando (exemplo: **ftp**).

**Destino:** cole o número de IP que você salvou lá no [passo **04**](broken-reference).

**Status da entrada:** este campo virá automaticamente como **Ativado**. Caso tenha alguma informação diferente, altere para ativado.

**Nº11–** Verifique todos os dados e clique no visto ✔ para **Salvar**.\


![](https://legado.leadlovers.site/wp-content/uploads/2020/12/uh10.png)

**Nº12–** Repita os passos **10** e **11** e recrie **todas** as outras entradas da lista que você tinha salvado antes.

### **Apontamento do domínio principal** <a href="#apontamento" id="apontamento"></a>

Agora sim, iremos fazer o apontamento do seu domínio para o nosso servidor.\
Algumas alterações aconteceram na forma de apontamento de domínios e no Locaweb o _**apontamento agora é por CNAME**_.

**Nº13–** Então na categoria **Tipo CNAME**, clique novamente no botão **Criar nova entrada**.

A entrada deve ser criada da seguinte forma:

**Entrada:** esse campo deve ficar vazio.

**Destino:** insira o nome do nosso servidor, **cname.leadlovers.site**

**Status da entrada:** verifique se está como **Ativado**.

**Nº14–** Confira todos os dados e clique no visto ✔ para **Salvar**.

![](https://legado.leadlovers.site/wp-content/uploads/2017/02/uh14.png)

### **Entrada de WWW** <a href="#www" id="www"></a>

É preciso também fazer o apontamento da entrada de **www**. Assim, quem incluir estas letras na hora de digitar seu domínio no navegador, será direcionado normalmente para as suas páginas.

Geralmente, essa entrada está na categoria **Tipo CNAME**, mas pode ser que esteja na Tipo A. Então lembre de verificar essas 2 categorias, beleza?

_**Observação:**_ Caso esteja na categoria Tipo A, exclua a entrada que tiver ali e prossiga com a configuração pela categoria do Tipo CNAME.

Se essa entrada já estiver junto as entradas tipo CNAME você só precisa editá-la, agora, se ela não estiver será necessário criá-la.

**Nº15–** Clique no **ícone de lista e então em Editar** _OU_ no botão **Criar nova entrada**.

As informações da entrada serão:

Entrada: coloque **www** (não inclua outros caracteres, letras, ou espaços em branco).

Destino: neste campo, inclua o **seu domínio** **sem o www**. No exemplo, ficou somente wikilovers.com.br

**Status da entrada:** novamente, verifique se está como **Ativado**.

**Nº16–** Confira todos os dados inclusos e clique em **Salvar**.

![](https://legado.leadlovers.site/wp-content/uploads/2017/02/uh16.png)

### **Resultado** <a href="#resultado" id="resultado"></a>

Ao final, você deve ter 3 entradas totais: 2 dos IPs + 1 do www.\
As informações criadas ficarão similares às da imagem abaixo.

![](https://legado.leadlovers.site/wp-content/uploads/2017/02/uh-re.png)

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
