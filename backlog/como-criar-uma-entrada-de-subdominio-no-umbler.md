# Como criar uma entrada de subdomínio no Umbler?

**Objetivo:** Passo a passo de como criar uma entrada de _**subdomínio**_ no Umbler.

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

**–** Os passos à seguir devem ser seguidos apenas se a **Zona DNS** de seu domínio for administrada através da sua **conta do Umbler**.

**–** Se ela estiver sob administração em outro serviço, é preciso que sejam feitas no **Painel de Controle específico** deste serviço contratado.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 24 hrs para propagar** e surtir seus efeitos.

### **Acessando a conta no UMBLER** 

[**Acesse o site de login do Umbler**](https://app.umbler.com/account/login), e localize o quadro onde você deve inserir as opções de login e senha.

### ![](https://legado.leadlovers.site/wp-content/uploads/2021/01/umbler.png)

**1 –** Informe o **endereço de e-mail** usado para acessar a sua conta do Umbler.

**2 –** Neste campo, forneça a **senha de acesso**.

**3 –** Clique em **Entrar**.

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/umbler1.png)\


**4 –** Na próxima tela, haverá um painel lateral esquerdo com a listagem de seus domínios. Clique no domínio para o qual deseja realizar a configuração de dns de e-mail.

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/umbler2.png)

\
**5 –** Ao clicar sobre o domínio desejado, uma listagem será exibida. Clique na opção **Domínio.**

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/umbler-3.png)

**6 –** Após clicar sobre Domínio, um painel lateral direito será exibido**.** Clique na opção **Editor de DNS.**

**IMPORTANTE :**\
– Nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

– Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

### **Criando a Entrada de Subdomínio**

\
Dentro da próxima tela, você vai ver diversas entradas já criadas e que direcionam o funcionamento das diversas funções de seu domínio.

Agora você fará a criação da entrada do seu subdomínio. Clique no botão ![](https://legado.leadlovers.site/wp-content/uploads/2021/01/2021-01-06\_09-53-35.png) e insira os dados da seguinte forma:

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/dns-umbler1.png)

**7 –** Aqui, selecione a opção **CNAME**

**8 –** Em **Nome**, coloque a palavra que você quer que apareça antes do domínio principal.

**EXEMPLO:** se quero que minha entrada de subdomínio seja **click.wikilovers.com.br**, o nome da entrada que estou criando tem que ser **click**.

**9 –** Clique em **Dados**, e coloque: **cname.leadlovers.site**

**10 –** Mantenha esta opção em **TTL.**

**11 –** Confira todos os dados e clique em **Salvar.**

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/subdominio.png)

A nova entrada ficará salva, junto com as outras que já existem em sua Zona DNS. Ela ficará similar à esta da imagem acima.

Pronto! Ela está criada e corretamente apontada para o nosso servidor!

◽ O próximo passo é adicionar este subdomínio na sua máquina! [**Clique aqui e veja o passo a passo**!](https://suporte.love/como-cadastrar-dominio-maquina/)

**IMPORTANTE:** Pode levar até 24 horas para as configurações sejam totalmente validadas na sua Hospedagem.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
