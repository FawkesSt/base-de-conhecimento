# Instalando os Eventos do pixel do Facebook

**Objetivo:** ensinar como metrificar eventos do pixel Facebook nas páginas leadlovers.\
**Para que serve:** rastrear efetivamente eventos do Facebook em casos em que o lead não está usando iOS 14, com o bloqueio de rastreio na web ou qualquer outro dispositivo com bloqueador de anúncios.\
**Requisito(s) necessário(s):** **1.** possuir o pixel do Facebook [instalado e _validado_](https://suporte.love/instalar-pixel-fb/) em suas páginas ou máquina na leadlovers.

#### **Escolhendo a forma de configuração** <a href="#como-configurar" id="como-configurar"></a>

É possível configurar o Facebook Pixel com a instalação manual do código nas páginas ou com a ferramenta de configuração de eventos. As configurações são feitas de maneiras diferentes e é muito importante frisar que para utilizar a **API de conversões** será necessário configurar os eventos _manualmente_ via código, portanto, recomendamos que seja feito dessa forma.

Abaixo explicamos a diferença entre as duas maneiras de instalar.

**Instalação manual via código:** você pode fazer tranquilamente mesmo sem um entendimento a fundo de códigos HTML. O que precisa ser feito é acessar uma biblioteca do Facebook, copiar o código do evento desejado e inserir em uma parte específica do código da página. A leadlovers possui um campo exclusivo para esses códigos, o que facilita a inserção. Essa configuração permite o uso da **API de conversões**.

**Instalação via ferramenta de configuração de eventos:** caso você prefira fazer da forma mais fácil (como o próprio Facebook diz), você precisará apenas selecionar em qual URL deseja fazer a configuração e fará utilizando o mouse tudo em poucos cliques direto na página.

#### **Instalação manual via código** <a href="#instalacao-manual" id="instalacao-manual"></a>

**Copiando código**

Nesse tipo de configuração é importante lembrar que não é necessário apagar os códigos já existentes em sua página, basta pular uma linha dando Enter e colar os novos.\
O primeiro passo é copiar o código referente ao evento que deseja metrificar.

**Nº1–** Acesse a [biblioteca de eventos](https://www.facebook.com/business/help/402791146561655?id=1205376682832142) do Facebook.

**Nº2–** Copie o código do evento desejado e guarde em um local de fácil acesso, o bloco de notas pode ser um grande aliado. Nesse exemplo utilizaremos o evento “Cadastro”, logo o código copiado será: _fbq(‘track’, ‘Lead’);_ .

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem0.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem0.png)

**Observação:** o Facebook sugere que o código (snippet) do evento seja configurado no BODY, separadamente do código do Pixel, e dessa maneira também é possível realizar essa configuração. Contudo, identificamos que para que a API de Conversões do próprio FB funcione (aquela que ajuda a metrificar o Pixel/Evento em dispositivos com o iOS 14) a maneira “correta” de instalar o Evento é como ensinaremos a seguir.

Se escolheu essa forma de configuração, você ainda deve decidir se instalará o evento em todas as páginas de um domínio ([em toda a máquina](broken-reference)) ou se será somente em uma ou algumas [páginas específicas](broken-reference), isso vai depender de sua estratégia de metrificação. Mostraremos as duas formas a seguir.

**Em uma página**

O método a seguir é para configurar um evento em somente uma página. Caso deseje configurar o evento em algumas páginas específicas, precisará repetir este método página por página.

**Nº3–**  Na leadlovers, acesse a aba “Páginas” dentro da máquina.

**Nº4–**  Clique sobre a engrenagem ao lado da qual deseja configurar o evento.

**Nº5–**  Iremos alterar as configurações da mesma.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem1a.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem1a.png)

**Nº6–**  Vá até a aba “Configurações Avançadas”.

**Nº7–**  Em “Scripts do Cabeçalho (HEAD)” cole o código do evento que você escolheu e copiou da biblioteca do Facebook, pulando uma linha usando a tecla Enter após o _fbq(‘track’, ‘PageView’);_ .

