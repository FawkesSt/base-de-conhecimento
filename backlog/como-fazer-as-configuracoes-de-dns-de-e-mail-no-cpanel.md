# Como fazer as configurações de DNS de E-mail no Cpanel?

**Objetivo:**  Mostrar o passo a passo de como fazer as configurações de DNS (**DKIM**, **SPF**, **DMARC**, **MX e LINK DE REDIRECT**) no CPANEL.

**Para que serve:** A principal função delas é auxiliar a entregabilidade de suas mensagens, disparadas pela automação de sua conta. [_**saiba mais clicando aqui.**_](https://suporte.love/dns-de-e-mail/)

\
**Requisito(s) Obrigatórios:**

**1.**Possuir uma conta de disparos de domínio próprio;

**2.** Acesso ao painel de controle do domínio.

**–** Estas entradas não substituem nenhuma informação ou configuração que já existem na Zona DNS de seu domínio. Caso tenha alguma dúvida no momento de inseri-las, por favor [**entre em contato com o nosso suporte**](https://app.leadlovers.com/atendimento)!

**– Siga exatamente a ordem das etapas descritas neste material**. A inversão de qualquer etapa pode causar falha na validação dos dados.

### **Acessando o Cpanel**

Acesse o link de acesso ao Cpanel de seu domínio.

**1 –** Informe o seu **nome de usuário**.

**2 –** Informe sua **senha**.

**3 –** Clique em **Login** para acessar.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_subdmaon-cpanel-1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_subdmaon-cpanel-1.png)

### **Criando o subdomínio mailsg**

**4 –** Localize o quadro da categoria **Domínios**, igual ao da imagem abaixo.\
Dentre as opções disponíveis nele, clique sobre a opção **Subdomínios**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-1.png)

Na próxima tela, procure o quadro **Criar um subdomínio**.\
Preencha os campos à seguir com os dados abaixo:

**5 –** No campo **Subdomínio**, escreva a palavra **mailsg**

**6 –** No campo **Domínio**, escolha o domínio principal no qual deseja criar as entradas de DNS de e-mail (neste exemplo, faremos no domínio leadlovers.com.br).

**7 –** O campo **Raiz do documento** vai ser preenchido automaticamente pelo texto **mailsg**. Nenhuma alteração deve ser feita aqui.

**8 –** Confira os dados preenchidos e clique em **Criar**.

### [![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-2.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-2.png)

**9 –** Ainda na mesma tela, vá ao canto direito e localize a opção **Início** (um botão formado de 9 quadrados menores).\
Clique nela e você vai retornar para tela principal do Cpanel.

#### [![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-3.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-3.png)

### **Criando as Entradas DKIM, SPF, DMARC, MX e LINK DE REDIRECT**

**10 –** Localize, novamente, o quadro da categoria **Domínios**. Dentre as opções disponíveis, clique sobre **Zone Editor**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-4.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-4.png)

**11 –** Agora, você está na lista de domínios gerenciados por este Cpanel.\
Procure o qual você deseja usar para seu subdomínio e clique em **Gerenciar** (no exemplo, vamos usar o leadlovers.com.br).

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-5.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-5.png)

**12 –** Acima da lista de registros existentes, localize e clique sobre o botão **Adicionar registro**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-6.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-6.png)

#### **Criando a entrada DKIM**

**13 –** Em **Valid zone name**, insira **m1.\_domainkey** (o nome vai ser autocompletado com o seu domínio principal).

**14 –** Em TTL, mantenha **14400**

**15 –** Em Tipo, insira **TXT**.

**16 –** Em **Text**, coloque **k=rsa; t=s; p=MIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDXvW9fJQkmcbewKoTCB8LkW4kk27dgUVlT3YH2VKfFsS8GDDUZmM5w4CkVk4pZlWdFnu5ekbjqzYekT73289XklSuv94nRaJjkuIEvoGmn1ObskNZNxYBnUdE47o/lgjtbjj0UX7MLQ7WCcEIED2qCmLHXbebpf9NoVMAK7Uy4JQIDAQAB**

