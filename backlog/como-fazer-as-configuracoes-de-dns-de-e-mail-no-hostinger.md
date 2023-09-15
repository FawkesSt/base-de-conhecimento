# Como fazer as configurações de DNS de E-mail no Hostinger?

**Objetivo:** Ensinar como fazer as configurações de DNS de e-mail na Hostinger\
**Para que serve:** A principal função das [**configurações de DNS**](https://suporte.love/dns-de-email/)\
é auxiliar na entregabilidade de suas mensagens, disparadas pela automação de sua conta.

**Requisitos Obrigatórios:**

1\. Possuir uma conta de e-mail feita com um domínio próprio.

2\. Ter acesso à zona DNS do seu domínio. Confira [**aqui**](https://suporte.love/descobrir-cpanel/) como descobrir onde ele está sendo administrado.

Este artigo abrange os seguintes tópicos:

* [Configurando o DNS de E-mail](https://suporte.love/como-fazer-o-dns-de-e-mail-no-google-domains/#configurando-dns)
* [Validando as entradas](https://suporte.love/como-fazer-o-dns-de-e-mail-no-google-domains/#validando-entradas)

### **Configurando o DNS de E-mail**

**1.** Acesse o seu painel da Hostinger e clique no menu **DNS**.

![](https://suporte.love/wp-content/uploads/2020/07/Captura-de-Tela-2023-06-08-as-20.13.15.png)

**2.** Encontre o seu domínio e clique em **Gerenciar**, aqui você deverá criar **5 registros** com os dados que informaremos a seguir

![](https://suporte.love/wp-content/uploads/2020/07/Captura-de-Tela-2023-06-08-as-20.16.43.png)

Para cada um que for criar, clique em **adicionar registro** no canto direito.

Preencha os campos da seguinte forma:

**Registro DKIM**

**Nome do host:** m1.\_domainkey\
**Tipo:** TXT\
**TTL:** 14400\
**Dados:** k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB

\
![](https://suporte.love/wp-content/uploads/2020/07/Captura-de-Tela-2023-06-08-as-20.28.38.png)\


**Registro SPF**

**Nome do host:** mailsg\
**Tipo:** TXT\
**TTL:** 14400\
**Dados:** v=spf1 include:sendgrid.net \~all

![](https://suporte.love/wp-content/uploads/2020/07/Captura-de-Tela-2023-06-08-as-20.29.20.png)

**Registro MX**

**Nome do host:** mailsg\
**Tipo:** MX\
**TTL:** 14400\
**Dados:** mx.sendgrid.net

![](https://suporte.love/wp-content/uploads/2020/07/Captura-de-Tela-2023-06-08-as-20.30.17.png)

**Registro DMARC**

**Nome do host:** \_dmarc\
**Tipo:** TXT\
**TTL:** 14400\
**Dados:** v=DMARC1; p=none; rua=mailto:postmaster@_seudominio.com_\


**Atenção: Substitua a informação **_**seudominio.com**_** pelo domínio próprio que você adquiriu e está configurando.**

![](https://suporte.love/wp-content/uploads/2020/07/Captura-de-Tela-2023-06-08-as-20.31.49.png)

**3.** Para editá-las futuramente, volte e repita o processo.&#x20;

### **Validando as entradas**

Depois que criar todas as entradas, faça a sua [**validação na leadlovers**](https://suporte.love/validando-dns-no-leadlovers/).\
Esse passo é essencial para garantir que os registros funcionem corretamente.

![](https://suporte.love/wp-content/uploads/2022/12/download.png)

### Criando a Entrada Link de Redirect

#### _O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta._ De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect redireciona o lead para o link da página com o seu domínio.&#x20;

O Link redirect é tão importante quanto as demais configurações do DNS de e-mail. Uma configuração completa a outra.&#x20;

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/3-1024x402.png)

Tipo: CNAME\
Nome: Coloque Click \
Objeto: Apontar para, cname.leadlovers.site \
TTL: 14400\
Confira todos os dados e clique em Adicionar registro.![](https://legado.leadlovers.site/wp-content/uploads/2021/01/5-1024x123.png)

A nova entrada ficará salva, junto com as outras que já existem em sua Zona DNS. Ela ficará similar à esta da imagem acima.

OBS: A configuração do redirect é extremamente importante, visto que  Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link.

Depois de todas as entradas realizadas, é necessário validá-las dentro da Leadlovers. Acesse o tutorial a respeito da validação, [clicando aqui.](https://suporte.love/validando-dns-no-leadlovers/)

Suporte

Se você tiver dúvidas na configuração do seu provedor, dê uma olhada se eles possuem um suporte disponível para te auxiliar. E lembre-se: você sempre pode contar conosco ![🥰](https://s.w.org/images/core/emoji/14.0.0/svg/1f970.svg)

![🏁](https://s.w.org/images/core/emoji/14.0.0/svg/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://s.w.org/images/core/emoji/14.0.0/svg/2764.svg)&#x20;
