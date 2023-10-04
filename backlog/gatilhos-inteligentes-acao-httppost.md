# Gatilhos Inteligentes: Ação HttpPost

**Objetivo:** Mostrar o passo a passo de uma configuração de ação HttpPost para gatilhos inteligentes.\
**Para que serve:** A função HttpPost serve para enviar **dados dos leads** capturados em sua conta leadlovers **para sistemas externos**_**.**_\
**Requisito Obrigatório:** Possuir um sistema disponível para receber o link com os parâmetros contendo as informações dos leads.

### **Como funciona?** <a href="#como-funciona" id="como-funciona"></a>

Para que a **função do HttpPost** funcione corretamente, é preciso que você já tenha o **link** que irá utilizar para a integração via post com seu sistema externo. Neste link é preciso ter todos os **parâmetros** que deseja que o leadlovers **envie para seu sistema.**\
\
A partir deste link você irá configurar a ação no **gatilho inteligente** dentro do leadlovers, informando o domínio e os parâmetros contidos no link, fazendo com que a leadlovers consiga enviar os dados dos leads que se enquadrem nos filtros do gatilho inteligente para o seu sistema externo.

Os dados do lead que você consegue enviar para seu sistema externo são: **e-mail**, **nome**, **data de nascimento**, **telefone**, **empresa**, **cidade** e **estado**, ressaltando que só será enviado para seu sistema essas informações caso o **lead tenha sido capturado com elas**!

**IMPORTANTE:** Caso você **ainda não saiba como criar um gatilho inteligente**, [**temos este tutorial ensinando como se faz.**](https://suporte.love/criar-e-configurar-gatilhos-inteligentes/) Depois que entender como configurar retorne aqui para aprender a configurar a ação **HttpPost**, beleza?

### **Como configurar a ação HttpPost?** <a href="#como-configurar" id="como-configurar"></a>

**Nº1–** Acesse o gatilho inteligente que você irá configurar o HttpPost e clique em cima da numeração do status **Ações.**[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip1.png)

**Nº2**– Ao abrir a tela, aparecerá um popup clique em **Criar Ação.**

**Nº3–** Em Tipo da Ação escolha a opção **Executar HttpPost**

**Nº4–** No campo **URL** você deve informar o início de seu link, tudo que vier antes dos parâmetros.

**Por exemplo:**

Vamos dizer que o link que irei utilizar é :\
[https://minhaaplicacao.com/meupost?token=0132456789\&email=emailDoLead](https://minhaaplicacao.com/meupost?token=0132456789\&email=emailDoLead)

Nele você encontra **três informações:**

✔ A URL **https://minhaaplicacao.com/meupost;**

✔ O parâmetro referente ao token **token=0132456789**

✔ E outro parâmetro que solicita o e-mail do lead **email**=emailDoLead

Portanto no campo **URL** eu irei informar **apenas o** _https://minhaaplicacao.com/meupost,_ que é tudo que vem antes dos parâmetros.

**Nº5**– Escolha se a comunicação necessário é através de **GET** ou **POST**

**Observação:** Caracteres como **?** e **&** que se encontram pelo link servem para separar a **URL dos parâmetros** e os parâmetros uns dos outros, **ignore-os** pois nesta integração iremos utilizar apenas os dados, beleza?

**IMPORTANTE:** No print abaixo, observe que existe um campo chamado **“Usar Autenticação”**_**.**_ Algumas ferramentas externas, além da URL de autenticação utilizam esses dois componentes (chave e valor) como se fosse um usuário e senha. Isso serve para validar a integração.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip3.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip3.png)

Se o destino do post precisar de autenticação tem que fornecer esses dois campos.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip0.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip0.png)

**Nº6–** Nos campos abaixo do que foi inserida a URL, é aonde você deverá informar os parâmetros referentes aos dados dos leads que você deseja enviar para o sistema externo.

**Por exemplo:**\
Em meu link https://minhaaplicacao.com/meupost?token=0132456789\&email=emailDoLead os **dados do lead** que desejo enviar pro meu sistema externo **é o e-mail** “email=emailDoLead”.

Então eu vou **no campo E-mail** na configuração do gatilho inteligente e coloco ali o dado referente ao parâmetro, que no caso é o email sem o =emailDoLead.\
Vale lembrar que esse parâmetro deve ser o mesmo utilizado dentro do seu sistema externo.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip1-1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip1-1.png)

**Nº7**– Depois de adicionar **todos** os parâmetros de seu link nas configurações do gatilho inteligente, clique em **Salvar** para criá-lo.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip2.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip2.png)

Assim que criar a ação, note que ficará com um ícone vermelho com uma exclamação, ele quer dizer que ainda não foi testada a ação criada. Para que a ação seja ativada e comece a funcionar corretamente é preciso realizar um teste antes, caso contrário a ação será criada mas não irá funcionar, **somente depois de testar**.

**Nº8**– Para testar clique na opção **Teste de execução (ícone de aviãozinho).**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip4.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/gatilhos-inteligentes\_-ao-httppost-360043058133\_mceclip4.png)

**Observação:** Caso dê alguma mensagem de erro as configurações para a comunicação com seu sistema externo não foram realizadas corretamente ou há algo impedindo a comunicação entre as duas plataformas, refaça as configurações e teste novamente.

Pronto, agora o gatilho inteligente já está configurado e ativado. Não se esqueça de testar junto com seu sistema externo antes de iniciar sua campanha, beleza?

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, **entre em contato com o nosso suporte**!

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
