# Como fazer as configurações de DNS de E-mail na Locaweb?

**Objetivo:**  Mostrar o passo a passo de como fazer as configurações de DNS(**DKIM**, **SPF**, **DMARC**, **MX e LINK DE REDIRECT**) na Locaweb.\
**Para que serve:** A principal função delas é auxiliar a entregabilidade de suas mensagens, disparadas pela automação de sua conta, [_**saiba mais clicando aqui**_](o-que-sao-as-configuracoes-de-dns-de-e-mail.md)_**.**_\
**Requisito(s) Obrigatórios:**&#x20;

**1.**Possuir uma conta de disparos de domínio próprio \
**2.** Acesso a hospedagem do domínio.\


**–** Estas entradas não substituem nenhuma informação ou configuração que já existem na Zona DNS de seu domínio. Caso tenha alguma dúvida no momento de inseri-las, por favor [**entre em contato com o nosso suporte**](https://app.leadlovers.com/atendimento)!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

### **Acessando a sua conta na Locaweb**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-2-1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-2-1.png)

1 – [**Acesse o site principal da Locaweb**](https://www.locaweb.com.br/). No canto superior direito, localize as informações mostradas na imagem acima, e clique sobre a opção **Central do Cliente**.

Uma faixa cinza aparecerá, logo abaixo do botão. Localize, do lado direito, o local para inserir os dados de acesso.\
[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-locaweb\_-360034914134\_subdomain-locaweb-2.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-locaweb\_-360034914134\_subdomain-locaweb-2.png)\


**2 –** Aqui, informe o **usuário** usado para acessar a sua conta da Locaweb.

**3 –** Neste campo, forneça a **senha de acesso**.

**4 –** Clique em **Entrar na central**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-locaweb\_-360034914134\_subdomain-locaweb-3.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-locaweb\_-360034914134\_subdomain-locaweb-3.png)

**5 –** Você será direcionado para sua Central de Cliente. Logo após acessar, procure e clique sobre a opção **Registro de domínio.**

\
[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-locaweb\_-360034914134\_subdomain-locaweb-4.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-locaweb\_-360034914134\_subdomain-locaweb-4.png)\


**6 –** A tela de Registro de Domínio será aberta em uma nova guia de seu navegador. Localize o quadro com o título “Selecione o domínio que deseja administrar”, e procure o domínio no qual vamos criar a entrada de subdomínio (no exemplo, vamos usar o leadlovers.com.br). Logo à frente dele, clique sobre a opção **Administrar.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-locaweb\_-360034914134\_subdomain-locaweb-5.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-locaweb\_-360034914134\_subdomain-locaweb-5.png)

**7 –** Na próxima tela, localize o quadro chamado “Zona de DNS”. Nele, procure e clique sobre a opção **Consulte e altere zona de DNS**.

### **Criando as novas entradas**

Uma nova guia será aberta, e você será direcionado para a Administração da Zona DNS de seu domínio. Nela, estão as diversas entradas já criadas.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-locaweb\_-360034914134\_subdomain-locaweb-6.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-locaweb\_-360034914134\_subdomain-locaweb-6.png)

**8 –** Logo no início do quandro de Entradas de DNS, localize o botão **Adicionar Entrada** e clique sobre ele. Uma nova faixa de opções será aberta, logo em seguida.

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

#### **Criando a entrada MX**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/LB-mx.png)

**9 –** Na parte superior da faixa, clique sobre a opção **MX**

**10 –** Em **Entrada**, insira a palavra **mailsg**

**11 –** Em **Prioridade**, coloque o número **0** (aqui, só pode ser inserido o número. Não escreva por extenso)

**12 –** Em **Conteúdo**, coloque: **mx.sendgrid.net**

**13 –** Confira todos os dados e clique em **Adicionar entradas**

A nova entrada ficará salva, junto com as outras que já existem em Zona DNS.

#### **Criando a entrada DKIM**

Agora, insira os dados da seguinte forma:

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/LB-dkim.png)

**14 –** Na parte superior da faixa, clique sobre a opção **TXT**

**15 –** Em **Entrada**, insira a palavra **m1.\_domainkey**

**16 –** Em **Conteúdo**, coloque:\


**“k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB”**

**17 –** Confira todos os dados e clique em **Adicionar entradas**

A nova entrada ficará salva, junto com as outras que já existem em Zona DNS.

#### **Criando a entrada SPF**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/LB-spf.png)

**18 –** Na parte superior da faixa, clique sobre a opção **TXT**

**19 –** Em **Entrada**, insira a palavra **mailsg**

**20 –** Em **Conteúdo**, coloque: **“v=spf1 include:sendgrid.net \~all”**

**21 –** Confira todos os dados e clique em **Adicionar entradas**

A nova entrada ficará salva, junto com as outras que já existem em Zona DNS.

#### **Criando a entrada DMARC**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/LB-dmarc.png)

**22 –** Na parte superior da faixa, clique sobre a opção **TXT**

**23 –** Em **Entrada**, insira a palavra **\_dmarc**

**24 –** Em **Conteúdo**, coloque: “**v=DMARC1; p=none; rua=mailto:\[email protected]”**

**MUITA ATENÇÃO:** substitua a parte **seudominio.com.br** pelo domínio o qual é usado pelo seu e-mail profissional, e no qual você está inserindo estas informações.

No exemplo deste material, o domínio usado é **leadlovers.com.br**. Por isso, a entrada fica: **“v=DMARC1; p=none; rua=mailto:postmaster@leadlovers.com.br”**

**25 –** Confira todos os dados e clique em **Adicionar entradas**

A nova entrada ficará salva, junto com as outras que já existem em Zona DNS.

#### **Criando a entrada LINK DE REDIRECT**

_Sobre o link de redirect: O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta. De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect (que se trata de um subdomínio criado) redireciona o lead para o link da página com o seu domínio, personalizado. Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link._

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-16-1024x245.png)

**26 –** Na parte superior da faixa, clique sobre a opção **CNAME**

**27 –** Em **Entrada**, você pode inserir qualquer palavra que desejar. Neste tutorial, escolhemos a palavra click. Portanto nosso link de redirect ficará: click.wikilovers.com.br.

**28 –** Em **Conteúdo**, coloque: **cname.leadlovers.site**

**29 –** Confira todos os dados e clique em **Adicionar entradas.**

### **Validando as entradas** <a href="#validando-entradas" id="validando-entradas"></a>

Depois que criar todas as entradas, faça a sua[ **validação na leadlovers**](../../backlog/como-fazer-as-configuracoes-de-dns-de-e-mail-no-builderall.md).\
Esse passo é essencial para garantir que os registros funcionem corretamente.

![](https://suporte.love/wp-content/uploads/2022/12/download.png)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor **entre em contato com o nosso suporte**!

