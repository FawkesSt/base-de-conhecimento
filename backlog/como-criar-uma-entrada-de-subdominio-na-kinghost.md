# Como criar uma entrada de subdomínio na Kinghost?

**Objetivo:** Passo a passo de como criar uma entrada de _**subdomínio**_ no KingHost.

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

**–** Os passos à seguir devem ser seguidos apenas se a **Zona DNS** de seu domínio for administrada através da sua **conta do KingHost**

**–** Se ela estiver sob administração em outro serviço, é preciso que sejam feitas no **Painel de Controle específico** deste serviço contratado.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 24 hrs para propagar** e surtir seus efeitos.

### **Acessando a conta no KingHost**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-84.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-84.png)

**1 –** Acesse a página principal da **KingHost**. No canto superior direito, localize as informações mostradas na imagem acima, e clique sobre a opção **Painel de Controle**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-83.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-83.png)

Na próxima tela, localize o quadro indicado na imagem acima.

**2 –** informe o seu **e-mail de acesso**

**3 –** informe sua **senha**.

**4 –** Marque a opção **“Não sou um robô”** e Clique em **Acessar Painel** para acessar.

#### **Acessando o Tela de Registros de sua Zona DNS**

Na próxima tela, você verá as diversas opções de serviços e configurações acessíveis em sua conta.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-86.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-86.png)

**5 –** Clique no quadro **Gerenciar Domínios**, localizado na lateral direita do painel.

Após selecionar o seu domínio, você _**será direcionado a uma outra tela.**_

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-85.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-85.png)

**6 –** Localize a opção **“Gerenciar DNS”** para acessar o seu painel de configurações do domínio.

### **Criando a Entrada de Subdomínio**

Dentro da próxima tela, chamada **Registros**, você vai ver diversas entradas já criadas e que direcionam o funcionamento das diversas funções de seu domínio.

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-87.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-87.png)

Logo no inicio da área de registros na parte superior da tela, você verá esse bloco acima.\
nele será incluso as informações do apontamento do seu subdominio.

**7 –** Em **Host**, coloque a palavra que você quer que apareça antes do domínio principal.\
\
**EXEMPLO:** se quero que minha entrada de subdomínio seja **click.leadlovers.com.br**, a palavra que vou colocar tem que ser **click**.

**8 –** Em **Tipo**, escolha a opção **CNAME**.

**9 –** Em **Destino**, insira o número de o nosso servidor: **cname.leadlovers.site**

**12 –** Verifique todos os dados inseridos. clique em Inserir DNS.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-88.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-88.png)

A nova entrada ficará salva, junto com as outras que já existem em sua tela de Registros. Ela ficará similar à esta da imagem acima.

Pronto! Ela está criada e corretamente apontada para o nosso servidor!

◽ O próximo passo é adicionar este subdomínio na sua máquina! [**Clique aqui e veja o passo a passo**!](https://suporte.love/como-cadastrar-dominio-maquina/)

**IMPORTANTE:** Pode levar até 24 horas para as configurações sejam totalmente validadas na sua Hospedagem.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