**Nº8–**  Salve as configurações. Não há limite de eventos por página, para instalar mais de um basta dar Enter e colar abaixo do anterior.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem2.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem2.png)

Evento instalado na página com sucesso! Lembre-se de [testar](broken-reference).

**Em uma máquina**

Se você deseja metrificar um mesmo evento em todas as páginas de sua máquina, deve realizar a instalação direto nas configurações gerais da mesma. Lembrando que aqui estamos somente exemplificando como fazer a configuração, mas sugerimos para melhor análise que o evento “Cadastro” seja sempre usado em páginas de obrigado/próximos-passos.

**Nº3–**  Na leadlovers, já na máquina em que deseja fazer a instalação do evento, acesse a aba “Configurações”.

**Nº4–** Vá até a seção “Scripts Globais(HEAD)”.

**Nº5–**  Em “Scripts do Cabeçalho (HEAD)” cole o código do evento que você escolheu e copiou da biblioteca do Facebook, pulando uma linha usando a tecla Enter após o _fbq(‘track’, ‘PageView’);_ .

**Nº6–**  Sempre se lembre de salvar as configurações. Não há limite de eventos por máquina, para instalar mais de um basta dar Enter e colar abaixo do anterior.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem3.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem3.png)

Evento instalado na página com sucesso! Não esqueça de [testar](broken-reference).

#### **Instalação via ferramenta de configuração de eventos** <a href="#instalacao-facebook" id="instalacao-facebook"></a>

Essa forma de configuração é feita através de um pop-up do Facebook direto em sua página. É importante frisar que nessa ferramenta serão possíveis somente as configurações de eventos que o Facebook previamente identificar e que usando esse tipo de configuração _**não é possível utilizar a API de conversões**_ disponibilizada na plataforma.\
Ela também permite que você gere métricas sobre todo um domínio ou referente a somente uma página. Por conta disso, o início das configurações é idêntico, a diferença está após o passo Nº11.

**Nº1–**  Clique em “Mais Ferramentas”.

**Nº2–** Acesse o “Gerenciador de Eventos”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem6.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem6.png)

**Nº3–**  Selecione o pixel em que está a página que deseja metrificar eventos.

**Nº4–**  Clique em “Adicionar Eventos”.

**Nº5–**  Escolha “Do pixel”, onde possui uma seta de cursor que ilustra esse tipo de configuração.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem7.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem7.png)

Feito isso abrirá uma pop-up.

**Nº6–**  Nela clique sobre o botão “Abrir a ferramenta de configuração de eventos”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem8.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem8.png)

Agora você precisará definir se deseja que esse mesmo evento seja para somente para uma página específica ou todo o seu domínio.

**Nº7–**  Aqui cole o link de sua página ou domínio.\
O ideal é sempre utilizar e divulgar com o “https”, pois incentivamos o uso do certificado SSL em páginas criadas na leadlovers e disponibilizamos esse recurso gratuitamente.

**Nº8–**  Clique em “Abrir site”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem9.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem9.png)

Feito isso, abrirá sua página em uma nova guia com a ferramenta do Facebook para instalação do evento. Você consegue optar por metrificar o evento pelo simples acesso ao link de seu domínio/página (Rastrear uma URL) ou pelo clique em algum botão da mesma (Rastrear novo botão).\
Nesse exemplo veremos como configurar para aplicar o evento “Cadastro” para quando alguém acessar o link.\
Reforçando que isso é somente um exemplo e que recomendamos a inserção desse evento nas páginas de obrigado/próximos-passos e não nas páginas de cadastro.

**Nº9–** Clique em “Rastrear uma URL”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem10.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem10.png)

**Nº10–**  Escolha o evento desejado.

**Nº11–**  Automaticamente, o Facebook puxará o link inserido no passo 07, mas é aqui que você definirá se essa configuração valerá para todo o domínio ou somente para uma página específica. Usaremos de exemplo quando é em somente uma página.

