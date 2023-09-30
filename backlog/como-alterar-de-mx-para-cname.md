# Como alterar de MX para CNAME ?

Algumas hospedagens não permitem a inclusão de mais uma entrada do tipo MX. Somente a do domínio principal.\
Nestes casos, o DNS de E-mail precisa ser feito no tipo CNAME. Utilizamos três das entradas neste outro formato (o DMARC continua sendo em formato TXT).

### **ÍNDICE :**

[**O QUE É DNS DE EMAIL ?**](https://suporte.love/dns-de-e-mail/)

[**COMO FAÇO PARA CONFIGURAR ?**](https://suporte.love/dns-de-e-mail/)

#### **DNS DE EMAIL:**

A principal função delas é auxiliar a entregabilidade de suas mensagens, disparadas pela automação de sua conta.\
A ausência destas entradas pode causar diversos comportamentos indesejados, no momento do envio dos e-mails. Entre eles, os principais são: seus e-mails não chegarem aos destinatários, ou até serem entregues como **SPAM**.

#### **ENTRADAS PADRÃO :**

Recomendamos que o DNS de E-mail seja feito por **TXT e MX** porque são entradas mais eficientes na validação das configurações de segurança pelos Provedores de E-mail.\
Porém, _**alguns Painéis de Controle não aceitam**_ a criação de mais uma **entrada MX.** Visto isso, é preciso fazer as configurações do **DNS de E-mail por CNAME.**\


#### **FORMATO CNAME** <a href="#h_cf11b644-9d90-4d88-ad02-4abf53865d6b" id="h_cf11b644-9d90-4d88-ad02-4abf53865d6b"></a>

Esse artigo mostra passo a passo como configurar as entradas em [_**formato padrão e em formato CNAME.**_](https://suporte.love/dns-de-e-mail/)

#### **COMO ALTERAR DENTRO DO LEADLOVERS PARA CNAME ?**

Dentro da plataforma é necessário modificar qual o tipo de informação o sistema deve validar: de MX e TXT para CNAME.

Segue o passo a passo para realizar essa alteração:

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-60-1.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-60-1.png)

**N 1º –** Acesse configurações \[imagem de uma engrenagem] > **contas de e-mail**

**Escolha/Clique na conta que deseja configurar o DNS de E-mail.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-61-1.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-61-1.png)

**N 2º –** Clique em Configurações de DNS , abrirá essa imagem acima.

**N 3º –** Clique no ícone [![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-62-1.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-62-1.png)

**N 4º –** Desmarque a opção **Utilizar MX >** Depois clique em **Salvar.**

Aguarde uns instantes e após a atualização automática da página, _**ficará assim :**_

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-63-1.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-63-1.png)

**Feito isso, você pode Validar as configurações feitas em CNAME.**\
**Caso ainda não as tenha feito,** [**clique e veja como fazê-las.**](https://suporte.love/validando-dns-no-leadlovers/)

**OBS.:** A configuração da entrada de DMARC segue como TXT.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
