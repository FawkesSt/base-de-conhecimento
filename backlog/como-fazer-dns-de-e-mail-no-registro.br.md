# Como fazer DNS de e-mail no Registro.br

**Objetivo:** Ensinar como fazer as configurações de DNS de e-mail no Registro.br.\
**Para que serve:** A principal função das [**configurações de DNS**](https://suporte.love/dns-de-email/)\
é auxiliar na entregabilidade de suas mensagens, disparadas pela automação de sua conta.\
**Requisitos Obrigatórios: 1.** Possuir uma conta de e-mail feita com um domínio próprio. **2.** Ter acesso à zona DNS do seu domínio. Confira [**aqui**](https://suporte.love/descobrir-cpanel/) como descobrir onde ele está sendo administrado.

Este artigo abrange os seguintes tópicos:

* [Configurando o DNS de E-mail](broken-reference)
* [Validando as entradas](broken-reference)

### **Configurando o DNS de E-mail**

**1.** Acesse o seu painel do Registro.br\
e clique no domínio que deseja configurar.

**2.** Role até o menu\
**DNS** e expanda a seção **Configurar zona DNS** (pode\
aparecer também como **Configurar endereçamento**). Caso essa seja\
a primeira vez que ela estiver sendo configurada, ative o\
**Modo Avançado** e prossiga para o passo **3**.

**3.** Você deverá criar **5 registros** com os dados que informaremos a seguir. Para cada um que for criar, clique em **Nova entrada**\
\


Preencha os campos da seguinte forma:

**Registro DKIM**

**Tipo:** TXT\
**Nome:** m1.\_domainkey\
**Dados:** k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB

**Registro SPF**

**Tipo:** TXT\
**Nome:** mailsg\
**Dados:** v=spf1 include:sendgrid.net \~all

**Registro MX**

**Tipo:** MX\
**Nome:** mailsg\
**Prioridade:** 0\
**Nome do servidor de email:** mx.sendgrid.net

**Registro DMARC**

**Tipo:** TXT\
**Nome:** \_dmarc\
**Dados:** v=DMARC1; p=none; rua=mailto:postmaster@_seudominio.com_

**Atenção:** Substitua a informação _seudominio.com_ pelo domínio próprio que você adquiriu e está configurando.

**Link de Redirect**

**Tipo:** CNAME\
**Nome:** insira a palavra que quiser em minúsculo, sem caracteres especiais ou acentos. Sugerimos que utilize _click_\
**Nome do servidor:** cname.leadlovers.site

**4.** Clique em **Salvar alterações**. As entradas criadas devem ficar similares às do print abaixo.&#x20;

### **Validando as entradas**

Depois que criar todas as entradas, faça a sua [**validação na leadlovers**](https://suporte.love/validando-dns-no-leadlovers/). Esse passo é essencial para garantir que os registros funcionem corretamente.

#### **Suporte**

Se você tiver dúvidas na configuração do seu provedor, dê uma olhada se eles possuem um suporte disponível para te auxiliar. E lembre-se: você sempre pode contar conosco🥰

**🏁 É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
