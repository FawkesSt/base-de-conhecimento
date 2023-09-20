# Como criar uma entrada de subdomínio no Cloudflare?

**Objetivo:** Passo a passo de como criar uma entrada de _**subdomínio**_ no Cloudflare.

**Para que serve:** Um mesmo subdomínio/Domínio não pode ser usado em mais de uma máquina ao mesmo tempo, aqui no LeadLovers.\
Junto a isso, nestes tipos de caso, aconselhamos criar um novo **subdomínio**.

**Requisito(s) Obrigatórios:**&#x20;

**1.**Possuir um domínio próprio.\
**2.**Possuir acesso a hospedagem do domínio.

**Em quais casos eu posso Utilizar um subdominio ?**\
**Situações comuns são:**

* Meu domínio principal está sendo usado em outro site/ferramenta
* Meu domínio principal não permite apontamento por cname
* Meu domínio principal é usado, de alguma forma, em outra ferramenta fora do LeadLovers.

**IMPORTANTE:**

**–** Os passos à seguir devem ser seguidos apenas se a **Zona DNS** de seu domínio for administrada através da sua **conta do Cloudflare**.

**–** Se ela estiver sob administração em outro serviço, é preciso que sejam feitas no **Painel de Controle específico** deste serviço contratado.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 24 hrs para propagar** e surtir seus efeitos.

### **Acessando a sua conta no Cloudflare**

[**Acesse o site de login do Cloudflare**](https://dash.cloudflare.com/login), e localize o quadro onde você deve inserir as opções de login e senha.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-23.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-23.png)

**1 –** Informe o **usuário** ou **endereço de e-mail** usado para acessar a sua conta do Cloudflare.

**2 –** Neste campo, forneça a s**enha de acesso**.

**3 –** Clique em **Log in**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/07/cloudflare.png)

**4 –** Na próxima tela,clique sobre o domínio que é usado em seu e-mail profissional.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-63.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-63.png)

**5 –** Depois, localize na parte superior da tela um conjunto de ícones azuis, como este da imagem. Clique sobre a opção **DNS**.

### **Criando a Entrada de Subdomínio**

Dentro da próxima tela, você vai ver diversas entradas já criadas e que direcionam o funcionamento das diversas funções de seu domínio.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-64.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-64.png)

Localize o quadro, mostrado na imagem acima, pois é nele onde vamos inserir os dados para a criação da entrada de Subdomínio.

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-65.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-65.png)

**6 –** Aqui, selecione a opção **CNAME**

**7 –** Em **Name**, coloque a palavra que você quer que apareça antes do domínio principal.

**EXEMPLO:** se quero que minha entrada de subdomínio seja **click.wikilovers.com.br**, o nome da entrada que estou criando tem que ser **click**.

**8 –** Clique em **IPv4 adress/Target**, e coloque: **cname.leadlovers.site**

**9 –** Mantenha esta opção em **Automatic TLL.**

**10 –** Confira todos os dados e clique em **Add Record/Save.**

A nova entrada ficará salva, junto com as outras que já existem em sua Zona DNS. Ela ficará similar à esta da imagem acima.

Pronto! Ela está criada e corretamente apontada para o nosso servidor!

◽ O próximo passo é adicionar este subdomínio na sua máquina! [**Clique aqui e veja o passo a passo**!](https://suporte.love/como-cadastrar-dominio-maquina/)

**IMPORTANTE:** Pode levar até 24 horas para as configurações sejam totalmente validadas na sua Hospedagem.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
