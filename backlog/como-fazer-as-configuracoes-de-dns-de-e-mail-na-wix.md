# Como fazer as configurações de DNS de E-mail na Wix?

**Objetivo:** mostrar o passo a passo de como fazer as configurações de DNS de E-mail no **WiX**\
**Para que serve:** a principal função delas é auxiliar a entregabilidade de suas mensagens disparadas pela suas automações aqui na leadlovers.\
**Requisito(s) Obrigatórios: 1.** possuir uma conta de e-mail do domínio próprio em questão e **2.** ter acesso a Zona DNS do seu WiX.\


**📢 IMPORTANTE:**\


**–** Os passos à seguir devem ser feitos **somente se o seu domínio for administrado pelo WiX**.\
Se ele estiver sob administração de outro serviço, é preciso que as configurações sejam realizadas no Painel de Controle específico deste segundo serviço. Nesse [artigo aqui](https://suporte.love/descobrir-cpanel/) nós mostramos como você pode confirmar qual é o painel do seu domínio.

**–** Se feitas corretamente, estas entradas não substituem e nem conflitam com nenhuma informação ou configuração já existente na Zona DNS de seu domínio. Caso tenha alguma dúvida no momento de inseri-las, por favor **entre em contato com o nosso suporte**!&#x20;

### **Acessando a Zona DNS** <a href="#zona-dns" id="zona-dns"></a>

Após acessar seu [**WiX**](https://users.wix.com/signin) você verá uma lista com todos os sites cadastrados por lá.

**Nº1–** Localize o quadrado do domínio no qual deseja fazer as configurações de DNS de E-mail e clique em **Selecionar e Editar Site**.\
Caso tenha apenas um site configurado no WiX, depois de logar no Wix, você já será redirecionado direto para o Painel de Controle do mesmo e, nesse caso, pode ir para o passo 02.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/12/wx1.png)

**Nº2–** No Painel de Controle do site, no canto superior direito, clique sobre seu Perfil e então acesse a opção **Domínios**.

**Nº3–** Você será redirecionado para uma tela com a lista dos seus domínios cadastrados no WiX.\
Mais uma vez, encontre o domínio no qual fará as configurações e clique nos **3 pontinhos**.

**Nº4–** E então em **Gerenciar registros DNS** para acessar a Zona de DNS.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/08/2-3.png)](https://legado.leadlovers.site/wp-content/uploads/2020/08/2-3.png)

![⚠](https://s.w.org/images/core/emoji/13.0.0/svg/26a0.svg) **ATENÇÃO:**

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

– Utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em um formato diferente da orientação e/ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

### **DNS de E-mail**  <a href="#configuracoes" id="configuracoes"></a>

Dentro da próxima tela você verá diversas entradas já criadas e que direcionam o funcionamento das diversas funções de seu domínio. Essas entradas estão organizadas por **Tipos**.

E em alguns Painéis de Controle, como o WiX, não é possível incluir uma entrada do tipo MX para um Nome do Host diferente do Host do domínio principal. Nestes casos, utilizamos três das entradas do tipo CNAME equivalentes as entradas de MX, SPF e DKIM. O DMARC continua sendo em formato TXT e o Link de Redirect em formato CNAME.

#### **Entrada 1** <a href="#cname1" id="cname1"></a>

**Nº5–** Vá na categoria **Registro CNAME (Aliases)** e clique no botão **+ Adicionar registro** que terá no final da mesma.

Os dados da nova entrada devem ser preenchidos com as seguintes informações:

**Nome do Host:** coloque **mailsg**

**Valor:** insira o endereço **u2316725.wl226.sendgrid.net**

**TTL:** este campo virá automaticamente como **1 hora**. Caso tenha alguma informação diferente, altere para 1 hora.

**Nº6–** Verifique todos os dados e clique em **Salvar**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/08/5.png)](https://legado.leadlovers.site/wp-content/uploads/2020/08/5.png)

#### **Entrada 2** <a href="#cname2" id="cname2"></a>

**Nº7–** Ache novamente o botão de **+ Adicionar registro**.

E os dados dessa entrada serão:

**Nome do Host:** informe o nome **s1.\_domainkey**

**Valor:** dessa vez o conteúdo será **s1.domainkey.u2316725.wl226.sendgrid.net**

**TTL:** deve ficar como **1 hora**.

**Nº8–** Salve para criar a nova entrada criada.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/08/7.png)](https://legado.leadlovers.site/wp-content/uploads/2020/08/7.png)

#### **Entrada 3** <a href="#cname3" id="cname3"></a>

**Nº9–** Localize a opção **+ Adicionar registro** mais uma vez.

A entrada precisa ser criada com as seguintes informações:

**Nome do Host:** o nome agora será **s2.\_domainkey**

**Valor:** preencha o campo com o dado **s2.domainkey.u2316725.wl226.sendgrid.net**

**TTL:** confirme se o campo está como **1 hora**.

**Nº10–** Confira os dados inserido e clique em **Salvar**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/08/9.png)](https://legado.leadlovers.site/wp-content/uploads/2020/08/9.png)

#### **Criando a entrada DMARC** <a href="#dmarc" id="dmarc"></a>

Como mencionado antes, a entrada DMARC segue sendo feito pelo tipo TXT.

**Nº11–** Para isso, vá na categoria **TXT (Texto)** e clique no botão **+ Adicionar registro** que terá no final da mesma.

As informação da entrada serão:

**Nome do Host:** coloque **\_dmarc**

**Valor:** insira **v=DMARC1; p=none; rua=mailto:\[email protected]**

**TTL:** verifique se o campo está **1 hora**.

**MUITA ATENÇÃO:** substitua a parte **seudominio.com.br** pelo domínio no qual você está fazendo essas configurações.\
No exemplo das imagens, o domínio usado é **wikilovers.com.br**. Por isso, a entrada ficaria: v=DMARC1; p=none; rua=mailto:postmaster**@wikilovers.com.br**

**Nº12–** Verifique todos os dados e clique em **Salvar**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/08/11.png)](https://legado.leadlovers.site/wp-content/uploads/2020/08/11.png)

#### **Link de Redirect** <a href="#link-de-redirect" id="link-de-redirect"></a>

**Nº13–** Para fazermos a última das configurações de DNS de E-mail, volte na categoria **Registros CNAME (Aliases)** e clique novamente no botão **+ Adicionar registro**.

E a entrada será:

**Nome do Host:** sugerimos colocar o nome como **click**, mas você pode inserir a palavra que desejar. Em nossa sugestão, o Link de Redirect ficará como: click.wikilovers.com.br

**Valor:** insira: **cname.leadlovers.site**

**TTL:** confira se a informação está como **1 hora**.

**Nº14–** Clique em **Salvar.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/08/13.png)](https://legado.leadlovers.site/wp-content/uploads/2020/08/13.png)

### **Resultado** <a href="#resultado" id="resultado"></a>

Ao final, você terá 5 entradas totais: 3 CNAMES + 1 do DKIM + 1 do Link de Redirect.\
As informações inseridas ficarão similares às da imagem abaixo.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/08/re.png)](https://legado.leadlovers.site/wp-content/uploads/2020/08/re.png)

Pronto! Agora as configurações de DNS de E-mail da leadlovers estão configuradas para todas as contas de e-mail do seu domínio em questão!

### **Validando as entradas** <a href="#validacao" id="validacao"></a>

Depois de criar todas as entradas, é necessário validá-las dentro da Leadlovers.\
Acesse o tutorial a respeito da validação, [**clicando aqui**](https://suporte.love/validando-dns-no-leadlovers/).&#x20;

**Artigos sugeridos**

– Se você caiu aleatoriamente aqui e não sabe o que são as configurações de DNS de E-mail e nem como elas podem auxiliar em seus disparos, confira [**este artigo**](https://suporte.love/dns-de-e-mail/).

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, **entre em contato com o nosso suporte**!

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
