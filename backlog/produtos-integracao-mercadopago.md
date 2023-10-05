# Produtos: Integração MercadoPago

**Objetivo**:  Mostrar o passo a passo de uma configuração do leadlovers com o Mercado Pago.\
**Para que serve:** Para quem busca fazer a venda de seu infoproduto ou serviço através da plataforma MercadoPago e entregar o acesso ao produto dentro do EAD da leadlovers e/ou também utilizar das configurações de pós vendas para se relacionar de forma exclusiva com seus clientes.\
**Requisito(s) obrigatório(s): 1.** Este tipo de integração só pode ser feita na conta MercadoPago do produtor; **2.** É necessário já possuir um produto EAD ou Produto Integração criado dentro da leadlovers.

### **Índice**

[**Realizando a integração**](broken-reference)

[**Criando o botão de vendas**](broken-reference)

[**Testando a Integração**](broken-reference)

### **Realizando a integração** <a href="#h_df917a10-4ec9-4cfb-b47b-78e14dedf91d" id="h_df917a10-4ec9-4cfb-b47b-78e14dedf91d"></a>

#### **Fazendo login em conta Mercado Pago**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip0.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip0.png)

**1 –** Primeiro [**acesse o MercadoPago**](https://www.mercadopago.com.br/) e faça login em sua conta.

**Importante:** Dentro do seu produto no leadlovers, você irá pegar as informações que precisam ser inclusas dentro do Mercado pago.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip1.png)\
[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip2.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip2.png)

**2 –** Clicando **na interrogação,** conforme imagem acima, aparecerá um link que irá direcionar ao local exato para inserir os dados necessários para integração, na página **IPN-Notifications.**

#### **URL DE NOTIFICAÇÃO | BOTÃO VENDAS** <a href="#h_813e9de5-d5ab-4d4d-9434-3c90cd1ab4c3" id="h_813e9de5-d5ab-4d4d-9434-3c90cd1ab4c3"></a>

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip4.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip4.png)

**3-** Cole a **URL de notificação** nesse campo.

**4 –** Marque todos os _tópicos acima._

#### **CHAVE DE REFERÊNCIA**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip5.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip5.png)

**5 –** Retorne ao seu produto no leadlovers**,** e Copie a **CHAVE DE REFERÊNCIA.**

**6 –** Clique na _**interrogação azul**_ , clique no link do [_**mercado pago**_](https://www.mercadopago.com.br/tools/create) fornecido no produto no leadlovers.\
ele irá direcionar a página **para criação do botão.**

\
[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip6.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip6.png)\


Preencha as **informações do botão.**\
Titulo | Valor | imagem do produto.

**7 –** Clique em _**MAIS OPÇÕES.**_\
O código de **referência** do produto precisa ser incluso _**dentro do botão de vendas.**_

#### **TOKEN DE ACESSO**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip0-1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip0-1.png)

**8 –** Retorne ao seu produto no leadlovers, em **Access Token** clique na **interrogação azul.**

_**Você será direcionado a essa tela.**_

\
[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_2020-01-30\_10-56-24.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_2020-01-30\_10-56-24.png)\


Nesta tela , você pode perceber que existe duas categorias **“Modo Sandbox e Modo Produção”**\
e cada categoria **possui dois tokens.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_sss.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_sss.png)

**9 –** Iremos utilizar a categoria **“Modo produção”** Copie o **“Access token”** e cole dentro do leadlovers, conforme **informado no passo \[ 8 ].**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip1-1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip1-1.png)

Retorne ao leadlovers novamente, o ultimo passo é incluir o **“e-mail da sua conta Mercado pago”.**

**IMPORTANTE : **_**NUNCA INICIE AS VENDAS SEM ANTES TESTAR A INTEGRAÇÃO, OK?**_

#### **TESTANDO A INTEGRAÇÃO:** <a href="#h_5362cb2b-9054-45dc-9594-0391eaaf8433" id="h_5362cb2b-9054-45dc-9594-0391eaaf8433"></a>

#### Para testar será preciso que você simule uma compra de seu produto, então recomendo que faça o seguinte:

_Dentro do produto no leadlovers, habilite o botão “Liberar acesso na emissão do boleto”._

_Acesse o link de_ vendas do seu produto n_o mercado pago**, simule uma compra por boleto bancário.**_\
_gere esse boleto._\
\
_Depois que simular a compra aguarde alguns minutos e veja em seu produto no leadlovers na Aba Clientes se o e-mail que utilizou na simulação da compra, entrou como cliente no produto._

_**Segue exemplo :**_

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip17.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-mercadopago-360042650133\_mceclip17.png)

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
