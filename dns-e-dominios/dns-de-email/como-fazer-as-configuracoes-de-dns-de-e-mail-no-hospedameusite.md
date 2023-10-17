# Como fazer as configurações de DNS de E-mail no HospedameuSite?

**Objetivo:**  Mostrar o passo a passo de como fazer as configurações de DNS(**DKIM**, **SPF**, **DMARC**, **MX e LINK DE REDIRECT**) no Hospedameusite.\
**Para que serve:** A principal função delas é auxiliar a entregabilidade de suas mensagens, disparadas pela automação de sua conta.\
**Requisito(s) Obrigatórios: 1.**Possuir uma conta de disparos de domínio próprio **2.** Acesso a hospedagem do domínio.

**–** Estas entradas não substituem nenhuma informação ou configuração que já existem na Zona DNS de seu domínio. Caso tenha alguma dúvida no momento de inseri-las, por favor [**entre em contato com o nosso suporte**](https://app.leadlovers.com/atendimento)!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

#### **Acessando o Hospeda meu site e o painel de seu domínio:**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip0.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip0.png)

**1 –** Acesse : https://hospedameusite.com.br Clique em **Área do Cliente.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip1.png)

**2 –** Aqui, informe o usuário usado para acessar a sua conta do **Hospeda meu site.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_2019-12-18\_09-11-00.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_2019-12-18\_09-11-00.png)

**3 –** Você será direcionado para sua **Central de Cliente**. Logo após acessar, procure e clique sobre a opção **“Serviços”, clique em Meus serviços.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip0-1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip0-1.png)

**4 –** Em **“Meus produtos/Serviços”** terá a listagem dos seus domínios, clique no botão **“ativo”** ao lado do domínio que deseja configurar.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip3.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip3.png)

**5 –** Conforme a imagem acima clique no botão **“Login no Painel de controle Cpanel”**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip4.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip4.png)

**6 –** A tela de Registro de Domínio será aberta, localize o quadro com o título **“Zone editor”.**

#### **Criando as novas entradas:**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip5.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip5.png)

**7 –** Na próxima tela aparecerá o campo aonde seus **Domínios estarão listados**.\
Clique em **Gerenciar.**

**8 –** Você será direcionado para a Administração da Zona DNS de seu domínio.\
Nela, estão as diversas entradas já criadas.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip5-1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hospedameusite\_-360040571874\_mceclip5-1.png)

**9 –** Logo no início do quandro de Entradas de DNS, localize o botão **Add Record/Adicionar Registro** e clique sobre ele. Uma nova faixa de opções será aberta, logo em seguida.

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia **(modo de escrever) delas é muito importante**.

Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

**Criando a entrada MX**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/HSM-mx.png)

**10 – Em Nome, insira a palavra mailsg**\


**11 –** Em **TTL,** coloque **14400**

**12 –** Em **Tipo**, coloque: **MX**

**13 –** Em **Prioridade**, coloque o número **0** (aqui, só pode ser inserido o número. Não escreva por extenso)

**14 –** Em **Registro**, coloque: **mx.sendgrid.net**

**15 –** Confira todos os dados e clique em **Add Record/Adicionar Registro.**

**Obs:** A nova entrada ficará salva, junto com as outras que já existem em Zona DNS.

**Criando a entrada DKIM**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/HMS-dkim.png)

**Agora, insira os dados da seguinte forma:**

**16 –** Em **Nome,** insira a palavra **m1.\_domainkey**

**17 –** Em **TTL,** coloque 14400

**18 –** Em **Tipo**, coloque: **TXT**\
\
**19 –** Em **Registro**, coloque:\


**“k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB”**

**20 –** Confira todos os dados e clique em **Add Record/Adicionar Registro.**

**Obs:** A nova entrada ficará salva, junto com as outras que já existem em Zona DNS.

**Criando a entrada SPF**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/HSM-spf.png)

**21 –** Em **Nome,** insira a palavra **mailsg**

**22 –** Em **TTL,** coloque 14400

**23 –** Em **Tipo**, coloque: **TXT**

**24 –** Em **Registro**, coloque: **“v=spf1 include:sendgrid.net \~all”**

**25 –** Confira todos os dados e clique em Add Record/Adicionar Registro.

**Criando a entrada DMARC**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/HSM-dmarc.png)

**26 –** Em **Nome,** insira a palavra **\_dmarc**

**27 –** Em **TTL,** coloque 14400

**28 –** Em **Tipo**, coloque: **TXT**

**29 –** Em **Registro**, coloque: “**v=DMARC1; p=none; rua=mailto:\[email protected]”**

**MUITA ATENÇÃO:** substitua a parte **seudominio.com.br** pelo domínio o qual é usado pelo seu e-mail profissional, e no qual você está inserindo estas informações.

No exemplo deste material, o domínio usado é **leadlovers.com.br**. Por isso, a entrada fica: **“v=DMARC1; p=none; rua=mailto:postmaster@leadlovers.com.br”**

**30 –** Confira todos os dados e clique em **Add Record/Adicionar Registro.**

**Criando a entrada LINK DE REDIRECT**

_Sobre o link de redirect: O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta. De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect (que se trata de um subdomínio criado) redireciona o lead para o link da página com o seu domínio, personalizado. Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link._

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-17-1024x178.png)

\
**30 – Em HostName/Nome,** você pode inserir qualquer palavra que desejar. Neste tutorial, escolhemos a palavra click. Portanto nosso link de redirect ficará: click.leadlovers.com.br\


**31 –** Em **TTL,** coloque **14400**

**32 –** Em **Tipo/Type**, coloque: **CNAME**

**33 –** Em **Prioridade/Value/Valor**, coloque **cname.leadlovers.site**

34 – Clique em Save Changes.

📢 ✅ Depois de todas as entradas realizadas, é necessário validá-las dentro da Leadlovers.\
Acesse o tutorial a respeito da validação, [clicando aqui.](../../backlog/como-fazer-as-configuracoes-de-dns-de-e-mail-no-builderall.md)

**É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
