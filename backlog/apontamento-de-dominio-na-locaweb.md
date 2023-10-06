# Apontamento de domínio na Locaweb

**Objetivo:** Mostrar o passo a passo de como utilizar o seu domínio que está na Locaweb dentro da leadlovers.\
**Para que serve:** O apontamento permite utilizar o seu domínio como endereço de acesso as páginas e/ou área de membros criadas dentro do sistema.\
**Requisito(s) necessário(s):** **1.** Ter um domínio próprio já comprado e **2.** ter acesso a Zona DNS da Locaweb.

&#x20;**IMPORTANTE:**\


**–** Os passos a seguir devem ser feitos **somente se o seu domínio for administrado pela Locaweb**.\
Se ele estiver sob administração de outro serviço, é preciso que as configurações sejam realizadas no Painel de Controle específico deste segundo serviço. Nesse [artigo aqui](https://legado.leadlovers.site/descobrir-hospedagem/) nós mostramos como você pode confirmar qual é o painel do seu domínio.

**–** Caso seu domínio já seja utilizado para abrir um site feito em outra plataforma, apontá-lo para o nosso IP fará com que ele não abra mais estas páginas. **Seu site externo sairá do ar**.\
Se deseja manter seu domínio principal na forma como está, você pode criar uma entrada do tipo **subdomínio**. [**Clique aqui e veja nosso passo a passo ensinando a criar um subdomínio!**](https://legado.leadlovers.site/como-criar-uma-entrada-de-subdominio-no-locaweb/)

### **Acessando a Zona de DNS de seu domínio** <a href="#zona-dns" id="zona-dns"></a>

Após logar na [**Locaweb**](https://www.locaweb.com.br/), você verá os Produtos que possui.

**Nº1–** Clique em **Hospedagem de Sites**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw1.png)

**Nº2–** Abrirá uma nova guia e nela terá uma lista com todos os domínios cadastrados por lá.\
Localize o domínio que deseja usar em sua máquina aqui na leadlovers e clique no ícone de engrenagem.

**Nº3–** Selecione então a opção **Zona de DNS** e, de novo, você será redirecionado a uma nova guia.\


[![](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw2.png)](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw2.png)

### **Salvando as informações necessárias** <a href="#salvar" id="salvar"></a>

Normalmente, a Zona DNS da Locaweb já vem com configurações nela e, por isso, antes de fazer qualquer apontamento precisamos primeiro salvar algumas informações! Ok?

&#x20;**ATENÇÃO:**\


– Essa forma de apontamento é muito sensível e deve ser feita com muita atenção!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

– Utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em um formato diferente da orientação e/ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 2 dias** para propagar e surtir seus efeitos. Caso, após este prazo, elas não tenham funcionado como deveriam, por favor, **entre em contato com o nosso suporte**!

**Nº4–** Entre as entradas que já existem na sua Zona DNS, procure uma entrada do tipo **A**, cujo nome esteja como um **ponto** ( **.** ). Essa é a entrada principal do seu domínio.\
**Copie o número de IP** para qual ela está apontada e salve essa informação (_você pode usar o Bloco de Notas para isso, se quiser_).

**Exemplo:** na imagem, a primeira entrada ” **.** ” é do tipo **A** e está apontada para o número **191.252.51.36**. Então, no caso do exemplo, salvarei este número.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/02/lw4.png)](https://legado.leadlovers.site/wp-content/uploads/2017/02/lw4.png)

**Nº5–** Localize todas as entradas que sejam do tipo **CNAME** e que estejam apontadas para o seu domínio principal, ou seja, na coluna de Conteúdo conterá somente o seu domínio como valor.\
Salve qual é o nome delas (_novamente, o Bloco de Notas pode ser seu amigo aqui_).

_**Observação:**_ Para essa configuração, a entrada “www” não será levada em consideração. Ela pode ser mantida como está.

**Exemplo:** a entrada **ftp**, do tipo **CNAME**, está apontada para **wikilovers.com.br** (o domínio que estamos usando de exemplo).\
Então vou salvar o Nome dela (**ftp**).

[![](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw5.png)](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw5.png)

Faça isso com **todas** as entradas do tipo **CNAME** que estejam nesse padrão.

_**Observação:**_ Caso não tenha localizado nenhuma entrada que se encaixe nos critérios informados, pule essa etapa e vá para o [apontamento do domínio](broken-reference).

### **Excluindo entradas** <a href="#excluir" id="excluir"></a>

Depois que já salvou as informações, você precisa remover todas essas entradas (CNAMEs apontadas para seu domínio).

**Nº6–** Clique em **Excluir**

[![](https://legado.leadlovers.site/wp-content/uploads/2017/02/lw6.png)](https://legado.leadlovers.site/wp-content/uploads/2017/02/lw6.png)

**Nº7–** Abrirá um pop-up confirmando se deseja remover o registro, clique novamente em **Sim**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw7.png)](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw7.png)

**Nº8–** Faça isso com todas as entradas das quais você guardou os dados.

### **Recriando as entradas** <a href="#recriar" id="recriar"></a>

Agora, vamos **recriar **_**somente**_** as entradas de CNAME** que apagamos (você salvou o nome de todas elas, certo?) com as devidas informações, mas em um novo tipo.

**Observação:** A entrada do domínio principal veremos daqui à pouco.

Vamos lá!

**Nº9–** Clique no botão **Adicionar Entrada** localizado no topo da sua Zona de DNS.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw9.png)](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw9.png)

