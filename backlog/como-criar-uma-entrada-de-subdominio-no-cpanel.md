# Como criar uma entrada de subdomínio no cPanel?

**Objetivo:** Passo a passo de como criar uma entrada de _**subdomínio**_ no cPanel

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

**–** Os passos à seguir devem ser seguidos apenas se a **Zona DNS** de seu domínio for administrada através da sua **conta do cPanel**.

**–** Se ela estiver sob administração em outro serviço, é preciso que sejam feitas no **Painel de Controle específico** deste serviço contratado.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 24 hrs para propagar** e surtir seus efeitos.

### **Acessando o cPanel**

Acesse o link de acesso ao cPanel de seu domínio, e localize o quadro da imagem abaixo.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-56.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-56.png)

**1 –** Aqui, informe o seu **nome de usuário**.

**2 –** Já aqui, informe sua **senha**.

**3 –** Clique em **Login** para acessar.

#### **Acessando o Tela de Serviços**

Na próxima tela, você verá as diversas opções de serviços e configurações acessíveis pelo seu Cpanel.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/2020-08-03\_16-56-49.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/2020-08-03\_16-56-49.png)

**4 –** Localize o quadro da categoria Domínios, igual ao da imagem acima. Dentre as opções disponíveis nele, clique sobre a opção **Zone Editor**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-58.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-58.png)

**5 –** Agora, você está na lista de domínios gerenciados por este Cpanel. Procure o qual você deseja usar para seu subdomínio e clique em **Gerenciar** (no exemplo, vamos usar o wikilovers.com.br).

### **Criando a Entrada de Subdomínio**

Dentro da próxima tela, você vai ver diversas entradas já criadas e que direcionam o funcionamento das diversas funções de seu domínio.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-59.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-59.png)

**6 –** Acima da lista de registros existentes, localize e clique sobre o botão **Adicionar registro**.

Logo sobre todas as entradas já existentes, vai aparecer uma nova entrada, só que **vazia** e **marcada em azul**. É nela que faremos os próximos passos.

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/2020-08-03\_17-00-56.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/2020-08-03\_17-00-56.png)

**7 –** Em **Valid zone name ou em NOME**, coloque a palavra que você quer que apareça antes do domínio principal.

**EXEMPLO:** se quero que minha entrada de subdomínio seja **click.wikilovers.com.br**, o nome da entrada que estou criando tem que ser **click**.

**8 –** No segundo campo, deixe o número **14400**.

**9 –** No terceiro campo, selecione a opção **CNAME**

**10 –** Já em **IPv4 address**, coloque: **cname.leadlovers.site**\


**11 –** Verifique as informações inseridas e clique em **Adicionar registro**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/2020-08-03\_17-04-44.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/2020-08-03\_17-04-44.png)

_A nova entrada ficará salva, mudando a cor azul para cinza. Ela ficará similar à esta da imagem acima._

Pronto! Ela está criada e corretamente apontada para o nosso servidor!

◽ O próximo passo é adicionar este subdomínio na sua máquina! [**Clique aqui e veja o passo a passo**!](https://suporte.love/como-cadastrar-dominio-maquina/)

**IMPORTANTE:** Pode levar até 24 horas para as configurações sejam totalmente validadas na sua Hospedagem.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
