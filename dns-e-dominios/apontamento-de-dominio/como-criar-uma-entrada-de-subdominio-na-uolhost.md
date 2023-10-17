# Como criar uma entrada de subdomínio na Uolhost?

**Objetivo:** Passo a passo de como criar uma entrada de _**subdomínio**_ no\
uolhost.\
**Para que serve:** Um mesmo subdomínio/Domínio não pode ser usado\
em mais de uma máquina ao mesmo tempo, aqui no LeadLovers. Junto a isso, nestes\
tipos de caso, aconselhamos criar um novo **subdomínio**.\
**Requisito(s) Obrigatórios: 1.** Possuir\
um domínio próprio. **2.** Possuir acesso a hospedagem do domínio.

Este artigo abrange os seguintes tópicos:

* [Em quais casos eu posso utilizar um subdomínio?](broken-reference)
* [Acessando a conta no UolHost](broken-reference)
* [Acessando a Tela de Registros de sua Zona DNS](broken-reference)
* [Criando a Entrada de Subdomínio](broken-reference)

**IMPORTANTE:**\
**–** Os passos a seguir devem\
ser seguidos apenas se a **Zona DNS** de seu domínio for\
administrada através da sua **conta do UolHost**.\
**–** Se ela estiver sob administração em outro serviço, é\
preciso que sejam feitas no **Painel de Controle específico** deste\
serviço contratado.\
**–** As alterações realizadas, seguindo estas instruções,\
podem levar **até 24 hrs para propagar** e surtir seus\
efeitos.

### **Em quais casos eu posso utilizar um subdomínio?** <a href="#h_01fxb304yypg0515g8d58rd2f4" id="h_01fxb304yypg0515g8d58rd2f4"></a>

**Situações comuns são:**

* Meu domínio principal está sendo usado em outro site/ferramenta
* Meu domínio principal não permite apontamento por cname
* Meu domínio principal é usado, de alguma forma, em outra ferramenta fora\
  do LeadLovers.

### **Acessando a conta no UolHost** <a href="#h_01fxb309snkjkcjn0n00zga23j" id="h_01fxb309snkjkcjn0n00zga23j"></a>

![](https://suporte.love/wp-content/uploads/2022/12/IMG1-1-300x36.png)

**N 1º –** Acesse a página **principal do Uolhost**.\
No canto superior direito, localize as informações mostradas na imagem acima,\
e clique sobre a opção Painel do cliente.

![](https://suporte.love/wp-content/uploads/2022/12/IMG2-1-219x300.png)

Na próxima tela, localize o quadro indicado na imagem acima.

**N 2º –** informe o seu **e-mail de acesso**

**N 3º –** informe sua **senha**.

**N 4º –** Clique em **Entrar** para\
acessar.

### **Acessando a Tela de Registros de sua Zona DNS** <a href="#h_01fxb30e22m6xhq1gnx5z3wrdw" id="h_01fxb30e22m6xhq1gnx5z3wrdw"></a>

![](https://suporte.love/wp-content/uploads/2022/12/IMG3-1-300x97.png)

**N 5º –** Clique no quadro em **“Administrar “** para _Gerenciar Domínios_,\
localizado na lateral direita **ou** clique **direto em Domínios.**

![](https://suporte.love/wp-content/uploads/2022/12/IMG4-1-300x107.png)

_**Na próxima tela, você verá as diversas opções de serviços e configurações acessíveis em sua conta.**_

**N 6º –** Localize a opção **“Alterar Zona DNS “** para\
acessar o seu painel de configurações do domínio.

![](https://suporte.love/wp-content/uploads/2022/12/IMG5-300x106.png)

**N 7º –** Clique no quadro **Gerenciar** ,\
localizado na lateral direita do painel ao lado do seu Domínio.

Logo no inicio da área de registros na parte superior da tela, você terá acesso\
a todas as entradas criadas na sua área DNS.

**IMPORTANTE:** Escolha o **tipo da entrada que deseja inserir** primeiro.\
Para essa configuração utilizaremos **(CNAME).**

![](https://suporte.love/wp-content/uploads/2022/12/IMG6-300x136.png)

**N 8º –** Clique no campo da entrada **CNAME** ou\
clique em Visualizar para ter acesso as entradas existentes e criar as novas\
entradas.

**IMPORTANTE:** nos próximos passos, utilize as imagens como\
apoio visual e confira sempre as informações inseridas. A grafia (modo de escrever)\
delas é muito importante.\
Se qualquer informação for inserida em formato diferente, ou com espaços em branco\
antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

### **Criando a Entrada de Subdomínio** <a href="#h_01fxb30j1xy1x0hcaa8vmfhf24" id="h_01fxb30j1xy1x0hcaa8vmfhf24"></a>

![](https://suporte.love/wp-content/uploads/2022/12/IMG7-300x90.png)

**N 9º –** Em **Tipo**, selecione a opção **CNAME**

**N 10º –** Em **Entrada**, coloque\
a palavra que você quer que apareça antes do domínio principal.

**EXEMPLO:** se quero que minha entrada de subdomínio seja **click.leadlovers.com.br**,\
o nome da entrada que estou criando tem que ser **click**.

**N 11º –** Já em **Destino**, coloque: **cname.leadlovers.site**

**N 12º –** Verifique as informações inseridas e **em Ações clique em confirmar**.

![](https://suporte.love/wp-content/uploads/2022/12/IMG8-300x21.png)

* O próximo passo é adicionar este subdomínio na sua máquina!\
  [**Clique aqui e veja o passo a passo!**](https://suporte.love/como-cadastrar-dominio-maquina/)

**ATENÇÃO:** Pode levar até 24 horas para as configurações\
sejam totalmente validadas na sua Hospedagem.

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante\
este procedimento, por favor,\
**entre em contato com o nosso suporte**!

🏁 **É isso, terminamos por aqui!**\
com\
amor ❤\
equipe **leadlovers™**
