# Como criar uma entrada de subdomínio no WebEmpresa?

Olá tudo bem ?\
Neste material, vamos aprender a como criar uma entrada de _**subdomínio**_ no webempresa.

Um mesmo subdomínio/Domínio não pode ser usado em mais de uma máquina ao mesmo tempo, aqui no LeadLovers. Junto a isso, Nestes tipos de caso, aconselhamos criar um novo **subdomínio**.

**Em quais casos eu posso Utilizar um subdominio ?**\
**Situações comuns são:**

* Meu domínio principal está sendo usado em outro site/ferramenta
* Meu domínio principal não permite apontamento por cname
* Meu domínio principal é usado, de alguma forma, em outra ferramenta fora do LeadLovers.

**IMPORTANTE:**

**–** Os passos à seguir devem ser seguidos apenas se a **Zona DNS** de seu domínio for administrada através da sua **conta do WebEmpresa**.

**–** Se ela estiver sob administração em outro serviço, é preciso que sejam feitas no **Painel de Controle específico** deste serviço contratado.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 24 hrs para propagar** e surtir seus efeitos.\
**–** Caso, após este prazo, elas não tenham funcionado como deveria, por favor [**entre em contato com o nosso suporte**](https://help.leadlovers.com/hc/pt-br/articles/360024579873)!

### **Acessando o WebEmpresa**

[Acesse a área do cliente no WebEmpresa](https://www.webempresa.com/areacliente.php), e selecione a sua localização atual.

Se você está no Brasil, selecione a opção “Otro país”

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-24.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-24.png)

Você será redirecionado para a área de login.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-25.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-25.png)

**1 –** Aqui, informe o endereço de e-mail usado para acesso à sua Área do Cliente.

**2 –** Neste campo, forneça a senha de acesso.

**3 –** Clique em **ACCEDER**.

#### **Acessando o CPanel de seu Domínio**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-26.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-26.png)

**4-** No menu de navegação do site, na parte de Hosting clique em Servicios Contratados.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-27.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-27.png)

**5 –** Na próxima tela, em **Servicio**, localize o domínio no qual deseja inserir as configurações do apontamento e clique na **Engrenagem**. ⚙

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-28.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-28.png)

**6-** Na tela de informações sobre o seu domínio role para baixo até localizar a parte de **Información de Alojamiento** então clique para **Acceder a Cpanel**.

**OBS:** Você será direcionado a uma nova tela do painel de controle do seu domínio.

**7 –** Você agora está no Painel de Controle (**CPanel**) do domínio, clique em **Editor de Zona.**

**8 –** Selecione em qual domínio irá criar a entrada **cname referente ao subdominio**.\
**Clique** em **Administrar,** para acessar a área DNS.

### **Criando a Entrada de Subdomínio**

Dentro da próxima tela, você vai ver diversas entradas já criadas. Este é o local onde editamos as informações da **Zona DNS de seu domínio**.

Acima da lista de registros existentes, você tem os campos para criação de novos registros. Vamos usá-los para a criar a entrada de subdomínio.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-29.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-29.png)

**9 –** Em **Nombre**, coloque a palavra que você quer que apareça antes do domínio principal.

**EXEMPLO:** se quero que minha entrada de subdomínio seja **click.leadlovers.com.br**, o nome da entrada que estou criando tem que ser **click**.

**10 –** Em **TTL**, coloque **14400**.

**11 –** Em **Tipo**, selecione a opção **CNAME**

**12 –** Já em **Registro**, coloque: **cname.leadlovers.site**

**13 –** Verifique as informações inseridas e clique em **Agregar registro**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-30.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-30.png)

A nova entrada aparecerá no fim da tela, e ficará similar à esta da imagem acima. Pronto! Ela está criada e corretamente apontada para o nosso servidor!

◽ O próximo passo é adicionar este subdomínio na sua máquina! [**Clique aqui e veja o passo a passo**!](https://suporte.love/como-cadastrar-dominio-maquina/)

**IMPORTANTE:** Pode levar até 24 horas para as configurações sejam totalmente validadas na sua Hospedagem.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
