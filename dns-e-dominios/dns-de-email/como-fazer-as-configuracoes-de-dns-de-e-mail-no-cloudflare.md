# Como fazer as configurações de DNS de E-mail no CloudFlare?

**Objetivo:** Ensinar como fazer as configurações de DNS de e-mail na Cloudflare\
**Para que serve:** A principal função das [**configurações de DNS**](./) é auxiliar na entregabilidade de suas mensagens, disparadas pela automação de sua conta.

**Requisitos Obrigatórios:**

1\. Possuir uma conta de e-mail feita com um domínio próprio.

2\. Ter acesso à zona DNS do seu domínio. Confira [**aqui**](https://suporte.love/descobrir-cpanel/) como descobrir onde ele está sendo administrado.

Este artigo abrange os seguintes tópicos:

* [Configurando o DNS de E-mail](como-fazer-as-configuracoes-de-dns-de-e-mail-no-cloudflare.md#configurando-dns)
* [Validando as entradas](como-fazer-as-configuracoes-de-dns-de-e-mail-no-cloudflare.md#validando-entradas)

### **Configurando o DNS de E-mail** <a href="#configurando-dns" id="configurando-dns"></a>

**1.** Acesse o seu painel da Cloudflare e clique no seu domínio.

\
<img src="broken-reference" alt="" data-size="original">\


**2.** Encontre no painel lateral a opção de **DNS**

![](https://suporte.love/wp-content/uploads/2016/06/Captura-de-Tela-2023-06-08-as-21.03.43.png)

Para cada um que for criar, clique em **adicionar registro** no canto direito.

Preencha os campos da seguinte forma:

**Registro DKIM**

**Nome do host:** m1.\_domainkey\
**Tipo:** TXT\
**TTL:** Automático\
**Dados:** k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB

\
![](https://suporte.love/wp-content/uploads/2016/06/Captura-de-Tela-2023-06-08-as-21.12.06-1.png)\


**Registro SPF**

**Nome do host:** mailsg\
**Tipo:** TXT\
**TTL: Automático**\
**Dados:** v=spf1 include:sendgrid.net \~all

![](https://suporte.love/wp-content/uploads/2016/06/Captura-de-Tela-2023-06-08-as-21.15.18.png)

**Registro MX**

**Nome:** mailsg\
**Tipo:** MX\
**TTL: Automático**\
Servidor de e-mail: mx.sendgrid.net\
**Prioridade:** 0&#x20;

![](https://suporte.love/wp-content/uploads/2023/06/CapturarDDD.png)

**Registro DMARC**

**Nome do host:** \_dmarc\
**Tipo:** TXT\
**TTL: Automático**\
**Dados:** v=DMARC1; p=none; rua=mailto:postmaster@_seudominio.com_\


**Atenção: Substitua a informação **_**seudominio.com**_** pelo domínio próprio que você adquiriu e está configurando.**

![](https://suporte.love/wp-content/uploads/2016/06/Captura-de-Tela-2023-06-08-as-21.17.50.png)

**3.** Para editá-las futuramente, volte e repita o processo. &#x20;

**OBS:** Na criação das entradas, em **Status do Proxy** adicionar a opção **Somente DNS.**

<figure><img src="https://suporte.love/wp-content/uploads/2023/07/DDDDD.png" alt="" height="109" width="794"><figcaption></figcaption></figure>

### **Validando as entradas** <a href="#validando-entradas" id="validando-entradas"></a>

Depois que criar todas as entradas, faça a sua [**validação na leadlovers**](https://suporte.love/validando-dns-no-leadlovers/).\
Esse passo é essencial para garantir que os registros funcionem corretamente.

![](https://suporte.love/wp-content/uploads/2022/12/download.png)

### **Criando a Entrada Link de Redirect**

_O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta._

De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect redireciona o lead para o link da página com o seu domínio.

![](https://suporte.love/wp-content/uploads/2023/06/Screenshot\_37-1024x163.png)

**Nome :** Click\
Portanto nosso link de redirect ficará:**click.wikilovers.com.br**\
**Em Destino:** cname.leadlovers.site\
**TTL:** Auto

\
**Confira todos os dados inseridos, e clique em Salvar.**

OBS: A configuração do redirect é extremamente importante**,** visto que  Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link.

**Depois de todas as entradas realizadas, é necessário validá-las dentro da Leadlovers. Acesse o tutorial a respeito da validação,** [**clicando aqui.**](../../backlog/como-fazer-as-configuracoes-de-dns-de-e-mail-no-builderall.md)





**Suporte**

Se surgir qualquer dúvida ou se precisar de qualquer ajuda durante este procedimento\
por favor, **entre em contato com o nosso suporte**!

🏁 **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
