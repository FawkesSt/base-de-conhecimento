# Como fazer as configurações de DNS de E-mail no Builderall?

**Objetivo:** mostrar o passo a passo de como fazer as configurações de DNS de E-mail no **Builderall**\
**Para que serve:** a principal função delas é auxiliar a entregabilidade de suas mensagens disparadas pela suas automações aqui na leadlovers.\
**Requisito(s) Obrigatórios: 1.** possuir uma conta de e-mail do domínio próprio em questão e **2.** ter acesso a Zona DNS do seu Builderall.\


&#x20;**IMPORTANTE:**\


**–** Os passos à seguir devem ser feitos **somente se o seu domínio for administrado pelo Builderall**.\
Se ele estiver sob administração de outro serviço, é preciso que as configurações sejam realizadas no Painel de Controle específico deste segundo serviço. Nesse [artigo aqui](https://legado.leadlovers.site/descobrir-hospedagem/) nós mostramos como você pode confirmar qual é o painel do seu domínio.

**–** Se feitas corretamente, estas entradas não substituem e nem conflitam com nenhuma informação ou configuração já existente na Zona DNS de seu domínio. Caso tenha alguma dúvida no momento de inseri-las, por favor **entre em contato com o nosso suporte**!&#x20;

### **Acessando a Zona DNS** <a href="#zona-dns" id="zona-dns"></a>

Após acessar o seu [**Builderall**](https://office.builderall.com/br/office/login) você  verá a **Home** do seu escritório virtual.

**Nº1–** Localize o aplicativo do **Gerenciador de DNS** e clique em **Entrar**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/12/1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/12/1.png)

**Nº2–** Abrirá uma nova guia e nela terá uma lista com todos os domínios cadastrados por lá.\
Localize o domínio que deseja usar em sua máquina aqui no leadlovers e em **Gerenciar**, clique na opção **Gerenciar DNS**.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/2-4.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/2-4.png)

**Observação:** pode acontecer de aparecer um aviso ao acessar a sua Zona de DNS, nesse caso, basta clicar em **Continuar**.

![⚠](https://s.w.org/images/core/emoji/13.0.0/svg/26a0.svg) **ATENÇÃO:**

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

– Utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em um formato diferente da orientação e/ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

### **DNS de E-mail**  <a href="#configuracoes" id="configuracoes"></a>

Em alguns Painéis de Controle, como o Builderall, não é possível incluir uma entrada do tipo MX para um Host diferente do Host do domínio principal. Nestes casos, utilizamos três das entradas do tipo CNAME equivalentes as entradas de MX, SPF e DKIM. O DMARC continua sendo em formato TXT e o Link de Redirect em formato CNAME.

#### **Entrada 1** <a href="#cname1" id="cname1"></a>

**Nº3–** No canto inferior direito da tela, clique no botão  de **Adicionar**.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/3-4.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/3-4.png)

**Nº4–** Abrirá um pop-up onde você precisa primeiro selecionar o Tipo da nova entrada que deseja criar.\
Selecione o **Tipo CNAME**.

**Nº5–** E clique em **Adicionar** para prosseguir.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/4-5.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/4-5.png)

Os dados da nova entrada devem ser preenchidos com as seguintes informações:

**Tipo:** confirme se está como CNAME.

**Host:** coloque **mailsg**

**Valor:** insira o endereço **u2316725.wl226.sendgrid.net**

**Nº6–** Verifique todos os dados e clique em **Salvar**.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/6-2.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/6-2.png)

#### **Entrada 2** <a href="#cname2" id="cname2"></a>

**Nº7–** Ache novamente o botão de **Adicionar** (o mesmo do [passo **03**](broken-reference)).

**Nº8–** Mais uma vez, escolha o **Tipo CNAME** e clique em **Adicionar.**

E os dados dessa entrada serão:

**Tipo:** verifique se está como CNAME.

**Host:** informe o nome **s1.\_domainkey**

**Valor:** dessa vez o conteúdo será **s1.domainkey.u2316725.wl226.sendgrid.net**

**Nº9–** Verifique todos os dados e clique em **Salvar**.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/9.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/9.png)

#### **Entrada 3** <a href="#cname3" id="cname3"></a>

**Nº10–** Localiza o botão de **Adicionar**.

**Nº11–** O **Tipo** será CNAME novamente e, para prosseguir, clique em **Adicionar**.

A entrada precisa ser criada com as seguintes informações:

**Tipo:** confira se está como CNAME.

**Host:** o nome agora será **s2.\_domainkey**

**Valor:** preencha o campo com o dado **s2.domainkey.u2316725.wl226.sendgrid.net**

**Nº12–** Verifique todos os dados e clique em **Salvar**.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/12.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/12.png)

#### **Criando a entrada DMARC** <a href="#dmarc" id="dmarc"></a>

Como mencionado antes, a entrada DMARC segue sendo feito pelo tipo TXT.

**Nº13–** Para isso, clique em **Adicionar** para criar mais uma nova entrada.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/13.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/13.png)

**Nº14–** Dessa vez, quando o pop-up abrir, opte pelo **Tipo TXT**.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/14-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/14-1.png)

As informação da entrada serão:

**Tipo:** confirme se está como TXT.

**Host:** coloque **\_dmarc**

**Valor:** insira **v=DMARC1; p=none; rua=mailto:\[email protected]**

**MUITA ATENÇÃO:** substitua a parte **seudominio.com.br** pelo domínio no qual você está fazendo essas configurações.\
No exemplo das imagens, o domínio usado é **wikilovers.com.br**. Por isso, a entrada ficaria: v=DMARC1; p=none; rua=mailto:postmaster**@wikilovers.com.br**

**Nº15–** Verifique todos os dados e clique em **Salvar**.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/15-2.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/15-2.png)

#### **Link de Redirect** <a href="#link-de-redirect" id="link-de-redirect"></a>

**Nº16–** E para fazermos a última das configurações de DNS de E-mail, vamos clicar novamente no botão **Adicionar** que está no canto inferior da tela.

**Nº17–** Para o Link de Redirect, o **tipo** também deve ser **CNAME**.

E a entrada será:

**Tipo:** confirme se está corretamente como **CNAME**.

**Host:** sugerimos colocar o nome como **click**, mas você pode inserir a palavra que desejar. Em nossa sugestão, o Link de Redirect ficará como: click.wikilovers.com.br

**Valor:** insira: **cname.leadlovers.site**

**Nº18–** Clique em **Salvar.**

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/18.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/18.png)

### **Resultado** <a href="#resultado" id="resultado"></a>

Ao final, você terá 5 entradas totais: 3 CNAMES + 1 do DKIM + 1 do Link de Redirect.\
As informações inseridas ficarão similares às da imagem abaixo.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/re.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/re.png)

Pronto! Agora as configurações de DNS de E-mail da leadlovers estão configuradas para todas as contas de e-mail do seu domínio em questão!

### **Validando as entradas** <a href="#validacao" id="validacao"></a>

Depois de criar todas as entradas, é necessário validá-las dentro da Leadlovers.\
Acesse o tutorial a respeito da validação, [**clicando aqui**](https://suporte.love/validando-dns-no-leadlovers/).&#x20;

**Artigos sugeridos**

– Se você caiu aleatoriamente aqui e não sabe o que são as configurações de DNS de E-mail e nem como elas podem auxiliar em seus disparos, confira [**este artigo**](https://suporte.love/dns-de-e-mail/).

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, entre em contato com o nosso suporte!

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
