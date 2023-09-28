# Como criar uma entrada de subdomínio no Hostinger?

**Objetivo:** Passo a passo de como criar uma entrada de _**subdomínio**_ no Hostinger.

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

**–** Os passos à seguir devem ser seguidos apenas se a **Zona DNS** de seu domínio for administrada através da sua **conta do Hostinger**.

**–** Se ela estiver sob administração em outro serviço, é preciso que sejam feitas no **Painel de Controle específico** deste serviço contratado.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 24 hrs para propagar** e surtir seus efeitos.

### **Acessando a sua conta no Hostinger** 

[**Acesse o site de login do Hostinger**](https://www.hostinger.com.br/cpanel-login), e localize o quadro onde você deve inserir as opções de login e senha.

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/hostinger-login-300x294.png)\


**1 –** Informe o **usuário** ou **endereço de e-mail** usado para acessar a sua conta do Hostinger.

**2 –** Neste campo, forneça a **senha de acesso**.

**3 –** Clique em **Entrar**.

No menu superior, clique em HOSPEDAGEM

![](https://suporte.love/wp-content/uploads/2021/01/hospedagem-300x109.png)

Quando já estiver na tela de Hospedagens, clique em GERENCIAR

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/1-1024x167.png)

**4 –** Na próxima tela, clique no botão gerenciar do domínio para o qual deseja criar o subdomínio.

Você será redirecionado ao Painel de Controle (ou **Cpanel**) do domínio. Nele terão várias categorias e cada uma agrupa diversas opções.

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/2.png)

**5 –**  Localize o quadro da categoria Avançado. Dentre as opções disponíveis nele, clique sobre a opção **Editor de Zona DNS.**

### **Criando a Entrada de Subdomínio**

Dentro da próxima tela, você vai ver diversas entradas já criadas e que direcionam o funcionamento das diversas funções de seu domínio.

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/3-1024x402.png)

Localize o quadro, mostrado na imagem acima, pois é nele onde vamos inserir os dados para a criação da entrada de Subdomínio.

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/4-1-1024x436.png)

**6 –** Aqui, selecione a opção **CNAME** no tipo da entrada.

**7 –** Em **Nome**, coloque a palavra que você quer que apareça antes do domínio principal.

**EXEMPLO:** se quero que minha entrada de subdomínio seja **click.wikilovers.com.br**, o nome da entrada que estou criando tem que ser **click**

**8 –** Clique em **Objeto**, e coloque: **cname.leadlovers.site**

**9 –** Mantenha esta opção padrão (14400) em **TTL.**

**10 –** Confira todos os dados e clique em **Adicionar registro.**

![](https://legado.leadlovers.site/wp-content/uploads/2021/01/5-1024x123.png)

A nova entrada ficará salva, junto com as outras que já existem em sua Zona DNS. Ela ficará similar à esta da imagem acima.

Pronto! Ela está criada e corretamente apontada para o nosso servidor!

◽ O próximo passo é adicionar este subdomínio na sua máquina! [**Clique aqui e veja o passo a passo**!](https://suporte.love/como-cadastrar-dominio-maquina/)

**IMPORTANTE:** Pode levar até 24 horas para as configurações sejam totalmente validadas na sua Hospedagem.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
