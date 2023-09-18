# Como levar leads para outros sistemas pelo Pluga

**Objetivo:** Ensinar como levar leads para outros sistemas pelo Pluga realizando uma integração de exemplo.\
**Para que serve:** Utilizando o Pluga, é possível fazer com que leads sejam levados da leadlovers para outros sistemas sem possuir conhecimento em programação.\
**Requisitos Obrigatórios: 1.** Ter um plano contratado no [Pluga¹](broken-reference). **2.** Pesquisar se a plataforma que deseja integrar está [cadastrada no sistema](broken-reference). **3.** Ter uma conta na leadlovers com Máquina, Funil e Sequência criados.

* [O que é o Pluga?](broken-reference)
* [O que preciso saber antes de começar?](broken-reference)
* [Realizando a integração](broken-reference)

### **O que é o Pluga?** <a href="#o-que-pluga" id="o-que-pluga"></a>

O Pluga é um **sistema de gestão de integração**. Em poucas palavras, ele faz uma “ponte” entre duas ou mais plataformas, tornando possível integrá-las sem ter nenhum conhecimento em programação.&#x20;

Neste tutorial, ensinaremos como você pode **levar** leads da leadlovers para outros sistemas que também estejam cadastrados no Pluga.&#x20;

Para consultar se a integração está disponível, basta acessar esse link: [https://pluga.co/ferramentas/leadlovers/integracao/](https://pluga.co/ferramentas/leadlovers/integracao/) e digitar no campo de busca a plataforma desejada, como no GIF de exemplo abaixo.&#x20;

![img01.gif](https://leadloverssupport.zendesk.com/hc/article\_attachments/6210031311245/img01.gif)

### **O que preciso saber antes de começar?** <a href="#o-que-preciso" id="o-que-preciso"></a>

Antes de prosseguir, gostaríamos de chamar a atenção para alguns pontos:&#x20;

1. O Pluga é um sistema **pago**. No entanto, há um plano gratuito com limitações e, nele, são disponibilizados alguns dias de teste das funcionalidades completas. &#x20;
2. Neste tutorial, fizemos uma integração de **exemplo** utilizando o Google Sheets, apenas para ilustrar como funciona o processo no geral. Com outro aplicativo, é necessário seguir os passos indicados pelo Pluga, que podem ser **diferentes** dos que serão apresentados neste tutorial.

### **Realizando a integração** <a href="#realizando-integracao" id="realizando-integracao"></a>

Recentemente, o Pluga implementou a automatização guiada, com um passo a passo descrevendo exatamente o que precisa ser feito para que tudo funcione corretamente. Mostraremos a seguir como ela funciona.

**Nº1–** No painel inicial depois de logar na plataforma, clique em **“Iniciar”** para começar o processo.

![img02.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6210013589517/img02.png)

**Nº2–** Selecione a **primeira ferramenta** que deseja integrar. Nesse caso, seria a própria leadlovers.

**Nº3–** Clique em **“Escolher segunda ferramenta”**.

![img03.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6210063731725/img03.png)

**Nº4–** Agora, selecione a **segunda ferramenta** que deseja integrar (pode usar o campo de busca para encontrar mais rapidamente). No nosso caso, escolhemos o Google Sheets para exemplificar o processo.

**Nº5–** Prossiga clicando em **“Plugar e Continuar”**.

![img04.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6209997473165/img04.png)

**Nº6–** O próximo passo é escolher qual automatização deseja fazer. O próprio Pluga irá mostrar quais são possíveis, no nosso caso escolhemos: **“Quando um novo lead for criado na leadlovers, inserir em uma planilha no Google Sheets”**.

![img05.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6209982121613/img05.png)

**Observação:** Ao longo do processo, alguns balões explicativos aparecerão. É importante que eles sejam lidos, afinal as informações que estão neles podem ser importantes para realizar a integração corretamente.

![img06.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6210144212621/img06.png)

**Nº7–** Na tela seguinte, haverá uma breve explicação de **por que usar** e **como funciona** a integração escolhida. Recomendamos que leia atentamente e quando tiver certeza que é o que deseja, clique em **“Fazer essa automatização”**.

![img07.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6210365370253/img07.png)

**Nº8–** Quando começar o processo, basta seguir o que o Pluga orienta. Nessa primeira etapa do nosso exemplo, nós tivemos que conectar a conta leadlovers e a conta do Google.&#x20;

Faça também o que a plataforma solicitar e depois continue.

![img08.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6210348700813/img08.png)

**Nº9–** Na segunda etapa, o Pluga solicitou que selecionasse a planilha e a página. Em outras integrações, podem ser necessárias informações diferentes, mas o próprio sistema irá orientar o que precisa ser feito.&#x20;

Depois que configurar tudo corretamente, clique em **“Continuar”**.

![img09.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6210320670605/img09.png)

**Observação:** Ao clicar em **“Bem-vindo(a)!”** na lateral esquerda, é possível ver todo o progresso dos passos da automação e quanto falta para concluir.

![img10.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6210013261069/img10.png)

**Nº10–** Esse foi o momento de relacionar os campos de cada uma das plataformas. Vinculamos a coluna **“Email”** do Google Sheets\
com o campo **“Email”** da leadlovers, mas na lateral direita é possível relacionar outro campo estático ou dinâmico (disponível apenas em planos pagos).

![img11.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6210320533517/img11.png)

Assim que todos os passos solicitados forem feitos, basta clicar em **“Finalizar Automatização”**.

![img12.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6209981546893/img12.png)

Uma mensagem de sucesso aparecerá. Para testar se está funcionando corretamente, basta **simular o evento** que deverá desencadear o gatilho e verificar se o lead da leadlovers foi adicionado no sistema escolhido.&#x20;

No nosso caso, por exemplo, precisaríamos cadastrar um novo lead na leadlovers e conferir depois de alguns minutos se o mesmo foi adicionado na planilha do Google Sheets.

![img13.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6210031112205/img13.png)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, **entre em contato com o nosso suporte**!

**Artigos Relacionados**

**–**[ Como trazer leads de outros sistemas pelo Pluga](https://suporte.love/como-trazer-leads-de-outros-sistemas-pelo-pluga/)\
**–**[ Como trazer leads de outros sistemas pelo Zapier](https://suporte.love/como-trazer-leads-de-outros-sistemas-pelo-zapier/)\
**–**[ Como levar leads para outros sistemas pelo Zapier](https://suporte.love/como-levar-leads-para-outros-sistemas-pelo-zapier/)

🏁 **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
