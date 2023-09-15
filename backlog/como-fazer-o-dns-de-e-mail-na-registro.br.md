# Como fazer o DNS de e-mail na Registro.br

**Objetivo:** Ensinar como fazer as configurações de DNS de e-mail na registro.br\
**Para que serve:** A principal função das [**configurações de DNS**](https://suporte.love/dns-de-email/)\
é auxiliar na entregabilidade de suas mensagens, disparadas pela automação de sua conta.

**Requisitos Obrigatórios:**

1\. Possuir uma conta de e-mail feita com um domínio próprio.

2\. Ter acesso à zona DNS do seu domínio. Confira [**aqui**](https://suporte.love/descobrir-cpanel/) como descobrir onde ele está sendo administrado.

Este artigo abrange os seguintes tópicos:

* [Configurando o DNS de E-mail](https://suporte.love/como-fazer-o-dns-de-e-mail-no-google-domains/#configurando-dns)
* [Validando as entradas](https://suporte.love/como-fazer-o-dns-de-e-mail-no-google-domains/#validando-entradas)

### **Configurando o DNS de E-mail** <a href="#configurando-dns" id="configurando-dns"></a>

**1.** Acesse o seu painel da registro.br e clique no menu **PAINEL.**

![](https://suporte.love/wp-content/uploads/2023/06/Captura-de-Tela-2023-06-08-as-20.39.27.png)

&#x20;

**2.** Encontre o seu domínio e clique **NO DOMÍNIO QUE DESEJA ALTERAR O DNS.**\
\
**3.** Ao entrar, procure pelos campos DNS.

Com isso, vá até a opção Alterar Servidores DNS e **procure por MODO AVANÇADO**

![](https://suporte.love/wp-content/uploads/2023/06/Captura-de-Tela-2023-06-08-as-20.48.03-1.png)

Ele vai pedir uma confirmação, **pode confirmar!**

5\. Clique em **nova entrada** para conseguir executar os próximos passos.

![](https://suporte.love/wp-content/uploads/2023/06/Captura-de-Tela-2023-06-08-as-21.21.36.png)

**5.** aqui você deverá criar **5 registros** com os dados que informaremos a seguir

Para cada um que for criar, clique em **adicionar registro** no canto direito.

Preencha os campos da seguinte forma:

**Registro DKIM**

**Nome do host:** m1.\_domainkey\
**Tipo:** TXT\
**TTL:** 14400\
**Dados:** k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB

![](https://suporte.love/wp-content/uploads/2023/06/Captura-de-Tela-2023-06-08-as-21.22.15.png)

&#x20;

**Registro SPF**

**Nome do host:** mailsg\
**Tipo:** TXT\
**TTL:** 14400\
**Dados:** v=spf1 include:sendgrid.net \~all

![](https://suporte.love/wp-content/uploads/2023/06/Captura-de-Tela-2023-06-08-as-21.23.33.png)

**Registro MX**

**Nome do host:** mailsg\
**Tipo:** MX\
**TTL:** 14400\
**Dados:** mx.sendgrid.net

![](https://suporte.love/wp-content/uploads/2023/06/Captura-de-Tela-2023-06-08-as-21.24.57.png)

**Registro DMARC**

**Nome do host:** \_dmarc\
**Tipo:** TXT\
**TTL:** 14400\
**Dados:** v=DMARC1; p=none; rua=mailto:postmaster@_seudominio.com_\


**Atenção: Substitua a informação **_**seudominio.com**_** pelo domínio próprio que você adquiriu e está configurando.**

![](https://suporte.love/wp-content/uploads/2023/06/Captura-de-Tela-2023-06-08-as-21.25.47.png)

**6.** Para editá-las futuramente, volte e repita o processo.&#x20;

### **Validando as entradas** <a href="#validando-entradas" id="validando-entradas"></a>

Depois que criar todas as entradas, faça a sua [**validação na leadlovers**](https://suporte.love/validando-dns-no-leadlovers/).\
Esse passo é essencial para garantir que os registros funcionem corretamente.

![](https://suporte.love/wp-content/uploads/2022/12/download.png)

&#x20;

### **Criando a Entrada Link de Redirect**

_O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta._

De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect redireciona o lead para o link da página com o seu domínio.

![](https://suporte.love/wp-content/uploads/2023/06/Screenshot\_38-1024x254.png)

&#x20;

**Tipo:**  CNAME\
**Nome :** Click

você pode inserir qualquer palavra que desejar. Neste tutorial, escolhemos a palavra click. Portanto nosso link de redirect ficará:**click.wikilovers.com.br**

**Nome do servidor:** cname.leadlovers.site\
\
**Confira todos os dados inseridos, e clique em Salvar.**

&#x20;

**OBS:** A configuração do redirect é extremamente importante**,** visto que  Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link.

&#x20;

&#x20; **Depois de todas as entradas realizadas, é necessário validá-las dentro da Leadlovers.**\
**Acesse o tutorial a respeito da validação,** [**clicando aqui.**](https://suporte.love/validando-dns-no-leadlovers/)







**Suporte**

Se surgir qualquer dúvida ou se precisar de qualquer ajuda durante este procedimento\
por favor, **entre em contato com o nosso suporte**!

🏁 **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
