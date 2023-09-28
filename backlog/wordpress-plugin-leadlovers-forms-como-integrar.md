# WordPress Plugin leadlovers forms: Como integrar

**Objetivo:** Mostrar o passo a passo de como configurar qualquer formulário de captura do WordPress ao plugin **leadlovers forms**.\
**Para que serve:** Capturar leads para sua máquina na leadlovers por um formulário de captura que foi criado na sua página do WordPress.\
**Requisitos obrigatórios:**\
**1.** Ter uma página com um formulário de captura criado em seu WordPress utilizando o construtor de sua preferência.

Se você caiu aqui aleatoriamente e não conhece o\
[WordPress](https://br.wordpress.com/),\
não sabe o que é um\
[Plugin](https://br.wordpress.com/install-plugins/)\
nem como isso pode ser integrado ao leadlovers, confere primeiro este artigo:\
[Integração leadlovers com WordPress](https://suporte.love/integracao-leadlovers-com-wordpress/).

Este artigo abrange os seguintes tópicos:

* [O que é?](broken-reference)
* [Integrando leadlovers com WordPress](broken-reference)
* [Configurando um formulário de captura com o plugin leadlovers forms](broken-reference)
* [Testando a integração](broken-reference)

### **O que é?** <a href="#o-que-e" id="o-que-e"></a>

Com o plugin **leadlovers forms**, é possível utilizar seu formulário\
nativo criado no WordPress com qualquer construtor e fazer com que os leads que\
se cadastrem por ele entrem em uma máquina na leadlovers, sem precisar fazer\
integração direta com outros plugins ou inserir um formulário criado aqui por\
código HTML.

Para que funcione, basta instalar um plugin no seu WordPress, configurá-lo na\
página em que o formulário está e fazer o mapeamento dos campos dele com os que\
estão na leadlovers, como ensinaremos a seguir.

### **Integrando leadlovers com WordPress** <a href="#realizando-integracao" id="realizando-integracao"></a>

Primeiramente, dentro do painel do WordPress, será preciso instalar o plugin que vai possibilitar essa integração entre a página com o formulário e a leadlovers.

**Nº1–** Acesse a aba **“Plugins”** no canto esquerdo da tela dentro do menu principal.

**Nº2–** Clique em **“Adicionar novo”**.

**Nº3–** Na barra de pesquisa, busque por **“leadlovers forms”**.

**Nº4–** Assim que aparecer o plugin, selecione a opção **“Instalar agora”**. Após concluir a instalação, será evidenciado o botão **“Ativar”**. Clique nele para ativar o plugin em seu WordPress.

![img01.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/5020003199373/img01.png)

#### **Menu “Configurações”**

**Nº5–** Após ativar o plugin, vá até a aba **“Leadlovers”** na lateral esquerda do seu WordPress. O primeiro menu que abrirá será o de **“Configurações”**, permaneça nele.

**Nº6–** Em **“Chave de api”**, insira o [**Token Pessoal**](https://suporte.love/como-localizar-o-seu-token-pessoal-na-leadlovers/) da sua conta leadlovers.

**Nº7–** Clique em **“Salvar alterações”**.

![img02.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/5019981861517/img02.png)

Aparecerá uma mensagem de sucesso assim que as configurações forem salvas.

![img03.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/5019981967117/img03.png)

#### **Menu “Minhas integrações”**

Na opção **“Minhas Integrações”**, aparecerão todas as integrações já configuradas, com o **título** do\
formulário, **data** de publicação, em qual **página** foi inserido, para qual **máquina**, **funil** e **sequência** está capturando e se o formulário está **ativo ou não**.

**Observação:** Você poderá configurar mais de um formulário por página, se desejar.

![img04.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/5019982058765/img04.png)

#### **Menu “Log de capturas”**

Já no menu **“Log de Captura”,** mostrará todo o histórico de capturas realizadas. Nele constará o **título** do\
formulário, **data** de publicação, **página** em que ele está, para qual **máquina**, **funil** e **sequência** está enviando o lead e quais foram as **informações capturadas**.

![img05.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/5019948194061/img05.png)

#### **Menu “Log de erros”**

Por fim, em **“Log de Erros”** aparecerá todo o histórico de erros de captura para análise, se houver.

![img06.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/5019982325005/img06.png)

### **Configurando um formulário de captura do WordPress com o plugin leadlovers forms** <a href="#configurando-formulario" id="configurando-formulario"></a>

Depois que vincular a sua conta da leadlovers ao WordPress, será necessário configurar\
o formulário para que os leads capturados sejam enviados para a leadlovers.

**Nº8–** Ainda dentro do painel do seu WordPress, clique em **“Páginas”**.

**Nº9–** Selecione a opção **“Ver”** na página que deseja integrar o plugin.

**IMPORTANTE:** É obrigatório que nessa página **já exista** um formulário de captura com pelo menos o campo de **E-mail** (caso queira enviar os leads para uma **Máquina de E-mail**) ou **Telefone** (se quiser adicionar os leads em uma **Máquina de SMS**, **Voz** ou **Telegram**) criados.

![img07.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/5019948246925/img07.png)

**Nº10–** Encontre o formulário de captura desejado e clique no ícone da leadlovers que está ativo (com a cor rosa). Serão disponibilizados campos para a integração ser efetuada.

**ATENÇÃO:** Caso o botão esteja cinza, é porque ainda não é possível integrar o formulário com a leadlovers. Para isso, é necessário que ele tenha um identificador (ID) em sua estrutura. Em breve, lançaremos um guia de como adicionar um ID nos principais temas de formulários do WordPress.

![img08.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/5020530865805/img08.png)

**Nº11–** Quando o interruptor está escrito **“Habilitado”**, significa que o formulário está ativo. Ao desabilitá-lo, as capturas serão interrompidas.

**Nº12–** Em **“Destino do lead”**, escolha a **Máquina**, **Funil** e **Sequência** nos quais o lead será inserido.&#x20;

**Nº13–** No menu **“Configurações do lead”**, é possível escolher tags para adicionar na captura.

**Nº14–** Para prosseguir, clique em **“Próximo passo”**.&#x20;

![img09.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/5019981594509/img09.png)

**Nº15–** Nesse próximo passo, você deverá configurar o **“Mapeamento dos campos do formulário”**, ou seja, relacionar os campos do formulário com os campos da leadlovers, sejam eles **estáticos** ou **dinâmicos** –\
caso ainda não tenha campos dinâmicos criados na plataforma, configure-os **antes** de relacionar no formulário [**clicando aqui**](https://suporte.love/como-criar-campos-dinamicos-e-como-criar-formulario-dinamico/).&#x20;

**Nº16–** Clique em **“Salvar integração”** para aplicar as alterações.

![img10.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/5019986971917/img10.png)

Assim que salvar as alterações, aparecerá uma mensagem de confirmação:

![img11.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/5019948063117/img11.png)

### **Testando a integração** <a href="#testando-integracao" id="testando-integracao"></a>

Para testar a integração, basta abrir a página com o formulário sem estar logado no seu painel do WordPress e simular o cadastro de um lead. Uma maneira simples de abrir a página sem precisar deslogar do seu WordPress, é acessá-la por uma guia anônima (para fazer isso no Google Chrome, é só usar o atalho **Ctrl + Shift + N**).&#x20;

Após realizar a captura, aguarde alguns minutos e então verifique a aba **“Leads”** dentro da máquina que configurou no momento que fez a integração com o formulário.

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante\
este procedimento, por favor,\
**entre em contato com o nosso suporte**!

**Artigos Relacionados**

**–**\
[Integrações leadlovers com WordPress](https://suporte.love/integracao-leadlovers-com-wordpress/)\
**–**\
[Como localizar o Token Pessoal na leadlovers](https://suporte.love/como-localizar-o-seu-token-pessoal-na-leadlovers/)

🏁 **É isso, terminamos por aqui!**\
com\
amor ❤\
equipe **leadlovers™**
