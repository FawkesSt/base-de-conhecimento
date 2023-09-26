# Como levar leads para outros sistemas pelo Zapier

**Objetivo:** Ensinar como levar leads da leadlovers para outros sistemas pelo Zapier realizando uma integração de exemplo. **Para que serve:** Utilizando o Zapier, é possível fazer com que leads sejam levados da leadlovers para outros sistemas sem ter conhecimento em programação. **Requisitos Obrigatórios: 1.** Ter um plano contratado no [Zapier¹](broken-reference). **2.** Pesquisar se a plataforma que deseja integrar está [cadastrada no sistema](broken-reference). **3.** Ter uma conta na leadlovers com Máquina, Funil e Sequência criados.

* [O que é o Zapier?](broken-reference)
* [O que preciso saber antes de começar?](broken-reference)
* [Configurando o evento](broken-reference)
* [Configurando o gatilho](broken-reference)

### **O que é o Zapier?** <a href="#o-que-e" id="o-que-e"></a>

O Zapier é um **sistema de gestão de integração**. Em poucas palavras, ele faz uma “ponte” entre duas ou mais plataformas, tornando possível integrá-las sem ter nenhum conhecimento em programação.&#x20;

Neste tutorial, ensinaremos como você pode **levar** leads da leadlovers para outros sistemas que também estejam cadastrados no Zapier.&#x20;