**17 –** Verifique todos os dados inseridos, e clique em **Adicionar Registro**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-7.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-7.png)

#### **Criando a entrada SPF**

Clique novamente no botão **Adicionar registro**, que fica acima de todas as entradas de sua Zona DNS (o mesmo botão do passo **12**), para incluirmos uma nova entrada.

**18 –** Em **Valid zone name**, coloque **mailsg** (o nome vai ser autocompletado com o seu domínio principal).

**19 –** No segundo campo, **mantenha o valor 14400**

**20 –** No terceiro campo, selecione a opção **TXT**.

**21 –** Em **Text**, coloque **v=spf1 include:sendgrid.net \~all**

**22 –** Verifique todos os dados inseridos, e clique em **Adicionar Registro**.

#### [![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-8.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-8.png)

#### **Criando a entrada DMARC**

Clique novamente no botão **Adicionar registro.**

**23 –** Em **Valid zone name**, coloque **\_dmarc** (o nome vai ser autocompletado com o seu domínio principal).

**24 –** No segundo campo, **mantenha o valor 14400**

**25 –** No terceiro campo, selecione a opção **TXT**.

**26 –** Em **Text**, coloque **v=DMARC1; p=none; rua=mailto:\[email protected]**

**MUITA ATENÇÃO:** substitua a parte **seudominio.com.br** pelo domínio o qual é usado pelo seu e-mail profissional e no qual você está inserindo estas informações.

No exemplo deste material, o domínio usado é **leadlovers.com.br**. Por isso, a entrada fica: **v=DMARC1; p=none; rua=mailto:postmaster@leadlovers.com.br**

**27 –** Verifique todos os dados inseridos, e clique em **Adicionar Registro**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-9.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-9.png)

#### **Criando a entrada MX**

**28 –** No primeiro campo, estará o domínio principal onde estamos fazendo a configuração. Substitua ele pela palavra **mailsg**&#x20;

**29 –** No segundo campo, não será possível fazer nenhuma edição, então não se preocupe.

**30 –** No terceiro campo, selecione a opção **MX**.

**31 –** No campo à frente de **Prioridade**, coloque o número **0** (aqui, só pode ser inserido o número. Não escreva por extenso).

**32 –** No campo à frente de **Destino**, coloque **mx.sendgrid.net**

**33 –** Verifique todos os dados inseridos, e clique em **Adicionar Registro**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-10.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/como-fazer-as-configuraes-de-dns-de-e-mail-no-cpanel\_-360030629993\_cpanel-dns-email-10.png)

#### **Criando a entrada LINK DE REDIRECT**

\
_Sobre o link de redirect: O link de redirect serve para ser aplicado em todos os links e hiperlinks da sua conta. De modo mais prático, observe que, entre o seu clique no link e o redirecionamento para página, levam milésimos de segundos. Nesse meio período, o link de redirect (que se trata de um subdomínio criado) redireciona o lead para o link da página com o seu domínio, personalizado. Isso aumenta a confiabilidade do seu link aos provedores de e-mails e passa autoridade para quem está clicando do link._

![](https://legado.leadlovers.site/wp-content/uploads/2016/06/1-1024x92.png)

**34 –** No primeiro campo, você pode inserir qualquer palavra que desejar. Neste tutorial, escolhemos a palavra click. Portanto nosso link de redirect ficará: click.leadlovers.com.br

**35 –** No segundo campo, mantenha o **TTL em 14400.**

**36 –** No terceiro campo, selecione a opção **CNAME**.

**37 –** Aqui, insira: **cname.leadlovers.site**

**38 –** Verifique todos os dados inseridos, e clique em **Adicionar Registro**.

**📢 ✅ Depois de todas as entradas realizadas, é necessário validá-las dentro da Leadlovers.**\
**Acesse o tutorial a respeito da validação,** [**clicando aqui.**](https://suporte.love/validando-dns-no-leadlovers/)

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
