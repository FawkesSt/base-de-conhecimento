# Como fazer as configurações de DNS de E-mail no Hostgator?

**Objetivo:** Ensinar como fazer as configurações de DNS de e-mail na Hostgator\
**Para que serve:** A principal função das [**configurações de DNS**](https://suporte.love/dns-de-email/)\
é auxiliar na entregabilidade de suas mensagens, disparadas pela automação de sua conta.

**Requisitos Obrigatórios:**

1\. Possuir uma conta de e-mail feita com um domínio próprio.

2\. Ter acesso à zona DNS do seu domínio. Confira [**aqui**](https://suporte.love/descobrir-cpanel/) como descobrir onde ele está sendo administrado.

Este artigo abrange os seguintes tópicos:

* [Configurando o DNS de E-mail](https://suporte.love/como-fazer-o-dns-de-e-mail-no-google-domains/#configurando-dns)
* [Validando as entradas](https://suporte.love/como-fazer-o-dns-de-e-mail-no-google-domains/#validando-entradas)

### **Configurando o DNS de E-mail** <a href="#configurando-dns" id="configurando-dns"></a>

**1.** [**Acesse a área do cliente no Hostgator**](https://financeiro.hostgator.com.br/)

**1 –** Informe o endereço de e-mail usado para acesso à sua **Área do Cliente.**

**2 –** Forneça a **senha de acesso**.

**3 –** Marque a opção de segurança. Caso haja algum erro nesta etapa, teste abrir o link de acesso à Área do cliente em outro navegador, ou em uma aba anônima.

**4 –** Clique em **ENTRAR**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_hostgator-login-financeiro-edited.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_hostgator-login-financeiro-edited.png)

### **Acessando o Cpanel de seu Domínio**

**5 –** No quadro de **Lista de Sites**, localize o domínio no qual deseja inserir as configurações de e-mail e Clique em **Cpanel**.

**OBS:** Você será direcionado a uma nova tela do painel de controle do seu domínio.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip0.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip0.png)

**6 –** Encontre e clique na opção **Editor de Zona DNS**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/2020-08-03\_16-56-49.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/2020-08-03\_16-56-49.png)

### **Criando a Entrada MX**

**7 –** não é necessário apagar nenhuma entrada, apenas adicionar novas.

**8 –** Para acessar o seu painel, clique em Gerenciar.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip10.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip10.png)

**9 –** Clique em **Adicionar Registro.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip11.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip11.png)

Use os campos indicados na imagem abaixo e insira os seguintes dados:

**Registro MX**

**Nome do host:** mailsg\
**Tipo:** MX\
**TTL:** 14400\
**Prioridade: 10**\
**Dados:** mx.sendgrid.net

**15 –** Confira todos os dados inseridos, e clique em **Adicionar Registro.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip12.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip12.png)

**Nome do host:** m1.\_domainkey\
**Tipo:** TXT\
**TTL:** 14400\
**Dados:** k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip13.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip13.png)

**Registro SPF**

**Nome do host:** mailsg\
**Tipo:** TXT\
**TTL:** 14400\
**Dados:** v=spf1 include:sendgrid.net \~all

#### &#x20;

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip14.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip14.png)

**Registro DMARC**

**Nome do host:** \_dmarc\
**Tipo:** TXT\
**TTL:** 14400\
**Dados:** v=DMARC1; p=none; rua=mailto:postmaster@_seudominio.com_\


**Atenção: Substitua a informação **_**seudominio.com**_** pelo domínio próprio que você adquiriu e está configurando.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip15.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip15.png)

Ao concluir a adição das quatro entradas, você vai visualizar informações similares à estas na tela de Registros de seu domínio. A ordem como as entradas são exibidas, entretanto, pode variar.

#### **Criando a entrada LINK DE REDIRECT**

\
_Sobre o link de redirect: O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta. De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect (que se trata de um subdomínio criado) redireciona o lead para o link da página com o seu domínio, personalizado. Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link._\


Para criar uma nova entrada é preciso clicar novamente em  [![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip17.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-hostgator\_-360025815813\_mceclip17.png)

**31 –** Em **Nome,**você pode inserir qualquer palavra que desejar. Neste tutorial, escolhemos a palavra click. Portanto nosso link de redirect ficará: click.wikilovers.com.br.

**32 –** Em **TTL**, coloque 14400.

**33 –** Em **Tipo**, selecione **CNAME**.

**34 –** Agora, em **Registro**, coloque **cname.leadlovers.site**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/2-15-1024x61.png)

**35 –** Verifique todos os dados inseridos, e clique em **Adicionar Registro**.

### **Validando as entradas** <a href="#validando-entradas" id="validando-entradas"></a>

Depois que criar todas as entradas, faça a sua [**validação na leadlovers**](https://suporte.love/validando-dns-no-leadlovers/).\
Esse passo é essencial para garantir que os registros funcionem corretamente.

![](https://suporte.love/wp-content/uploads/2022/12/download.png)

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
