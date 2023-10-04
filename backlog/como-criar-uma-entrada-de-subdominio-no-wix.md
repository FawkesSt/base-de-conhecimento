# Como criar uma entrada de subdomínio no WIX?

**Objetivo:** Passo a passo de como criar uma entrada de _**subdomínio**_ no Wix.

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

**–** Os passos à seguir devem ser seguidos apenas se a **Zona DNS** de seu domínio for administrada através da sua **conta do Wix.**

**–** Se ela estiver sob administração em outro serviço, é preciso que sejam feitas no **Painel de Controle específico** deste serviço contratado.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 24 hrs para propagar** e surtir seus efeitos.

### **Acessando a conta no WIX**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-103.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-103.png)

**1 –** Acesse a página principal da [**Wix**](https://pt.wix.com/).\
No canto superior direito, localize as informações mostradas na imagem acima, e clique em entrar.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-104.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-104.png)

Na próxima tela, localize o quadro indicado na imagem acima.

**2 –** informe o seu **e-mail de acesso**

**3 –** informe sua **senha**.

#### **Acessando o Tela de Registros de sua Zona DNS**

**Após incluir o login e senha, aparecerá a tela principal do WIX.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-105.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-105.png)

**4 – Clique em Gerenciar domínio.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-106.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-106.png)

**5 –** Clique nesse **ícone de três pontos** para acessar a **área DNS.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-107.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-107.png)

**6 –** Clique em Gerenciar **registros DNS**

**IMPORTANTE :**\
– Nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Escolha o **tipo da entrada CNAME**.

### **Criando a Entrada de Subdomínio**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-108.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-108.png)

**N 7º –** Em Registro **CNAME** clique em **Adicionar registro.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-109.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-109.png)

**N 8º –** Nesse campo coloque a palavra que você quer que apareça antes do domínio principal.

**EXEMPLO:** se quero que minha entrada de subdomínio seja **click.leadlovers.com.br**, o nome da entrada que estou criando tem que ser **click**.\


**N 9º –** Já em **Valor**, coloque: **cname.leadlovers.site**

**N 10º –** Verifique as informações inseridas e clique em **Salvar.**

A nova entrada aparecerá no fim da tela, e ficará similar à esta da imagem acima. Ponto! Ela está criada e corretamente apontada para o nosso servidor!

◽ O próximo passo é adicionar este subdomínio na sua máquina! [**Clique aqui e veja o passo a passo**!](https://suporte.love/como-cadastrar-dominio-maquina/)

**IMPORTANTE:** Pode levar até 24 horas para as configurações sejam totalmente validadas na sua Hospedagem.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
