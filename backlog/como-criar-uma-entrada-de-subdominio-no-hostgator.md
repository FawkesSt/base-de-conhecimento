# Como criar uma entrada de subdomínio no Hostgator?

**Objetivo:** Passo a passo de como criar uma entrada de _**subdomínio**_ no hostgator.

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

**–** Os passos à seguir devem ser seguidos apenas se a **Zona DNS** de seu domínio for administrada através da sua **conta do Hostgator**.

**–** Se ela estiver sob administração em outro serviço, é preciso que sejam feitas no **Painel de Controle específico** deste serviço contratado.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 24 hrs para propagar** e surtir seus efeitos.\


### **Acessando o Hostgator**

[**Acesse a área do cliente no Hostgator**](https://financeiro.hostgator.com.br/), e localize o quadro da imagem abaixo.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-50.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-50.png)

**1 –** Aqui, informe o endereço de e-mail usado para acesso à sua Área do Cliente.

**2 –** Neste campo, forneça a senha de acesso.

**3 –** Marque esta opção de segurança. Caso haja algum erro nesta etapa, teste abrir o link de acesso à Área do cliente em outro navegador, ou em uma aba anônima.

**4 –** Clique em **ENTRAR**.

#### **Acessando o Cpanel de seu Domínio**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-51.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-51.png)

**5 –** Na próxima tela, no quadro de **Lista de Sites**, localize o domínio no qual deseja inserir as configurações de e-mail e Clique em **Cpanel**.

**OBS:** Você será direcionado a uma nova tela do painel de controle do seu domínio.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-52.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-52.png)

**6 –** Você agora está no Painel de Controle (**Cpanel**) do domínio, clique em **Zona Dns.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-53.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-53.png)

**7 –** Selecione em qual domínio irá criar a entrada **cname referente ao subdominio**.\
**Clique** em **Gerenciar,** para acessar a área DNS.

### **Criando a Entrada de Subdomínio**

Dentro da próxima tela, você vai ver diversas entradas já criadas. Este é o local onde editamos as informações da **Zona DNS de seu domínio**.

Acima da lista de registros existentes, você tem os campos para criação de novos registros. Vamos usá-los para a criar a entrada de subdomínio.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-54.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-54.png)

**8 –** Em **Nome**, coloque a palavra que você quer que apareça antes do domínio principal.

**EXEMPLO:** se quero que minha entrada de subdomínio seja **click.leadlovers.com.br**, o nome da entrada que estou criando tem que ser **click**.

**9 –** Em **TTL**, coloque **14400**.

**10 –** Em **Tipo**, selecione a opção **CNAME**

**11 –** Já em **Registro**, coloque: **cname.leadlovers.site**

**12 –** Verifique as informações inseridas e clique em **Adicionar registro**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-55.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-55.png)

A nova entrada aparecerá no fim da tela, e ficará similar à esta da imagem acima. Pronto! Ela está criada e corretamente apontada para o nosso servidor!

◽ O próximo passo é adicionar este subdomínio na sua máquina! [**Clique aqui e veja o passo a passo**!](https://suporte.love/como-cadastrar-dominio-maquina/)

**IMPORTANTE:** Pode levar até 24 horas para as configurações sejam totalmente validadas na sua Hospedagem.



**🏁 É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
