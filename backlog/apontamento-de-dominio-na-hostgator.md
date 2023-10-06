# Apontamento de domínio na Hostgator

**Objetivo:** Mostrar o passo a passo de como utilizar o seu domínio que está na **Hostgator** dentro da leadlovers.\
**Para que serve:** O apontamento permite utilizar o seu domínio como endereço de acesso as páginas e/ou área de membro criadas dentro do sistema.\
**Requisito(s) necessário(s):** **1.** Ter um domínio próprio já comprado e **2.** ter acesso a Zona DNS da Hostgator.

&#x20;**IMPORTANTE:**\


**–** Os passos à seguir devem ser feitos **somente se o seu domínio for administrado pela Hostgator**.\
Se ele estiver sob administração de outro serviço, é preciso que as configurações sejam realizadas no Painel de Controle específico deste segundo serviço. Nesse [artigo aqui](https://suporte.love/descobrir-cpanel/) nós mostramos como você pode confirmar qual é o painel do seu domínio.

**–** Caso seu domínio já seja utilizado para abrir um site feito em outra plataforma, apontá-lo para o nosso IP fará com que ele não abra mais estas páginas. **Seu site externo sairá do ar**.\
Se deseja manter seu domínio principal na forma como está, você pode criar uma entrada do tipo **subdomínio**. [**Clique aqui e veja nosso passo a passo ensinando a criar um subdomínio!**](https://suporte.love/como-criar-uma-entrada-de-subdominio-no-hostgator/)

### **Acessando o cPanel de seu domínio** <a href="#zona-dns" id="zona-dns"></a>

Uma vez logado no [**Portal do cliente na Hostgator**](https://financeiro.hostgator.com.br/) você verá uma lista com todos os seus domínios cadastrados por lá.

**Nº1–** No domínio que deseja usar em sua máquina aqui no leadlovers, clique no botão **cPanel**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/hg1.png)

Você será redirecionado ao Painel de Controle (ou **cPanel**) do domínio. Nele terão várias categorias e cada uma agrupa diversas opções.

**Nº2–** Localize o quadro da categoria Domínios. Dentre as opções disponíveis nele, clique sobre a opção **Editor de zona DNS**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/hg2.png)

**Nº3–** Mais uma vez aparecerá uma lista com seus domínios, no domínio o qual deseja utilizar aqui no leadlovers clique em **Gerenciar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/hg3.png)

### **Salvando as informações necessárias** <a href="#salvar" id="salvar"></a>

Normalmente, a Zona DNS da Hostgator já vem com configurações nela e, por isso, antes de fazer qualquer apontamento precisamos primeiro salvar algumas informações! Ok?

&#x20;**ATENÇÃO:**\


– Essa forma de apontamento é muito sensível e deve ser feita com muita atenção!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

– Utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em um formato diferente da orientação e/ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 2 dias** para propagar e surtir seus efeitos. Caso, após este prazo, elas não tenham funcionado como deveriam, por favor, **entre em contato com o nosso suporte**!

**Nº4–** Entre as entradas que já existem na sua Zona DNS, procure uma do tipo **A**, sem o primeiro nome (haverá apenas o seu domínio principal).\
**Copie o número de IP** para qual ela está apontada e salve essa informação – você pode usar o Bloco de Notas para isso, se quiser.

**Exemplo:** na imagem, a entrada **wikilovers.com.br** é do tipo **A** e não tem primeiro nome.\
Ela está apontada para o número **162.241.2.202**. Então, no caso do exemplo, salvarei este número.

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/hg4.png)

**Nº5–** Localize todas as entradas que sejam do tipo **CNAME** e que esteja apontadas para o seu domínio principal, ou seja, na coluna de Registro conterá somente o seu domínio como valor.\
Salve qual é o primeiro nome dela (_novamente, o Bloco de Notas pode ser seu amigo aqui_).

_**Observação:**_ Para essa configuração, a entrada “www” não será levada em consideração. Ela pode ser mantida como está.

**Exemplo:** a entrada **ftp.wikilovers.com.br**, do tipo **CNAME**, está apontada para **wikilovers.com.br** (o domínio que estamos usando de exemplo).\
Então vou salvar o primeiro nome dela (**ftp**).

