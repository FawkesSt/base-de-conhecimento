# Como fazer as configurações de DNS de E-mail na UolHost ?

**Objetivo:**  Mostrar o passo a passo de como fazer as configurações de DNS(**DKIM**, **SPF**, **DMARC**, **MX e LINK REDIRECT**) na UolHost.\
**Para que serve:** A principal função delas é auxiliar a entregabilidade de suas mensagens, disparadas pela automação de sua conta, [_**saiba mais clicando aqui.**_](./)\
\
**Requisito(s) Obrigatórios:** \
**1.**Possuir uma conta de disparos de domínio próprio \
**2.** Acesso a hospedagem do domínio.\
\
**–** Estas entradas não substituem nenhuma informação ou configuração que já existem na Zona DNS de seu domínio. Caso tenha alguma dúvida no momento de inseri-las, por favor [**entre em contato com o nosso suporte**](https://app.leadlovers.com/atendimento)!\
\
**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

### **Acessando a conta no UolHost**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-uolhost-\_-360042964113\_mceclip0.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-uolhost-\_-360042964113\_mceclip0.png)

**1 –** Acesse a página principal do Uolhost. No canto superior direito, localize as informações mostradas na imagem acima, e clique sobre a opção **Painel do cliente.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-uolhost-\_-360042964113\_mceclip1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-uolhost-\_-360042964113\_mceclip1.png)

Na próxima tela, localize o quadro indicado na imagem acima.

**2 –** informe o seu **e-mail de acesso**

**3 –** informe sua **senha**.

**4 –** Clique em **Entrar** para acessar.

#### **Acessando o Tela de Registros de sua Zona DNS**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-uolhost-\_-360042964113\_mceclip2.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-uolhost-\_-360042964113\_mceclip2.png)

**5 –** Clique no quadro em **“Administrar “** para _Gerenciar Domínios_, localizado na lateral direita ou clique direto em **Domínios**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-uolhost-\_-360042964113\_mceclip3.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-uolhost-\_-360042964113\_mceclip3.png)

_**Na próxima tela, você verá as diversas opções de serviços e configurações acessíveis em sua conta.**_

**6 –** Localize a opção **“Alterar Zona DNS “** para acessar o seu painel de configurações do domínio.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-uolhost-\_-360042964113\_mceclip4.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-na-uolhost-\_-360042964113\_mceclip4.png)

**7 –** Clique no quadro **Gerenciar** , localizado na lateral direita do painel ao lado do seu Domínio.

Logo no inicio da área de registros na parte superior da tela, você terá acesso a todas as entradas criadas na sua área DNS.

**IMPORTANTE:** Escolha o **tipo da entrada que deseja inserir** primeiro. Para essa configuração utilizaremos **(MX, TXT e CNAME).**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/UH-txt-1.png)

**8 –** Clique em **Visualizar** para ter acesso as entradas existentes e **criar as novas entradas.**

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

#### **Criando a entrada MX**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/UH-nova-entrada.png)

Clique em **” Criar nova entrada.”**

**Agora, insira os dados da seguinte forma:**

\
![](https://legado.leadlovers.site/wp-content/uploads/2020/07/UH-mx.png)\


**9 –** Em Entrada, insira a palavra **mailsg**

**10-** Em Destino, insira **mx.sendgrid.net**

**11 – Em Prioridade MX** colocar coloque o **número 0** (aqui, só pode ser inserido o número. Não escreva por extenso).

**12 –** em **Status da entrada,** deixe como **Ativado.**

**13 –** Verifique todos os dados inseridos. clique para **Inserir a entrada** a opção **✔** na coluna em ações.

#### **Criando a entrada DKIM**

Para criar essa entrada é preciso escolher o **TIPO TXT.**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/UH-dkim-1.png)

**14 –** Selecione a **opção TXT** e clique em **Criar nova entrada.**

**15 –** Em **Entrada**, insira a palavra **m1.\_domainkey**

**16 –** Em **Valor**, insira **“k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB”**

**17 –** em **Status** da entrada, deixe como **Ativado**.

**18 –** Verifique todos os dados inseridos. clique para **Inserir a entrada** a opção **✔** na coluna em ações.

#### **Criando a entrada SPF**

_Repita o processo acima novamente, porém com os seguintes dados._

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/UH-spf.png)

**19 –** Em **Entrada**, insira a palavra **mailsg**

**Obs:** o **Tipo** **TXT** já foi escolhido anteriormente.

**20 –** Em **Valor**, insira **“v=spf1 include:sendgrid.net \~all”**

**21 –** em **Status** da entrada, deixe como **Ativado**.

**22 –** Verifique todos os dados inseridos. clique para **Inserir a entrada** a opção **✔** na coluna em ações.

#### **Criando a entrada DMARC**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/UH-dmarc.png)

**23 –** Em **Entrada**, insira a palavra **\_dmarc**

**Obs:** o **Tipo** **TXT** já foi escolhido anteriormente.

**24 –** Em **Valor**, insira “**v=DMARC1; p=none; rua=mailto:postmaster@seudominio.com.br“**

**MUITA ATENÇÃO:** substitua essa parte “ **seudominio.com.br “** pelo domínio o qual é usado pelo seu e-mail profissional, e no qual você está inserindo estas informações.

No exemplo deste material, o domínio usado é **leadlovers.com.br**. Por isso, a entrada fica: **“v=DMARC1; p=none; rua=mailto:postmaster@leadlovers.com.br”**

**25 –** em **Status** da entrada, deixe como **Ativado**.

**26 –** Verifique todos os dados inseridos. clique para **Inserir a entrada** a opção **✔** na coluna em ações.

### **Criando a Entrada Link de Redirect**

\
_Sobre o link de redirect: O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta. De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect (que se trata de um subdomínio criado) redireciona o lead para o link da página com o seu domínio, personalizado. Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link._

Para criar essa entrada é preciso escolher o **CNAME.**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/0-9.png)

**27 –** Selecione a **opção CNAME** e clique em **Criar nova entrada.**

**28 –** Em **Entrada**, você pode inserir qualquer palavra que desejar. Neste tutorial, escolhemos a palavra click. Portanto nosso link de redirect ficará: click.wikilovers.com.br.

**29 –** Em Destino, insira **cname.leadlovers.site**

**30 –** em **Status da entrada,** deixe como **Ativado.**

**31 –** Verifique todos os dados inseridos. clique para **Inserir a entrada** a opção **✔** na coluna em ações.

**📢 ✅ Depois de todas as entradas realizadas, é necessário validá-las dentro da Leadlovers.**\
**Acesse o tutorial a respeito da validação,** [**clicando aqui.**](../../backlog/como-fazer-as-configuracoes-de-dns-de-e-mail-no-builderall.md)



&#x20;🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™
