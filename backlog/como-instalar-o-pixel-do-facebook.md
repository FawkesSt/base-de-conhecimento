# Como instalar o Pixel do Facebook?

**Objetivo:** esse artigo mostra como inserir e validar um pixel do Facebook nas páginas ou máquinas criadas leadlovers.\
**Para que serve:** o pixel gera dados de rastreamento sobre sua(s) página(s) que podem ser analisados na sua conta do FB Business.\
**Requisito(s) Obrigatório(s):** **1.** ter o [pixel gerado](https://suporte.love/gerando-pixel-fb/); **2.** possuir uma [página criada](https://suporte.love/componentes-visao-geral/) e _ativa_ na leadlovers; **3.** definir uma [rota válida](https://suporte.love/como-cadastrar-dominio-maquina/) para o domínio cadastrado na máquina.

#### **Validando o domínio** <a href="#validar-dominio" id="validar-dominio"></a>

Antes de começarmos, precisamos confirmar se o domínio no qual você deseja instalar o pixel tem uma [rota válida](https://suporte.love/como-cadastrar-dominio-maquina/).

**Nº1–** Nas Configurações da máquina onde seu domínio está, acesse o menu Domínios e Rotas e verifique se a Rota do seu domínio está definida para uma página específica e não como aleatória.

#### **Instalação do pixel** <a href="#instalando-pixel" id="instalando-pixel"></a>

Para facilitar o procedimento, mantenha a leadlovers e sua conta Business do Facebook abertas.

Após validar se seu domínio abre corretamente a página configurada, podemos copiar o código e instalar o pixel na máquina ou em páginas específicas.

**Copiando o código**

**Nº2–** Após ter gerado o [código do pixel](https://suporte.love/gerando-pixel-fb/), acesse o [gerenciador de eventos do Facebook](https://business.facebook.com/events\_manager2).\
**Nº3–** Selecione o pixel que deseja configurar.\
**Nº4–** Clique em “Continuar a configuração do Pixel”.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem3.png" alt=""><figcaption></figcaption></figure>

**Nº5–** Feito isso abrirá uma pop-up, nela selecione “Pixel do Facebook”.\
**Nº6–** Para prosseguir clique em “Conectar”.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem4.png" alt=""><figcaption></figcaption></figure>

**Nº7–** Agora escolha a opção ”Adicionar manualmente o código do pixel ao site”.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem5.png" alt=""><figcaption></figcaption></figure>

**Nº8–** Copie o código e guarde-o em um local seguro, o bloco de notas pode ser um excelente aliado.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem6.png" alt=""><figcaption></figcaption></figure>

**Definindo o local de aplicação**

Agora será necessário definir se a instalação será feita em todas as páginas de um domínio ([em toda a máquina](broken-reference)) ou se será somente em uma ou algumas [páginas específicas](broken-reference), isso vai depender de sua estratégia de metrificação. Mostraremos as duas formas a seguir.

**Em todo o domínio ou máquina**

Se você deseja metrificar o Pixel em sua máquina, deve realizar a instalação direto nas configurações gerais da mesma.&#x20;

**IMPORTANTE:** Este método replica os códigos inseridos em todas as páginas presentes em sua máquina.

**Nº9–** Volte à **leadlovers** na máquina em que está instalando o pixel.\
**Nº10–** Vamos para a aba “Configurações”.\
**Nº11–** Acesse a seção “Scripts Globais (HEAD)”.\
**Nº12–** Cole aqui o código copiado no passo Nº11. Caso você já possua outros códigos adicionais em sua máquina, não se preocupe, basta pular uma linha dando Enter e colar abaixo, como no exemplo.\
**Nº13–** Salve as configurações.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem7.png" alt=""><figcaption></figcaption></figure>

Código inserido com sucesso na máquina e aplicado em todas as páginas da mesma! Agora é preciso [**testar a aplicação do pixel**](broken-reference), pois a validação do mesmo é essencial para o funcionamento.

**Em páginas específicas**

O método a seguir é para configurar o pixel em somente uma página. Caso deseje configurar o pixel em algumas páginas específicas, precisará repetir este método página por página.

**Nº9–** Agora acesse a leadlovers, e na máquina em que se encontra a página onde deseja inserir o pixel, vá até a aba “Páginas”.\
**Nº10–** Ao lado da miniatura da página existe um ícone de engrenagem, clique sobre ele.\
**Nº11–** Escolha a opção “Configurações”.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem9.png" alt=""><figcaption></figcaption></figure>

**Nº12–** Vá até a aba “Configurações avançadas”.\
**Nº13–** No campo “Scripts do Cabeçalho (HEAD)” cole o código de seu pixel. Caso você já possua outros códigos adicionais em sua página, não se preocupe! Basta pular uma linha dando Enter e colar abaixo, como no exemplo.\
**Nº14–** Salve as configurações feitas.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem10.png" alt=""><figcaption></figcaption></figure>

Feito isso, o pixel está instalado na página! Depois disso [**é preciso testá-lo**](broken-reference), pois a validação do mesmo é essencial para o funcionamento.

#### **Testando o pixel** <a href="#teste" id="teste"></a>

Existem 2 formas de testar se o pixel foi corretamente aplicado.\
A primeira é [dentro do próprio FB](broken-reference) e também agiliza na validação do pixel que veremos depois.\
O segundo jeito é através de uma [extensão do Google Chrome](broken-reference) e pode ser mais “na mão” se você tiver feito a instalação manual do código. Pois basta acessar o link da página/domínio e, pela extensão do próprio navegador, já consegue confirmar se o código está ou não inserido em seu domínio/página.

**Via Eventos de Teste**

**Nº15–** Volte ao Facebook e, na tela em que copiamos o código do pixel, clique em “Cancelar” para voltar à Visão Geral do Pixel.\
**Nº16–** Confirme o cancelamento da edição.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem11.png" alt=""><figcaption></figcaption></figure>

**Nº17–** Você será redirecionado para essa tela principal do pixel. Vá para a aba “Eventos de Teste”.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem8.png" alt=""><figcaption></figcaption></figure>

**Nº18–** Se fez a instalação em toda a máquina, insira seu domínio. Caso tenha feito em somente uma, insira o link da página na qual aplicou o código do Pixel.\
Agora, se feita em páginas específicas, cada uma precisará ser testada individualmente, inserindo e validando link por link.\
**Nº19–** Clique em “Abrir site”.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem12.png" alt=""><figcaption></figcaption></figure>

**Nº20–** Feito isso abrirá sua página em uma nova guia, basta aguardar que ela carregue totalmente e então fechá-la.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem13.png" alt=""><figcaption></figcaption></figure>

Após fechar a página, a tela do Gerenciador de Eventos ficará dessa forma caso tudo tenha dado certo.\
Isso significa que o Facebook localizou o Pixel e seu evento padrão “PageView” (visualização de página).

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem14.png" alt=""><figcaption></figcaption></figure>

**Via Extensão do Google Chrome**

**Instalando a extensão do Facebook**

Agora iremos instalar a extensão Facebook Pixel Helper. Se utilizá-la, poderá validar a configuração e terá um maior êxito.

**Nº15–** No navegador Google Chrome, acesse o hyperlink direto da extensão: [Facebook Pixel Helper](https://chrome.google.com/webstore/detail/facebook-pixel-helper/fdgfkebogiimcoedlicjlajpkdmockpc).\
**Nº16–** Clique em “Usar no Chrome”.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem15.png" alt=""><figcaption></figcaption></figure>

**Nº17–** Abrirá uma pop-up, nela selecione “Adicionar Extensão”.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem16.png" alt=""><figcaption></figcaption></figure>

Feito isso, a pop-up será atualizada e a extensão ficará da forma mostrada na imagem abaixo.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem17.png" alt=""><figcaption></figcaption></figure>

Ferramenta instalada com sucesso!

**Testando pela extensão**

**Nº18–** Acesse a página ou domínio configurado no navegador Google Chrome.\
**Nº19–** Abra a extensão, nela mostrará o ID do pixel e também o evento “PageView” que vem pré-configurado.

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem18.png" alt=""><figcaption></figcaption></figure>

#### **Validando o Pixel** <a href="#validacao" id="validacao"></a>

Quando o pixel for validado pelo Facebook, a tela inicial dele terá um gráfico semelhante a esse:

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem19.png" alt=""><figcaption></figcaption></figure>

Caso ainda não tenha recebido eventos ele estará dessa forma:

<figure><img src="https://legado.leadlovers.site/wp-content/uploads/2019/05/Imagem20.png" alt=""><figcaption></figcaption></figure>

**Importante:** O dashboard do Facebook pode levar até **24 horas** para atualizar. Então, caso você tenha seguido todos os passos desse tutorial e o gráfico ainda não esteja aparecendo, aguarde o período de um dia e consulte novamente a sua tela.

Caso não apareça o pixel configurado, revise os passos desse tutorial. Se ainda assim não funcionar, entre em contato com nosso time de suporte.

**Próximos passos**

E se você chegou até aqui e deseja também utilizar outros eventos em suas páginas, mostramos como fazer [nesse tutorial](https://suporte.love/pixel-fb-eventos/).

**Artigos recomendados**

– [O que é Pixel do FB](https://suporte.love/o-que-e-pixel-do-facebook/);

– [Como gerar o Pixel FB](https://suporte.love/gerando-pixel-fb/);

[– Instalando Eventos do Pixel FB;](https://suporte.love/pixel-fb-eventos/)

– [API de Conversões FB](https://suporte.love/api-conversao-facebook/);

– Como [inserir um script](https://suporte.love/inserir-script/) nas páginas da leadlovers.\