Para verificar se a integração está disponível, basta acessar a página [https://zapier.com/apps/webhook/integrations](https://zapier.com/apps/webhook/integrations) e digitar no campo de busca a plataforma que deseja integrar (caso ela tenha tradução, é necessário pesquisar em inglês).

![](https://suporte.love/wp-content/uploads/2023/06/Screenshot\_4-1024x182.png)

### **O que preciso saber antes de começar?** <a href="#o-que-preciso" id="o-que-preciso"></a>

Antes de prosseguir, gostaríamos de chamar a atenção para alguns pontos:&#x20;

1. O Zapier é um sistema **pago**. No entanto, há um plano gratuito com limitações e, nele, são disponibilizados alguns dias de teste das funcionalidades pagas. &#x20;
2. A plataforma Zapier é toda em **inglês**, podendo somente ser traduzida pelo próprio navegador (mas, por ter muitos termos técnicos, pode ser que não seja muito efetivo).&#x20;
3. Ainda não há um aplicativo próprio da leadlovers cadastrado no sistema, o que torna necessário coletar alguns dados mais **técnicos** na leadlovers. Mas não se preocupe, pois iremos explicar todos os passos e informações que serão necessários!
4. Neste tutorial, fizemos uma integração de **exemplo** utilizando o Google Sheets, apenas para ilustrar como funciona o processo no geral. Com outro aplicativo, os passos podem ser **diferentes** dos que serão apresentados neste tutorial.

### **Configurando o evento** <a href="#configurando-evento" id="configurando-evento"></a>

**Nº1–** Dentro do seu painel do Zapier, clique em **“Create Zap”** (**“Criar Zap”**).

![](https://suporte.love/wp-content/uploads/2023/06/Screenshot\_5.png)

**Nº2–** Na primeira etapa, busque pelo aplicativo **“Webhooks by Zapier”** e clique sobre ele.

![](https://suporte.love/wp-content/uploads/2023/06/Screenshot\_11.png)

**Nº3–** Em **“Event”** (**“Evento”**), selecione a opção **“Catch Hook”** (em tradução livre, **“Pegar Gancho”**).

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_15.png" alt="" height="352" width="591"><figcaption></figcaption></figure>

**Nº4–** Clique em **“Continue”** (**“Continuar”**) para prosseguir.

**Nº5–** Esse é o momento de verificar se o gatilho irá funcionar corretamente. Para isso, **copie** a URL gerada no Zapier.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_16.png" alt="" height="421" width="492"><figcaption></figcaption></figure>

Agora será necessário inserir essa URL **na leadlovers**. Abra a plataforma em uma nova guia e crie um [**Gatilho Inteligente**](https://suporte.love/como-criar-e-configurar-acoes-automatizadas/).&#x20;

Nele, você deve primeiramente criar os **filtros** que deseja que os leads atendam para serem enviados para o outro sistema clicando sobre o número que fica logo abaixo de **“Filtros”**.

**Exemplo**: Leads que estão localizados em uma determinada Máquina, Funil e Sequência.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_17-1.png" alt="" height="459" width="319"><figcaption></figcaption></figure>

Depois, você deve criar uma **ação** do tipo [**HttpPost** **Simples** ](https://suporte.love/gatilhos-inteligentes-acao-httppost/)(se quiser enviar apenas campos estáticos) ou **HttpPost** (caso queira enviar campos dinâmicos também).&#x20;

**Observação:** Caso escolha **HttpPost**, é preciso inserir os nomes dos parâmetros que desejar manualmente nos campos que deseja vincular com o outro sistema. Não são permitidos acentos ou espaço. Um exemplo de parâmetro: _EmailDoLead_.

Depois que fizer a sua escolha, você deverá **inserir a URL que copiou no Zapier** e decidir se a comunicação será do tipo **POST** (os parâmetros do lead **não são** exibidos na URL, a mais recomendada) ou **GET** (os parâmetros do lead **são** exibidos na URL).  &#x20;

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_18-2.png" alt="" height="334" width="348"><figcaption></figcaption></figure>

**Nº6–** Depois que finalizar, é necessário fazer um **teste** para ativá-lo. Para isso, clique no ícone de **“aviãozinho”** e preencha os dados que serão solicitados na tela.&#x20;

**Uma mensagem de sucesso deve aparecer em seguida, caso contrário, revise as configurações.**

**Nº7–** Agora volte ao Zapier e clique em **“Test trigger”** (**“Testar gatilho”**).

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_19-1.png" alt="" height="334" width="539"><figcaption></figcaption></figure>

Pode demorar alguns minutos para que o teste seja concluído. Se ele for bem sucedido, aparecerá a mensagem: **“We found a request!”** (“Nós encontramos uma requisição!”). Caso contrário, revise as configurações.

### **Configurando o gatilho** <a href="#configurando-gatilho" id="configurando-gatilho"></a>

**Nº8–** Clique em **“Continue”** (**“Continuar”**) para começar a configurar a **ação**.

**Nº9–** Agora, procure pelo sistema que você deseja integrar e selecione-o na lista.

![](https://suporte.love/wp-content/uploads/2023/06/Screenshot\_20-1.png)

**Nº10–** No nosso exemplo, nós escolhemos o **Google Sheets** para fazer a integração e definimos que o evento que acontecerá nele quando o gatilho for ativado é: **“Create Spreadsheet Row”** (**“Criar uma linha na planilha”**).

Depois que definir essa configuração no aplicativo escolhido, prossiga para os próximos passos.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_21-1.png" alt="" height="349" width="541"><figcaption></figcaption></figure>

**Nº11–** Em seguida, nós escolhemos uma conta do Google para vincular. **OBS:** Esse passo será diferente caso escolha outra plataforma, então é necessário fazer exatamente o que o Zapier solicitar. Para prosseguir, clique em **“Continue”** (**“Continuar”**).

**Nº12–** Na integração com o Google Sheets, são solicitadas algumas informações nesta etapa: em qual Drive está o documento, que planilha deve ser integrada e em qual página dela estão as informações.&#x20;

Quando o Zapier identificou as colunas que já tinham sido criadas dentro da planilha, as relacionamos com os campos da leadlovers.&#x20;

**Por exemplo:** **“Endereço de e-mail”** (da planilha) foi vinculado ao campo **“Email”** (identificado pelo Webhooks by Zapier na leadlovers), e assim por diante.&#x20;

Assim que terminar as configurações solicitadas, **prossiga**.

**Nº13–** Quando chegar na última etapa, você pode **“Testar e Revisar”** (**“Test and Review”**) ou **“Testar e Continuar”** (**“Test and Continue”**).&#x20;

**Nº14–** Se tudo estiver correto, o Zapier informará que testou a ação e que ela funcionou (**“Test was successful!”**). Para publicar a integração, clique em **“Turn on Zap”** (**“Ativar Zap”**).

**Nº15–** Um pop-up aparecerá na tela confirmando que o Zap está ativado. Você pode então copiar seu link (**“Copy Link”**) ou compartilhar as configurações (**“Sharing settings”**). Caso não queira fazer nenhuma das opções, clique fora do pop-up para fechá-lo.

Depois que tudo estiver pronto, é possível realizar um teste **simulando uma situação real**.&#x20;

No nosso caso, cadastramos um novo lead na máquina que informamos nos filtros do Gatilho Inteligente e, depois de alguns minutos, conferimos na planilha se o mesmo tinha sido inserido com sucesso como configuramos.