![](https://legado.leadlovers.site/wp-content/uploads/2020/11/hg5.png)

Faça isso com **todas** as entradas do tipo **CNAME** que estejam nesse padrão.

_**Observação:**_ Caso não tenha localizado nenhuma entrada que se encaixe nos critérios informados pule essa etapa e vá para o [apontamento do domínio](broken-reference).

### **Excluindo as entradas** <a href="#excluir" id="excluir"></a>

Depois que já salvou as informações, você precisa remover todas essas entradas CNAMEs apontadas para seu domínio.

Nº6– Clique em Excluir.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/01/img06.png)](https://legado.leadlovers.site/wp-content/uploads/2017/01/img06.png)

Nº7– Faça isso com todas as entradas que você guardou os dados.

### Recriando as entradas <a href="#recriar" id="recriar"></a>

Agora, vamos recriar _somente_ as entradas CNAME que apagamos (você salvou o nome de todas elas, certo?) com as devidas informações, mas em um novo tipo.

Observação: A entrada do domínio principal veremos daqui a pouco.

Vamos lá!

Nº8– Clique no botão Adicionar Registro localizado no topo da sua Zona de DNS.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/01/img07-1.png)](https://legado.leadlovers.site/wp-content/uploads/2017/01/img07-1.png)

A entrada deve ser preenchida com as seguintes informações:

Nome: aqui coloque o nome da entrada que você salvou (exemplo: ftp). O restante será automaticamente preenchido com o seu domínio.

TTL: este campo virá automaticamente como 14400. Caso tenha alguma informação diferente, altere para 14400.

Tipo: nesta opção, verifique se está o tipo A.

Conteúdo: já neste espaço, cole o número de IP que você guardou lá no [passo 04](broken-reference).

Nº9– Verifique todos os dados e clique em Adicionar Registro.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/01/img08-1.png)](https://legado.leadlovers.site/wp-content/uploads/2017/01/img08-1.png)

Nº10– Repita os passos 08 e 09 e recrie todas as outras entradas da lista que você tinha salvado as informações antes.

### Apontamento do domínio principal <a href="#apontar" id="apontar"></a>

Agora sim, iremos fazer o apontamento do seu domínio para o nosso servidor. Atualmente, o apontamento para a leadlovers é feito para _2 IPs_.

Nº11– Localize novamente a entrada do tipo A que tem apenas o seu domínio principal no campo Nome (a mesma que você salvou o IP no [passo 04](broken-reference)) e clique em Editar

[![](https://legado.leadlovers.site/wp-content/uploads/2017/01/img09.png)](https://legado.leadlovers.site/wp-content/uploads/2017/01/img09.png)

A entrada deve ser alterada da seguinte forma:

Nome: deixe esse campo como está.

TTL: este espaço virá automaticamente preenchido como 14400. Caso tenha alguma informação diferente, altere para 14400.

Tipo: confira se está como tipo A.

Registro: insira o número do IP primário do nosso servidor, 213.136.68.210

Nº12– Verifique todos os dados e clique em Salvar alteração.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/01/img10.png)](https://legado.leadlovers.site/wp-content/uploads/2017/01/img10.png)

Nº13– Agora lá no início da sua Zona DNS, localize a parte onde está escrito Adicione um registro. Clique nesta opção.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/01/img11.png)](https://legado.leadlovers.site/wp-content/uploads/2017/01/img11.png)

E para inserir o nosso IP secundário (redundância/backup) basta colocar os seguintes dados no novo registro:&#x20;

Nome: insira o seu domínio.

TTL: confirme se o campo está como 14400.&#x20;

Tipo: selecione o tipo A.

Dados: o IP dessa vez será 213.136.70.54

Nº14– Adicione o Registro para criar a nova entrada.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/01/img12.png)](https://legado.leadlovers.site/wp-content/uploads/2017/01/img12.png)

### Entrada de WWW <a href="#www" id="www"></a>

É preciso também fazer o apontamento da entrada de www. Assim, quem incluir estas letras na hora de digitar seu domínio no navegador, será direcionado normalmente para as suas páginas.

Se essa entrada já estiver na sua Zona de DNS você só precisa editá-la, agora, se ela não estiver, será necessário criá-la.

Nº15– Clique em Editar _OU_ Adicione registro.

As informações da entrada serão:

Nome: coloque www (não inclua outros caracteres, letras, ou espaços em branco).

TTL: confirme se o campo está como 14400.

Tipo: já neste campo, selecione a opção CNAME.

Dados: no último campo, inclua o seu domínio sem o www. No exemplo, ficou somente wikilovers.com

Nº16– Confira todos os dados inclusos e clique em Salvar _OU_ Adicionar.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/01/img13.png)](https://legado.leadlovers.site/wp-content/uploads/2017/01/img13.png)

### Resultado <a href="#resultado" id="resultado"></a>

Ao final, você deve ter 3 entradas totais: 2 dos IPs + 1 do www.

As informações criadas ficarão similares às da imagem abaixo.

[![](https://legado.leadlovers.site/wp-content/uploads/2017/01/img14.png)](https://legado.leadlovers.site/wp-content/uploads/2017/01/img14.png)

Pronto! Agora seu domínio está corretamente apontado para o nosso servidor!

### Cadastrando o domínio na máquina <a href="#proximos-passos" id="proximos-passos"></a>

O próximo passo é adicionar este domínio na sua máquina! [**Clique aqui e veja o passo a passo.**](https://suporte.love/como-cadastrar-dominio-maquina/)

**Artigos sugeridos**

– Se você caiu aleatoriamente aqui e não sabe o que é um domínio e nem como pode usá-lo dentro do nosso sistema, confira primeiro este artigo: [**o que é um domínio**](https://suporte.love/o-que-e-um-dominio/).

– Caso deseje entender melhor como funciona as entradas de uma Zona DNS temos esse material aqui \[em breve].

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, entre em contato com o nosso suporte!

🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™
