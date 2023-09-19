# Como criar uma entrada de subdomínio no Locaweb ?

**Objetivo:** Passo a passo de como criar uma entrada de _**subdomínio**_ no locaweb.

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

**–** Os passos à seguir devem ser seguidos apenas se a **Zona DNS** de seu domínio for administrada através da sua **conta do locaweb**.

**–** Se ela estiver sob administração em outro serviço, é preciso que sejam feitas no **Painel de Controle específico** deste serviço contratado.

**–** As alterações realizadas, seguindo estas instruções, podem levar **até 24 hrs para propagar** e surtir seus efeitos.

### **Acessando o Locaweb e o painel de seu domínio**

[**Acesse a área do cliente no Locaweb**](https://www.locaweb.com.br/), e localize o quadro da imagem abaixo.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-89.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-89.png)

**1 –** Clique em Central do Cliente.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-90.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-90.png)

**2 –** Aqui, informe o endereço de e-mail usado para acesso à sua Área do Cliente e sua senha de acesso.

#### **Acessando o Cpanel de seu Domínio**

**3 –** Na próxima tela, no quadro de Serviços, localize o **Hospedagem de sites.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-91.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-91.png)

**4 –** Logo após, ao lado do seu domínio terá um ícone de engrenagem, clique nele **(** [![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-94.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-94.png) **) e e depois clique em zona DNS.**

### **Criando a Entrada de Subdomínio**

Dentro da próxima tela, você vai ver diversas entradas já criadas. Este é o local onde editamos as informações da Zona DNS de seu domínio.

Acima da lista de registros existentes, você tem os campos para criação de novos registros. Vamos usá-los para a criar a entrada de subdomínio.

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever) delas é muito importante.

Se qualquer informação for inserida em formato diferente, ou com espaços em branco antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-92.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-92.png)

**5 –** Logo no inicio da página Clique em **“Adicionar Entrada”.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-93.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/t1-93.png)

**6 –** Em **Tipo**, selecione a opção **CNAME**

**7 –** Em **Entrada**, coloque a palavra que você quer que apareça antes do domínio principal.

**EXEMPLO:** se quero que minha entrada de subdomínio seja **click.leadlovers.com.br**, o nome da entrada que estou criando tem que ser **click**.

**8 –** Já em **conteúdo**, coloque: **cname.leadlovers.site**

**9 –** Verifique as informações inseridas e clique em **Adicionar entradas.**

A nova entrada aparecerá no fim da tela.\
_**Ela está criada e corretamente apontada para o nosso servidor!**_

◽ O próximo passo é adicionar este subdomínio na sua máquina! [**Clique aqui e veja o passo a passo**!](https://suporte.love/como-cadastrar-dominio-maquina/)

**IMPORTANTE:** Pode levar até 24 horas para as configurações sejam totalmente validadas na sua Hospedagem.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
