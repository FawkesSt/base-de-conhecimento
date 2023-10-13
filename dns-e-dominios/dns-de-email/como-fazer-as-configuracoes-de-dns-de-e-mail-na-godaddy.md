# Como fazer as configurações de DNS de E-mail na GoDaddy?

**Objetivo:** Ensinar como fazer as configurações de DNS de e-mail na godaddy\
**Para que serve:** A principal função das [**configurações de DNS**](./)\
é auxiliar na entregabilidade de suas mensagens, disparadas pela automação de sua conta.

**Requisitos Obrigatórios:**

1\. Possuir uma conta de e-mail feita com um domínio próprio.

2\. Ter acesso à zona DNS do seu domínio. Confira [**aqui**](https://suporte.love/descobrir-cpanel/) como descobrir onde ele está sendo administrado.

Este artigo abrange os seguintes tópicos:

* [Configurando o DNS de E-mail](como-fazer-as-configuracoes-de-dns-de-e-mail-na-godaddy.md#configurando-o-dns-de-e-mail)
* [Validando as entradas](como-fazer-as-configuracoes-de-dns-de-e-mail-na-godaddy.md#validando-as-entradas)

### **Configurando o DNS de E-mail**

**1.** Acesse o seu painel da Godaddy e procure por **Minha Conta, clique em Domínios.**

![](https://suporte.love/wp-content/uploads/2016/06/Captura-de-Tela-2023-06-08-as-21.31.21.png)

**2.** Vá até a barra lateral e procure pela **opção de DNS**\
\
![](https://suporte.love/wp-content/uploads/2016/06/Captura-de-Tela-2023-06-08-as-21.32.56.png)

Procure pelo seu domínio.

![](https://suporte.love/wp-content/uploads/2016/06/Captura-de-Tela-2023-06-08-as-21.35.41.png)

**3.** Ao entrar, procure pelos campos **Adicionar novo registro**

![](https://suporte.love/wp-content/uploads/2016/06/Captura-de-Tela-2023-06-08-as-21.36.24.png)

**4.** aqui você deverá criar **5 registros** com os dados que informaremos a seguir

Para cada um que for criar, clique em **adicionar registro** no canto direito.

Preencha os campos da seguinte forma:

**Registro DKIM**

**Nome do host:** m1.\_domainkey\
**Tipo:** TXT\
**TTL:** 14400 – Padrão\
**Dados:** k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB

![](https://suporte.love/wp-content/uploads/2016/06/Captura-de-Tela-2023-06-08-as-21.37.01.png)

**Registro SPF**

**Nome do host:** mailsg\
**Tipo:** TXT\
**TTL:** 14400 – Padrão\
**Dados:** v=spf1 include:sendgrid.net \~all

![](https://suporte.love/wp-content/uploads/2016/06/Captura-de-Tela-2023-06-08-as-21.37.30.png)

**Registro MX**

**Nome do host:** mailsg\
**Tipo:** MX\
**TTL:** 14400 – Padrão\
**Prioridade: 0**\
**Dados:** mx.sendgrid.net

![](https://suporte.love/wp-content/uploads/2023/06/cxs-1024x272.png)

**Registro DMARC**

**Nome do host:** \_dmarc\
**Tipo:** TXT\
**TTL:** 14400 – Padrão\
**Dados:** v=DMARC1; p=none; rua=mailto:postmaster@_seudominio.com_\


**Atenção: Substitua a informação **_**seudominio.com**_** pelo domínio próprio que você adquiriu e está configurando.**

![](https://suporte.love/wp-content/uploads/2016/06/Captura-de-Tela-2023-06-08-as-21.39.15.png)

**5.** Para editá-las futuramente, volte e repita o processo.

Criando a Entrada Link de Redirect

#### _O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta._ De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect redireciona o lead para o link da página com o seu domínio.&#x20;

O Link redirect é tão importante quanto as demais configurações do DNS de e-mail. Uma configuração completa a outra.&#x20;

Tipo: CNAME\
Nome: Coloque Click\
Valor: cname.leadlovers.site &#x20;

TTL: Padrão \
\
OBS: A configuração do redirect é extremamente importante, visto que  Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link.  &#x20;

Depois de todas as entradas realizadas, é necessário validá-las dentro da Leadlovers.&#x20;

### **Validando as entradas**

Depois que criar todas as entradas, faça a sua [**validação na leadlovers**.](../../backlog/como-fazer-as-configuracoes-de-dns-de-e-mail-no-builderall.md)\
Esse passo é essencial para garantir que os registros funcionem corretamente.

![](https://suporte.love/wp-content/uploads/2022/12/download.png)



**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor **entre em contato com o nosso suporte**!



