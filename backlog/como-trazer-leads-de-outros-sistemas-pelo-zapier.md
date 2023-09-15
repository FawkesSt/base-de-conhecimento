# Como trazer leads de outros sistemas pelo Zapier

**Objetivo:** Ensinar como trazer leads de outros sistemas pelo Zapier realizando uma integração de exemplo.\
**Para que serve:** Utilizando o Zapier, é possível fazer com que leads sejam trazidos de outros sistemas para a leadlovers sem ter conhecimento em programação.\
**Requisitos Obrigatórios: 1.** Ter um plano contratado no [Zapier¹](broken-reference). **2.** Pesquisar se a plataforma que deseja integrar está [cadastrada no sistema](broken-reference). **3.** Ter uma conta na leadlovers com Máquina, Funil e Sequência criados.

* [O que é o Zapier?](broken-reference)
* [O que preciso saber antes de começar?](broken-reference)
* [Configurando o evento](broken-reference)
* [Configurando o gatilho](broken-reference)

### **O que é o Zapier?** <a href="#o-que-e" id="o-que-e"></a>

O Zapier é um **sistema de gestão de integração**. Em poucas palavras, ele uma “ponte” entre duas ou mais plataformas, tornando possível integrá-las sem ter nenhum conhecimento em programação.&#x20;

Neste tutorial, ensinaremos como você pode **levar** leads da leadlovers para outros sistemas que também estejam cadastrados no Zapier.&#x20;

