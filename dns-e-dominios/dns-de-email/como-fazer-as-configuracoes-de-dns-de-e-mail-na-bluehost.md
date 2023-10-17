# Como fazer as configurações de DNS de E-mail na Bluehost?

**Objetivo:**  Mostrar o passo a passo de como fazer as configurações de DNS(**DKIM**, **SPF**, **DMARC**, **MX e LINK DE REDIRECT**) na Bluehost.\
**Para que serve:** A principal função delas é auxiliar a entregabilidade de suas mensagens, disparadas pela automação de sua conta.

\
**Requisito(s) Obrigatórios:**

&#x20;**1.**Possuir uma conta de disparos de domínio próprio&#x20;

**2.** Acesso a hospedagem do domínio.

\
**–** Estas entradas não substituem nenhuma informação ou configuração que já existem na Zona DNS de seu domínio. Caso tenha alguma dúvida no momento de inseri-las, por favor [**entre em contato com o nosso suporte**](https://app.leadlovers.com/atendimento)!\
**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

### **Acessando a sua conta na BLUEHOST** 

### [![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip0.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip0.png)

**1 –** [**Acesse o site principal da Bluehost**](https://br.bluehost.com/)**.** No canto superior direito, localize as informações mostradas na imagem abaixo, e clique sobre a opção Minha conta.

### [![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip0-1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip0-1.png)

**2 –** Aqui, informe o **usuário** usado para acessar a sua conta da **Bluehost.**

**3 –** Neste campo, forneça a **senha de acesso**.

**4 –** Clique em **Entrar na central**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip1.png)

**5 –** Você será direcionado para sua Central de Cliente. Logo após acessar, procure e clique sobre a opção **“ir para o Domínio”**, digite o **seu Domínio neste local.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip2.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip2.png)

**6 –** A tela de Registro de Domínio será aberta, localize o quadro com o título **“Gerenciar Hospedagem de Sites”.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip3.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip3.png)

**7 – Você será direcionado para sua o Painel de controle do seu domínio.**\
A tela será aberta em uma nova guia de seu navegador. localize o quadro chamado **“Zone Editor”**.

### **Criando as novas entradas**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip4.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip4.png)

**8 –** Na próxima tela aparecerá o campo aonde seus Domínios estarão listados.\
Clique em **Gerenciar.** Você será direcionado para a Administração da **Zona DNS** de seu domínio. Nela, estão as diversas entradas já criadas.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip5.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-bluehost\_-360039407394\_mceclip5.png)

**9 –** Logo no início do quandro de Entradas de DNS, localize o botão **Add Record** e clique sobre ele.\
Uma nova faixa de opções será aberta, logo em seguida.

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia **(modo de escrever) delas é muito importante**.

Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

#### **Criando a entrada MX**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/BH-mx.png)

**10 –** Em **Nome,** insira a palavra **mailsg**

**11 –** Em **Tipo**, coloque: **MX**

**12 –** Em **Prioridade**, coloque o número **0** (aqui, só pode ser inserido o número. Não escreva por extenso)

**13 –** Em **Conteúdo**, coloque: **mx.sendgrid.net**

Confira todos os dados e clique em **Adicionar entradas**

A nova entrada ficará salva, junto com as outras que já existem em Zona DNS.

#### **Criando a entrada DKIM**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/BH-dkim.png)

**Agora, insira os dados da seguinte forma:**

**14 –** Em **Nome,** insira a palavra **m1.\_domainkey**

**15 –** Em **Tipo**, coloque: **TXT**\
\
**16 –** Em **Registro**, coloque:\


**“k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB”**

**17-** Confira todos os dados e clique em **Add Record**

A nova entrada ficará salva, junto com as outras que já existem em Zona DNS.

#### **Criando a entrada SPF**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/BH-spf1.png)

**18 –** Em **Nome,** insira a palavra **mailsg**

**19 –** Em **Tipo**, coloque: **TXT**\
\
**20 –** Em **Registro**, coloque: **“v=spf1 include:sendgrid.net \~all”**

**21 –** Confira todos os dados e clique em **Adicionar entradas**

A nova entrada ficará salva, junto com as outras que já existem em Zona DNS

#### **Criando a entrada DMARC**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/BH-dmarc.png)

**22 –** Em **Nome,** insira a palavra **\_dmarc**

**23 –** Em **Tipo**, coloque: **TXT**\
\
**24 –** Em **Registro**, coloque: “**v=DMARC1; p=none; rua=mailto:\[email protected]”**

**MUITA ATENÇÃO:** substitua a parte **seudominio.com.br** pelo domínio o qual é usado pelo seu e-mail profissional, e no qual você está inserindo estas informações.\
No exemplo deste material, o domínio usado é **leadlovers.com.br**. Por isso, a entrada fica: **“v=DMARC1; p=none; rua=mailto:postmaster@leadlovers.com.br”**

**25 –** Deixe o TTL em 14400

**26 –** Confira todos os dados e clique em **Adicionar entradas**\
A nova entrada ficará salva, junto com as outras que já existem em **Zona DNS.**

#### **Criando a entrada LINK DE REDIRECT**

_Sobre o link de redirect: O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta. De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect (que se trata de um subdomínio criado) redireciona o lead para o link da página com o seu domínio, personalizado. Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link._

**Clique em adicionar nova entrada do tipo CNAME.**\
\
![](https://legado.leadlovers.site/wp-content/uploads/2020/07/0-11-1024x494.png)

27 – Em **Nome/HOST RECORD,** você pode inserir qualquer palavra que desejar. Neste tutorial, escolhemos a palavra click. Portanto nosso link de redirect ficará: click.leadlovers.com.br.

**28 –** Em Points to/Registro/Entrada, coloque: **cname.leadlovers.site**

**29 –** Em **TTL** mantenha 4 horas.

Confira todos os dados e clique em **Adicionar entradas/Save.**

**📢 ✅ Depois de todas as entradas realizadas, é necessário validá-las dentro da Leadlovers.**\
**Acesse o tutorial a respeito da validação,** [**clicando aqui.**](../../backlog/como-fazer-as-configuracoes-de-dns-de-e-mail-no-builderall.md)

\
&#x20;🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™
