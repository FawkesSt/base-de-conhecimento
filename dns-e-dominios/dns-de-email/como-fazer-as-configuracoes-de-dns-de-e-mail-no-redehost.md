# Como fazer as configurações de DNS de E-mail no RedeHost?

**Objetivo:**  Mostrar o passo a passo de como fazer as configurações de DNS(**DKIM**, **SPF**, **DMARC**, **MX e LINK DE REDIRECT**) na RedeHost.\
**Para que serve:** A principal função delas é auxiliar a entregabilidade de suas mensagens, disparadas pela automação de sua conta, [_**saiba mais clicando aqui.**_](./)\
\
**Requisito(s) Obrigatórios:** \
**1.**Possuir uma conta de disparos de domínio próprio \
**2.** Acesso a hospedagem do domínio.

**–** Estas entradas não substituem nenhuma informação ou configuração que já existem na Zona DNS de seu domínio. Caso tenha alguma dúvida no momento de inseri-las, por favor [**entre em contato com o nosso suporte**](https://app.leadlovers.com/atendimento)!\
**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

### **Acessando o RedeHost**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-redehost\_-360046842754\_redehost.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-redehost\_-360046842754\_redehost.png)

**1-** Acesse a página principal do RedeHost. No canto superior direito, localize as informações mostradas na imagem acima, e clique sobre a opção **Painel.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-redehost\_-360046842754\_redehost1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-redehost\_-360046842754\_redehost1.png)

Na próxima tela, localize o quadro indicado na imagem acima.

**2-** informe o seu **usuário de acesso**

**3-** informe sua **senha**.

**4-** clique em **Entrar** para logar.

#### **Acessando o Tela de Registros de sua Zona DNS**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-redehost\_-360046842754\_redehost2.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-redehost\_-360046842754\_redehost2.png)

**5-** No menu à esquerda, clique na informação **Editor de DNS**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-redehost\_-360046842754\_redehost3.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-redehost\_-360046842754\_redehost3.png)

**6-** Role para a tela para baixo até visualizar o botão de **Criar registro de DNS** e então clique nele.

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

#### **Criando a entrada MX**

**Insira os dados da seguinte forma:**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/RH-mx.png)

**7-** Em **Tipo**, escolha **MX**.

**8-** Em **Nome**, insira a palavra **mailsg**

**9-** Em **Dados**, insira **mx.sendgrid.net**

**10-** Agora sim o campo **Prioridade MX** está liberado para edição.\
Deixa a informação do **número 0** (aqui, só pode ser inserido o numeral. Não escreva por extenso).

**11-** Verifique todos os dados inseridos e clique para **Salvar** a entrada.

#### **Criando a entrada DKIM**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/RH-dkim.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-redehost\_-360046842754\_redehost4.png)

**12-** Em **Tipo**, escolha **TXT**.

**13-** Em **Nome**, insira a palavra **m1.\_domainkey**

**14-** Em **Dados**, insira **“k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB”**

**OBS.:** O campo Prioridade MX não estará “liberado” para essa configuração.

**15-** Verifique todos os dados inseridos e clique para **Salvar** a entrada.

#### **Criando a entrada SPF**

_Repita o processo acima novamente, porém com os seguintes dados._

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/RH-spf.png)

**16-** Em **Tipo**, escolha **TXT**.

**17-** Em **Nome**, insira a palavra **mailsg**

**18-** E m **Dados**, insira **“v=spf1 include:sendgrid.net \~all”**

**OBS.:** O campo Prioridade MX não estará “liberado” para essa configuração.

**19-** Verifique todos os dados inseridos e clique para **Salvar** a entrada.

#### **Criando a entrada DMARC**

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/RH-dmarc.png)

**20-** Em **Tipo**, escolha **TXT**.

**21-** Em **Nome**, insira a palavra **\_dmarc**

**22-** E m **Dados**, insira “**v=DMARC1; p=none; rua=mailto:postmaster@seudominio.com.br“**

**MUITA ATENÇÃO:** substitua essa parte “ **seudominio.com.br “** pelo domínio o qual é usado pelo seu e-mail profissional, e no qual você está inserindo estas informações.\
No exemplo deste material, o domínio usado é **leadlovers.com.br**. Por isso, a entrada ficaria: **“v=DMARC1; p=none; rua=mailto:postmaster@leadlovers.com.br”**

**OBS.:** O campo Prioridade MX não estará “liberado” para essa configuração.

**23-** Verifique todos os dados inseridos e clique para **Salvar** a entrada.

#### **Criando a entrada LINK DE REDIRECT**

_Sobre o link de redirect: O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta. De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect (que se trata de um subdomínio criado) redireciona o lead para o link da página com o seu domínio, personalizado. Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link._

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/0-7.png)\


**24-** Em **Tipo**, escolha **CNAME**.

**25-** Em **Nome**, você pode inserir qualquer palavra que desejar. Neste tutorial, escolhemos a palavra click. Portanto nosso link de redirect ficará: click.wikilovers.com.br.

**26-** Em **Dados**, insira **cname.leadlovers.site**

**27-** O campo Prioridade MX não estará “liberado” para essa configuração.

**28-** Verifique todos os dados inseridos e clique para **Salvar** a entrada.



**📢 ✅ Depois de todas as entradas realizadas, é necessário validá-las dentro da Leadlovers.**\
**Acesse o tutorial a respeito da validação,** [**clicando aqui.**](../../backlog/como-fazer-as-configuracoes-de-dns-de-e-mail-no-builderall.md)



&#x20;🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™

