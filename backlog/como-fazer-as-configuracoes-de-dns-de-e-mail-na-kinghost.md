# Como fazer as configurações de DNS de E-mail na KingHost?

**Objetivo:**  Mostrar o passo a passo de como fazer as configurações de DNS(**DKIM**, **SPF**, **DMARC**, **MX e LINK DE REDIRECT**) na KingHost.\
**Para que serve:** A principal função delas é auxiliar a entregabilidade de suas mensagens, disparadas pela automação de sua conta, [_**saiba mais clicando aqui.**_](https://legado.leadlovers.site/o-que-sao-as-configuracoes-de-dns-de-e-mail/)\
**Requisito(s) Obrigatórios: 1.**Possuir uma conta de disparos de domínio próprio **2.** Acesso a hospedagem do domínio.\


**–** Estas entradas não substituem nenhuma informação ou configuração que já existem na Zona DNS de seu domínio.\
Caso tenha alguma dúvida no momento de inseri-las, por favor [**entre em contato com o nosso suporte**](https://app.leadlovers.com/atendimento)!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

### **Acessando a conta no KingHost**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-67.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-67.png)

1 – Acesse a página principal da **KingHost**.\
No canto superior direito, localize as informações mostradas na imagem acima, e clique sobre a opção **Painel de Controle**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-68.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-68.png)

Na próxima tela, localize o quadro indicado na imagem acima.

**2 –** informe o seu **e-mail de acesso**

**3 –** informe sua **senha**.

**4 –** Marque a opção **“Não sou um robô”** e Clique em **Acessar Painel** para acessar.

#### **Acessando o Tela de Registros de sua Zona DNS**

Na próxima tela, você verá as diversas opções de serviços e configurações acessíveis em sua conta.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-69.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-69.png)

5 – Clique no quadro **Gerenciar Domínios**, localizado na lateral direita do painel e selecione o domínio.

Após selecionar o seu domínio, você _**será direcionado a uma outra tela.**_

**6 –** Localize a opção **“Gerenciar DNS”** para acessar o seu painel de configurações do domínio.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-70.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-70.png)

Logo no inicio da área de registros na parte superior da tela, você verá esse bloco acima.\
nele será incluso as informações do DNS.

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

#### &#x20;**Criando a entrada MX**

**7 – Em Tipo, escolha a opção MX**

**8 –** Em **Nome**, insira a palavra **mailsg**

**9 –** Em Destino, insira **mx.sendgrid.net**

**10 –** Em **Prioridade MX** coloque o número **0** (aqui, só pode ser inserido o número. Não escreva por extenso)

**11 –** E em **TTL** deixe **14400**.

**12 –** Verifique todos os dados inseridos. clique em **Adicionar registro.**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/KH-mx.png)

Criando a entrada DKIM

Agora, insira os dados da seguinte forma:

**13 –** Em **Tipo**, escolha a opção **TXT**

**14 –** Em **Nome**, insira a palavra **m1.\_domainkey**

**15 –** Em **valor TXT**, insira **“k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB”**

**16 –** E em **TTL** deixe **14400**.

**17 –** Verifique todos os dados inseridos. clique em **Adicionar registro.**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/KH-dkim.png)

Criando a entrada SPF

_Repita o processo acima novamente, porém com os seguintes dados._

**18 –** Em **Tipo**, escolha a opção **TXT**

**19 –** Em **Host**, insira a palavra **mailsg**

**20 –** Em **Destino**, insira **“v=spf1 include:sendgrid.net \~all”**

**21 –** E em **TTL** deixe **14400**.

**22 –** Verifique todos os dados inseridos. clique em **Inserir DNS.**

#### **Criando a entrada DMARC**

**23 –** Em **Tipo**, escolha a opção **TXT**

**24 –** Em **Host**, insira a palavra **\_dmarc**

**25 –** Em **Destino**, insira “**v=DMARC1; p=none; rua=mailto:postmaster@seudominio.com.br“**

**MUITA ATENÇÃO:** substitua essa parte “ **seudominio.com.br “** pelo domínio o qual é usado pelo seu e-mail profissional, e no qual você está inserindo estas informações.

No exemplo deste material, o domínio usado é **leadlovers.com.br**. Por isso, a entrada fica: **“v=DMARC1; p=none; rua=mailto:postmaster@leadlovers.com.br”**

**26 –** E em **TTL** deixe **14400**.

**27 –** Verifique todos os dados inseridos, clique em **Inserir DNS.**

#### **Criando a entrada LINK de REDIRECT**

_Sobre o link de redirect: O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta. De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect (que se trata de um subdomínio criado) redireciona o lead para o link da página com o seu domínio, personalizado. Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link._

**28 –** Em **Tipo**, escolha a opção **CNAME.**

**29 –** Em **Nome**, você pode inserir qualquer palavra que desejar. Neste tutorial, escolhemos a palavra click. Portanto nosso link de redirect ficará: click.wikilovers.com.br.

**30 –** Em **Objeto**, insira **cname.leadlovers.site**

**31 –** E em **TTL** deixe **14400**.

**32 –** Verifique todos os dados inseridos. clique em **Adicionar registro.**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/KH-link.png)

### **Validando as entradas** <a href="#validando-entradas" id="validando-entradas"></a>

Depois que criar todas as entradas, faça a sua [**validação na leadlovers**](https://suporte.love/validando-dns-no-leadlovers/).\
Esse passo é essencial para garantir que os registros funcionem corretamente.

![](https://suporte.love/wp-content/uploads/2022/12/download.png)

