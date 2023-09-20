# O que é um Subdomínio?

**Objetivo:** aprender o que é um subdomínio e como usá-lo dentro da leadlovers.\
**Para que serve:** o subdomínio é um endereço criado a partir do seu domínio principal, mas independente dele. Pode ser adicionado em uma máquina e utilizado para personalizar a URL das suas páginas aqui na leadlovers.\
**Requisito(s) Obrigatório(s):** **1.** Possuir um domínio próprio; **2.** Possuir acesso ao painel de controle do domínio.

### **O que é um Subdomínio?** <a href="#o-que-e" id="o-que-e"></a>

O subdomínio faz parte do domínio principal, mas funciona de forma independente. Ele nada mais é do que uma informação adicional (palavra) que é inserida antes do domínio principal sem afetar o seu funcionamento, criando um novo endereço e permitindo que seja utilizado para fins diferentes. Ele é composto por um subdomínio e o domínio principal, exemplo:

**cadastro.meunegocio.com.br**

**Subdomínio:** cadastro\
**Domínio principal:** meunegocio.com.br

A principal função deste tipo de entrada é poder ser apontada para um servidor diferente, independentemente para onde o domínio principal aponta. Isso permite, por exemplo, usar o domínio _meunegocio.com.br_ em uma máquina e o subdomínio _cadastro.meunegocio.com.br_ em outra dentro da mesma conta leadlovers e sem precisar adquirir um novo domínio.

_Então, em quais casos eu posso utilizar um subdomínio?_\
Situações comuns são:

* Meu domínio principal está sendo usado em outro site/ferramenta;
* Meu domínio principal já está sendo usado em outra máquina ou produto na leadlovers.

### **Subdomínio de domínio próprio** <a href="#subdominio-dominio-proprio" id="subdominio-dominio-proprio"></a>

Dentro da leadlovers disponibilizamos alguns domínios nossos, que chamamos de “públicos”, para que nossos clientes possam usar adicionando um subdomínio personalizado na frente deles. Por isso, denominamos como subdomínio de “domínio próprio” todo aquele que é criado a partir do domínio do próprio cliente/empresa.

É altamente recomendado que utilize um domínio ou subdomínio de domínio próprio para personalização da sua marca, tanto nos endereços das páginas criadas aqui quanto no e-mail de comunicação com os leads.

#### **Não tenho um domínio próprio, e agora?** <a href="#nao-tenho-dominio" id="nao-tenho-dominio"></a>

