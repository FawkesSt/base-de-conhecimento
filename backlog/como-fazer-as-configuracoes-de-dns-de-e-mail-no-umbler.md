# Como fazer as configurações de DNS de E-mail no Umbler?

**Objetivo:**  Mostrar o passo a passo de como fazer as configurações de DNS (**DKIM**, **SPF**, **DMARC, MX e LINK DE REDIRECT**) no Umbler.

**Para que serve:** A principal função delas é auxiliar a entregabilidade de suas mensagens, disparadas pela automação de sua conta, [_**saiba mais clicando aqui.**_](https://suporte.love/dns-de-e-mail/)\
\
**Requisito(s) Obrigatórios:**\
**1.**Possuir uma conta de disparos de domínio próprio\
**2.** Acesso a hospedagem do domínio.\


**–** Estas entradas não substituem nenhuma informação ou configuração que já existem na Zona DNS de seu domínio. Caso tenha alguma dúvida no momento de inseri-las, por favor [**entre em contato com o nosso suporte**](https://app.leadlovers.com/atendimento)!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

### **Acessando a conta no UMBLER** 

[**Acesse o site de login do Umbler**](https://app.umbler.com/account/login), e localize o quadro onde você deve inserir as opções de login e senha.

### ![](https://legado.leadlovers.site/wp-content/uploads/2021/01/umbler.png)

**1 –** Informe o **endereço de e-mail** usado para acessar a sua conta do Umbler.

**2 –** Neste campo, forneça a **senha de acesso**.

**3 –** Clique em **Entrar**.

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/umbler1.png)\


**4 –** Na próxima tela, haverá um painel lateral esquerdo com a listagem de seus domínios. Clique no domínio para o qual deseja realizar a configuração de dns de e-mail.

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/umbler2.png)

\
**5 –** Ao clicar sobre o domínio desejado, uma listagem será exibida. Clique na opção **Domínio.**\


![](https://legado.leadlovers.site/wp-content/uploads/2021/01/umbler-3.png)

**6 –** Após clicar sobre Domínio, um painel lateral direito será exibido**.** Clique na opção **Editor de DNS.**

**IMPORTANTE :**\
– Nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

### **Criando a Entrada MX** 

Agora, clique no botão  ![](https://legado.leadlovers.site/wp-content/uploads/2021/01/2021-01-06\_09-53-35.png)e insira os dados da seguinte forma:

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/umbler4.png)

**7 –** Em **Tipo**, escolha **MX**

**8 –** Em **Nome**, coloque **mailsg**

**9 –** Em **Dados,** coloque **mx.sendgrid.net**

**10 –** No campo **Prioridade**, coloque o número **0** (zero).

**11 –** Em **TTL**, coloque **1 hora**

**12 –** Confira todos os dados inseridos, e clique em **Salvar.**

### **Criando as Entradas DKIM, SPF, DMARC E LINK DE REDIRECT**

### **Criando a Entrada DKIM**

Para criar uma nova entrada é preciso clicar novamente em  ![](https://legado.leadlovers.site/wp-content/uploads/2021/01/2021-01-06\_09-53-35.png)

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/2021-01-06\_09-56-16.png)

**13 –** Em **Tipo**, escolha **TXT**

**14 –** Em **Nome**, coloque **m1.\_domainkey**

**15 –** Em **Dados,** coloque **k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB**

**16 –** Em **TTL**, coloque **1 hora**

**17 –** Confira todos os dados inseridos, e clique em **Salvar.**

### **Criando a Entrada SPF**

Para criar uma nova entrada é preciso clicar novamente em ![](https://legado.leadlovers.site/wp-content/uploads/2021/01/2021-01-06\_09-53-35.png)

\
\
![](https://legado.leadlovers.site/wp-content/uploads/2021/01/2021-01-06\_10-02-36.png)\


**18 –** Em **Tipo**, escolha **TXT**

**19 –** Em **Nome**, coloque **mailsg**

**20 –** Em **Dados,** coloque **v=spf1 include:sendgrid.net \~all**

**21 –** Em **TTL**, coloque **1 hora**

**22 –** Confira todos os dados inseridos, e clique em **Salvar.**

### **Criando a Entrada DMARC**

Para criar uma nova entrada é preciso clicar novamente em  ![](https://legado.leadlovers.site/wp-content/uploads/2021/01/2021-01-06\_09-53-35.png)

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/2021-01-06\_10-08-16.png)

**23 –** Em **Tipo**, escolha **TXT**

**24 –** Em **Nome**, coloque **\_dmarc**

**25 –** Em **Dados,** coloque **v=DMARC1; p=none; rua=mailto:\[email protected]**

**26 –** Em **TTL**, coloque **1 hora**

**MUITA ATENÇÃO:** substitua a parte **seudominio.com.br** pelo domínio o qual é usado pelo seu e-mail profissional e no qual você está inserindo estas informações.

No exemplo das imagens, o domínio usado é **wikilovers.com.br**. Por isso, a entrada ficaria: v=DMARC1; p=none; rua=mailto:postmaster**@wikilovers.com.br**

**27 –** Confira todos os dados inseridos, e clique em **Salvar.**

### **Criando a Entrada Link de Redirect**

\
_Sobre o link de redirect: O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta. De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect (que se trata de um subdomínio criado) redireciona o lead para o link da página com o seu domínio, personalizado. Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link._

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/1-7.png)

**28 –** Em **Tipo**, escolha **CNAME**\
\
**29 –** Em **Nome**, você pode inserir qualquer palavra que desejar. Neste tutorial, escolhemos a palavra click. Portanto nosso link de redirect ficará: click.wikilovers.com.br.

**30 –** Em **Dados**, insira: **cname.leadlovers.site.**

**31 –** Em **TTL**, mantenha 1 hora.

**32 – Clique** em Salvar**.**\


\
**📢 ✅ Depois de todas as entradas realizadas, é necessário validá-las dentro da Leadlovers.**\
**Acesse o tutorial a respeito da validação,** [**clicando aqui.**](https://suporte.love/validando-dns-no-leadlovers/)

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