A entrada deve ser preenchida com as seguintes informações:

**Tipo:** neste campo, verifique se está o tipo **A**.

**Entrada:** aqui, coloque o **nome da entrada** que você salvou (exemplo: **ftp**).

**Conteúdo:** já neste campo, cole o número de IP que você guardou lá no [passo **04**](broken-reference).

**Nº10–** Verifique todos os dados e clique em **Adicionar entradas**.\


[![](https://legado.leadlovers.site/wp-content/uploads/2017/02/lw10.png)](https://legado.leadlovers.site/wp-content/uploads/2017/02/lw10.png)

**Nº11–** Repita os passos **09** e **10** e recrie **todas** as outras entradas da lista que você tinha salvado as informações antes.

### **Apontamento do domínio principal** <a href="#apontamento" id="apontamento"></a>

Agora sim, iremos fazer o apontamento do seu domínio para o nosso servidor. Ele deve ser feito para _2 IPs_.

**Nº12–** Localize novamente a entrada do tipo A (a mesma do [passo 04](broken-reference)) que tem um ponto final ( . ). Clique em Editar.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/02/img09.png)](https://legado.leadlovers.site/wp-content/uploads/2017/02/img09.png)

No pop-up que abrir, confira as informações:

**Entrada:** aqui deve haver um ponto final  ( . ). É isso que irá indicar que a entrada é referente ao domínio principal.

**Tipo:** verifique se o tipo está como A.

**Conteúdo:** apague o IP que estava anteriormente e insira o nosso: 213.136.68.210

**Nº13–** Verifique todos os dados e clique em **Salvar**.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/02/img10.png)](https://legado.leadlovers.site/wp-content/uploads/2017/02/img10.png)

Nº14– Depois que salvar a entrada anterior, crie uma nova no botão Adicionar Entrada que fica em cima da zona DNS.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/02/img11.png)](https://legado.leadlovers.site/wp-content/uploads/2017/02/img11.png)

Nela insira os seguintes dados:

Tipo: selecione o tipo A.

Entrada: aqui você irá preencher com o ponto final  ( . ). É essa informação que irá indicar que a entrada é referente ao domínio principal.

Conteúdo: insira o nosso IP secundário: 213.136.70.54

Nº15– Verifique todos os dados e clique em Adicionar entradas.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/02/img12-3.png)](https://legado.leadlovers.site/wp-content/uploads/2017/02/img12-3.png)

### **Entrada de WWW** <a href="#www" id="www"></a>

É preciso também conferir como está o apontamento da entrada de **www**. Assim, quem incluir estas letras na hora de digitar seu domínio no navegador, será direcionado normalmente para as suas páginas.

Muito provavelmente na seu Locaweb já existirá essa entrada do www.\
Localize a entrada cujo Nome é **www** e confirme se o Conteúdo está com o seu domínio sem o www. No exemplo, está somente wikilovers.com.br

_**Observação:**_ Se no Conteúdo estiver com qualquer outra informação, exclua a entrada e prossiga para criar o registro igual mostramos abaixo no tópico: [**Não tem a entrada**](broken-reference)**.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw14.png)](https://legado.leadlovers.site/wp-content/uploads/2020/12/lw14.png)

#### **Não tem entrada** <a href="#sem-entrada" id="sem-entrada"></a>

**Nº16–** Clique em **Adicionar Entrada** .

As informações da entrada serão:

Tipo: selecione a opção **CNAME**.

Entrada: coloque **www** (não inclua outros caracteres, letras, ou espaços em branco).

Conteúdo: inclua o seu domínio **sem o www**. No exemplo, ficou somente wikilovers.com.br

**Nº17–** Confira todos os dados inclusos e clique em **Adicionar entradas**.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/02/img14.png)](https://legado.leadlovers.site/wp-content/uploads/2017/02/img14.png)

### **Resultado** <a href="#resultado" id="resultado"></a>

Ao final, você deve ter 3 entradas totais: 2 do domínio principal + 1 do www.\
As informações criadas ficarão similares às da imagem abaixo.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/02/img15.png)](https://legado.leadlovers.site/wp-content/uploads/2017/02/img15.png)

Pronto! Agora seu domínio está corretamente apontado para o nosso servidor!

### **Cadastrando o domínio na máquina** <a href="#cadastrando-dominio" id="cadastrando-dominio"></a>

O próximo passo é adicionar este domínio na sua máquina! [**Clique aqui e veja o passo a passo**](https://legado.leadlovers.site/como-cadastrar-dominio-maquina/).

**Artigos sugeridos**

– Se você caiu aleatoriamente aqui e não sabe o que é um domínio e nem como pode usá-lo dentro do nosso sistema, confira primeiro este artigo: [**o que é um domínio**](https://legado.leadlovers.site/o-que-e-um-dominio/).\
– Caso deseje entender melhor como funciona as entradas de uma Zona DNS, **temos esse material aqui \[em breve]**.

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, entre em contato com o nosso suporte!

**É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