Nós orientamos como adquirir um domínio nesse material: [**Clique aqui e confira!**](https://suporte.love/o-que-e-um-dominio/)&#x20;

### **Eu já tenho um domínio! Como posso criar um subdomínio e utilizar na leadlovers?** <a href="#como-criar-subdominio" id="como-criar-subdominio"></a>

É possível utilizar o seu subdomínio dentro da leadlovers para personalizar o link de acesso das páginas que criar por aqui. Para isso, é preciso fazer o que chamamos de _apontamento_.

O **apontamento** é o direcionamento do seu subdomínio para os nossos servidores. Ele é formado por algumas configurações, que são feitas na Zona DNS do seu domínio registrado, na intenção de que ele seja usado nas páginas criadas dentro da leadlovers.

**Observação:** Um mesmo domínio/subdomínio não pode ser usado em mais de uma máquina/produto ao mesmo tempo aqui na leadlovers.

### **Passo a passo das configurações** <a href="#passo-a-passo" id="passo-a-passo"></a>

Temos materiais com instruções específicas para várias hospedagens diferentes, e sempre estamos criando artigos novos. Se você não tem certeza de qual é o Painel de Controle do seu domínio, [confira esse material aqui onde te ensinamos como descobrir isso.](https://suporte.love/descobrir-cpanel/)

#### **Índice** <a href="#tutoriais" id="tutoriais"></a>

Verifique se dentre os links abaixo sua hospedagem já está listada:

[**Registro.BR**](https://suporte.love/como-como-criar-uma-entrada-de-subdominio-no-registro-br/)

[**cPanel**](https://suporte.love/como-como-criar-uma-entrada-de-subdominio-no-cpanel/)

[**Cloudflare**](https://suporte.love/como-criar-uma-entrada-de-subdominio-no-cloudflare/)

[**Hostgator**](https://suporte.love/como-criar-uma-entrada-de-subdominio-no-hostgator/)

[**GoDaddy**](https://suporte.love/como-criar-uma-entrada-de-subdominio-na-godaddy/)

[**Locaweb**](https://suporte.love/como-criar-uma-entrada-de-subdominio-no-locaweb/)

[**Hostinger**](https://suporte.love/como-criar-uma-entrada-de-subdominio-no-hostinger/)

[**KingHost**](https://suporte.love/como-criar-uma-entrada-de-subdominio-na-kinghost/)

[**UolHost**](https://suporte.love/9729-2/)

[**WiX**](https://suporte.love/como-criar-uma-entrada-de-subdominio-no-wix/)

[**Umbler**](https://suporte.love/como-criar-uma-entrada-de-subdominio-no-umbler/)

#### **Realizando o apontamento**  <a href="#realizando-apontamento" id="realizando-apontamento"></a>

&#x20;**ATENÇÃO:**\


**–** Algumas hospedagens oferecem um link ou botão para uma seção chamada **Subdomínios** (ou **Subdomains**). Os passos a seguir **não devem ser feitos neste tipo de seção.** Eles devem ser feitos dentro da **Zona DNS** de seu domínio, seguindo exatamente a ordem descrita abaixo.

**Observação:** Nem todos os painéis de controle de Zona DNS solicitam a informação TLL. Caso o painel de seu domínio solicite, utilize o valor **14400**.

**Nº1–** Acesse o Painel de Controle da Zona DNS de seu domínio principal. É nele que ficam as entradas tipo A, TXT, MX e CNAME (entre outros tipos).

**Nº2–** Crie uma **nova** entrada, seguindo os dados abaixo:

**Tipo da Entrada:** CNAME

**Nome da Entrada:** use a palavra que você quer que apareça antes do domínio principal.

Exemplo: se quero que minha entrada de subdomínio seja _click.wikilovers.com.br_, o nome da entrada que estou criando tem que ser **click**

**Aponte sua entrada CNAME para:** cname.leadlovers.site

Confira todos os dados e salve!

#### **Como criar uma entrada www para o subdomínio?** <a href="#entrada-www" id="entrada-www"></a>

Caso queira que seja possível acessar o seu subdomínio também digitando com www (por exemplo: _www.click.wikilovers.com.br_), é possível adicionar um novo apontamento para isso. Ele não é necessário para o funcionamento do subdomínio e a sua criação é **totalmente opcional**, mas se precisar ou quiser criá-lo basta adicionar uma nova entrada com os seguintes dados:

**Tipo da Entrada:** CNAME

**Nome da Entrada:** insira o www + o subdomínio que você escolheu, com um ponto entre eles.

Exemplo: se criei a entrada de subdomínio com o nome _click_, para fazer a entrada para _www_ preciso inserir no campo nome: **www.click**

**Aponte sua entrada CNAME para:** cname.leadlovers.site

**Observação:** Nem todos os painéis de controle de Zona DNS solicitam a informação TLL. Caso o painel de seu domínio solicite, utilize o valor **14400**.

Confira todos os dados e salve!

### **Próximos passos** <a href="#proximos-passos" id="proximos-passos"></a>

Depois de configurado o apontamento, você precisa adicionar seu subdomínio em sua máquina. Para maiores detalhes, [**clique aqui e veja nosso tutorial, explicando como incluir seu subdomínio em uma máquina!**](https://suporte.love/como-cadastrar-dominio-maquina/)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor **entre em contato com o nosso suporte!**

**Artigos relacionados**\


– [O que é um domínio?](https://suporte.love/o-que-e-um-dominio/)\
– Como [descobrir o Painel de Controle](https://suporte.love/descobrir-cpanel/) do seu domínio?\
– [Validando o apontamento.](https://suporte.love/como-saber-se-meu-apontamento-propagou/)\
– Como [cadastrar um domínio/subdomínio](https://suporte.love/como-cadastrar-dominio-maquina/) em sua máquina?



**🏁 É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