Se deseja que seja somente para a **página**, deixe da forma que está:\
URL igual a; seudominio.com.br/nome-da-página.

Se deseja que seja para todo o **domínio**, altere para:\
URL contém; seudominio.com.br.

**Nº12–**  Escolha “Não incluir valor”, pois nas páginas leadlovers não utilizamos carrinho de compras.

**Nº13–**  Salve as configurações.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem11.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem11.png)

**Nº14–**  Clique em “Concluir Configurações”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem12.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem12.png)

Será mostrado em uma nova pop-up qual ou quais eventos foram configurados.

**Nº15–**  Verifique se está correto e depois clique em concluir.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem13.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem13.png)

Se desejar, avalie a ferramenta ou pule esta etapa. Após isso, você será redirecionado de volta para a página principal do pixel.

Evento instalado na página ou domínio com sucesso! Sempre se lembre de [testar](broken-reference).

#### **Testando o evento** <a href="#teste" id="teste"></a>

Também há duas formas de validar se o evento está sendo metrificado e enviado ao Facebook corretamente.\
A primeira é [dentro do próprio FB](broken-reference) e também agiliza na validação do pixel que veremos depois.\
O segundo jeito é através de uma [extensão do Google Chrome](broken-reference) e pode ser mais “na mão” se você tiver feito a instalação manual do código. Pois basta acessar o link da página/domínio e, pela extensão do próprio navegador, já consegue confirmar se o código está ou não inserido em seu domínio/página.

**Via Eventos de Teste**

**Nº16–**  Na tela principal do pixel em que foi criado o evento, vá até a aba “Eventos de Teste”.

**Nº17–**  Caso já tenha feito eventos de teste anteriormente, limpe a atividade.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem15.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem15.png)

**Nº18–**  Insira a URL do domínio ou página em que configurou o evento.

**Nº19–**  Clique em “Abrir Site”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem16.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem16.png)

**Nº20–**  Isso abrirá a página em uma guia. Como nosso evento é somente de acesso basta aguardar a página carregar e fechar, mas caso utilize algum evento de clique ou qualquer outro, replique a ação configurada. A intenção aqui é simular o evento e ver se ele é encaminhado corretamente para o Facebook.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem17.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem17.png)

**Nº21–**  Após fechar a página, volte para o Gerenciador de eventos do Facebook. Na aba em que já estávamos, chamada ”Eventos de Teste”, aparecerá os eventos mensurados. Se mostrar os eventos configurados, está tudo certo!

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem18.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem18.png)

Caso não mostre os eventos, revise todos os passos deste tutorial. Se ainda assim não validar, entre em contato com nosso time de suporte.

**Via Extensão Google Chrome**

Caso não possua essa extensão, mostramos como instalar [nesse artigo](https://suporte.love/instalar-pixel-fb/).

**Nº16–**  Acesse a página ou o domínio em que foi configurado o evento no navegador Google Chrome.

**Nº17–**  Caso tenha configurado alguma ação na página como clique, por exemplo, simule-a. Já se os eventos configurados foram somente de acesso, como no caso do evento de Cadastro, basta acessar a página.

**Nº18–**  Abra a extensão, nela mostrará todos os eventos configurados e enviados para o Facebook.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem19.png)](https://legado.leadlovers.site/wp-content/uploads/2021/08/Imagem19.png)

Caso não apareçam os eventos configurados, revise os passos desse tutorial e, se ainda assim não funcionar, entre em contato com nosso time de suporte.

**Artigos recomendados**

– [O que é Pixel do FB](https://suporte.love/o-que-e-pixel-do-facebook/);

– [Como gerar o Pixel FB](https://suporte.love/gerando-pixel-fb/);

– [Como instalar o Pixel FB](https://suporte.love/instalar-pixel-fb/);

– [API de Conversões FB](https://suporte.love/api-conversao-facebook/);

– Como [inserir um script](https://suporte.love/inserir-script/) nas páginas da leadlovers.

🏁 **É isso, terminamos por aqui!**\
com amor ♥\
equipe **leadlovers™**