Para verificar se a integração está disponível, basta acessar a página [https://zapier.com/apps/webhook/integrations](https://zapier.com/apps/webhook/integrations) e digitar no campo de busca a plataforma que deseja integrar (caso ela tenha tradução, é necessário pesquisar em inglês).

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_4-1024x182.png" alt="" height="124" width="699"><figcaption></figcaption></figure>

### **O que preciso saber antes de começar?** <a href="#o-que-preciso-saber" id="o-que-preciso-saber"></a>

Antes de prosseguir, gostaríamos de chamar a atenção para alguns pontos:&#x20;

1. O Zapier é um sistema **pago**. No entanto, há um plano gratuito com limitações e, nele, são disponibilizados alguns dias de teste das funcionalidades pagas. &#x20;
2. A plataforma Zapier é toda em **inglês**, podendo somente ser traduzida pelo próprio navegador (mas, por ter muitos termos técnicos, pode ser que não seja muito efetivo).&#x20;
3. Ainda não há um aplicativo próprio da leadlovers cadastrado no sistema, o que torna necessário coletar alguns dados mais **técnicos** na leadlovers. Mas não se preocupe, pois iremos explicar todos os passos e informações que serão necessários!
4. Neste tutorial, fizemos uma integração de **exemplo** utilizando o Google Sheets, apenas para ilustrar como funciona o processo no geral. Com outro aplicativo, os passos podem ser **diferentes** dos que serão apresentados neste tutorial.

### **Configurando o evento** <a href="#configurando-evento" id="configurando-evento"></a>

**Nº1–** Dentro do painel da sua conta do Zapier, no menu lateral clique em **“Create Zap”** (**“Criar zap”**).

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_5.png" alt="" height="301" width="259"><figcaption></figcaption></figure>

**Nº2–** Você será direcionado a uma nova tela com um fluxograma, no primeiro quadro, dê um duplo clique e abrirá uma nova janela.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_6.png" alt="" height="191" width="661"><figcaption></figcaption></figure>

**Nº3–** D**igite no campo de busca o sistema do qual deseja trazer leads para a leadlovers. No nosso exemplo, usaremos o  “Google Sheets”.**

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_7-1024x628.png" alt="" height="413" width="674"><figcaption></figcaption></figure>

**Nº4–** Após isso é preciso selecionar o tipo de  evento. Em nosso caso, escolhemos: **“New or Updated Spreadsheet Row”** (**“Linha da planilha criada ou atualizada”**), ou seja, sempre que uma linha for criada ou atualizada na planilha, o gatilho deverá ser executado.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_8.png" alt="" height="405" width="515"><figcaption></figcaption></figure>

**Nº5–**Após isso, clique em **“Continue”** (**“Continuar”**) para prosseguir.

**Nº6–** Na próxima etapa, é preciso efetuar o login do Google conforme solicitado pelo Zapier.

**Obs.** Após efetuar o login, o Zapier irá trazer as informações de acordo com o sistema que você está tentando integrar. Preencha os dados solicitados para a plataforma que você escolheu e continue com as configurações.

**Nº7–** Na integração com o Google Sheets, são solicitadas algumas informações nesta etapa: qual planilha deve ser integrada, em qual página dela estão as informações e que coluna ativará o gatilho (sempre que a coluna indicada aqui for preenchida, a ação configurada acontecerá).

Depois que completar todas as informações solicitadas pelo Zapier para a plataforma escolhida, clique em **“Continue”** (**“Continuar”**) para prosseguir.

**Nº8–** Quando tudo estiver configurado, clique em **“Test your trigger”** (**“Teste seu gatilho”**) para que o Zapier realize um teste do gatilho. No caso do nosso exemplo, o sistema procurará por uma linha preenchida dentro da planilha para verificar se tudo está correto.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_9.png" alt="" height="341" width="468"><figcaption></figcaption></figure>

**Nº9–** Se houver sucesso no teste, pode continuar com a configuração.

### **Configurando o gatilho** <a href="#configurando-gatilho" id="configurando-gatilho"></a>

Depois que terminar de configurar o **evento**, é hora de partir para a **ação**.&#x20;

**Nº10–** No segundo passo (Step), dê um duplo para abrir.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_10.png" alt="" height="319" width="506"><figcaption></figcaption></figure>

**Nº11–** Na nova janela escolha a ação : **“Webhooks by Zapier”.**

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_11.png" alt="" height="188" width="340"><figcaption></figcaption></figure>

**Nº12–** No tipo de evento, selecione a opção **“POST”**.

**Nº13–** Clique em **“Continue”** (**“Continuar”**) para prosseguir.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_12-1024x589.png" alt="" height="374" width="650"><figcaption></figcaption></figure>

**Obs:** Para prosseguir após essa etapa, é necessário abrir a sua conta da leadlovers em outra aba e seguir o tutorial a de como gerar um [**WebHook**](https://suporte.love/como-criar-um-webhook/).&#x20;

Quando ele terminar as configurações do Webhook na leadlovers, prossiga com as configurações no zapier.

**Nº14–** Insira aqui a URL criada no WebHook da leadlovers, ela aparecerá no campo **“Endereço do WebHook (URL)”**. Basta copiar e colar.

**Nº15–** Em **“Payload Type”**, escolha **“json”**.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_13.png" alt="" height="498" width="513"><figcaption></figcaption></figure>

Já em **“Data”**, devem ser inseridos todos os dados que chegarão até a leadlovers, isso inclui o lugar (Máquina) em que o lead deve ser inserido, assim como quais informações serão adicionadas a ele.&#x20;

**Nº16–** Então, primeiramente, informe qual é a **Máquina**. Para isso, basta consultar o seu Webhook e depois preencher no Zapier com as informações que foram geradas: no primeiro campo, insira **“MachineCode”** e, no segundo, o **código da máquina** que foi fornecido.

**Nº17–** Clique em **“+”** para inserir um novo campo e preencha com as informações da **Sequência de E-mail**: no primeiro espaço, coloque **“EmailSequenceCode”** e, em seguida, o seu **código numérico** fornecido no WebHook.

**Nº18–** Também é necessário dizer em qual **Nível da Sequência** o lead entrará, então crie um novo campo com os seguintes dados: no campo menor, insira **“SequenceLevelCode”** e, no maior, coloque o número correspondente que foi gerado no seu WebHook.

**Nº19–** Além disso, você também precisa informar aqui **quais dados do lead** deseja trazer para a leadlovers, inserindo o seu nome e vinculando com o mesmo campo da plataforma escolhida para integração.&#x20;

No nosso exemplo, colocamos **“Name”** (**“Nome”**) e vinculamos com a coluna **“Qual o seu nome?”** de nossa planilha.

**Nº20–** Faça o mesmo com os outros dados que deseja inserir. Logo depois do print, há uma [**tabela**](broken-reference) mostrando como os campos estáticos devem ser preenchidos no Zapier (a primeira coluna é como é o campo na leadlovers e a segunda é como ele deve ser inserido no Zapier):

**Atenção:** Somente é possível trazer **campos estáticos** pelo Zapier.

**Tabela 1:** Relação de campos leadlovers x Zapier.

| Campos Estáticos na leadlovers | Campos Estáticos no Zapier |
| ------------------------------ | -------------------------- |
| Nome                           | Name                       |
| E-Mail                         | Email                      |
| Empresa                        | Company                    |
| Telefone                       | Phone                      |
| Cidade                         | City                       |
| Estado                         | State                      |
| Data De Nascimento             | Birthday                   |
| Mensagem                       | Message                    |
| Lead Score                     | Score                      |
| Tag                            | Tag                        |
| Observações                    | Notes                      |

Há algumas outras opções disponíveis na configuração da ação, como por exemplo: **“Wrap Request In Array”**, **“Unflatten”**, entre outras. Não é necessário preenchê-las para que a integração funcione.

**Nº21–** Role a página e, em **“Headers”**, insira no campo menor o dado **“Authorization”** e, no maior, o **“Código Bearer”** gerado em seu Webhook.

**Nº22–** Clique em **“Continue”** para prosseguir.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_14.png" alt="" height="206" width="656"><figcaption></figcaption></figure>

**Nº23–** Nesta etapa, clique em **“Test and Continue”** (**“Testar e Continuar”**).

**Nº24–** Se tudo estiver certo, o **“StatusCode”** será número 200 e haverá uma mensagem sobre a ação que foi realizada. Basta clicar em **“Turn on Zap”** (**“Ativar Zap”**)\
para publicar sua integração.

**Nº25–** Um pop-up abrirá confirmando que a sua integração está ativa. Nele, você pode decidir ir para a sua tela de Zaps (**“Go to My Zaps”**) ou transferir os dados já existentes (**“Transfer existing data”**).

**OBS:** Se desejar, faça um teste na integração depois de ativada, realizando uma **simulação** do evento que configurou.&#x20;

No nosso exemplo, nós acrescentamos uma linha na planilha e, como tudo ocorreu com sucesso, o lead entrou na leadlovers com a origem **“API LL”**.

