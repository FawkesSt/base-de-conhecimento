# 99Webinar: Como usar o Streaming nativo?

**Objetivo:** ensinar a configurar e usar a função de Streaming Nativo disponível na criação de um webinar.\
**Para que serve:** você pode fazer sua transmissão, sem a necessidade de usar o Youtube, Vimeo ou outra plataforma externa. Será possível, através do uso de um _encoder_, usar o serviço de Streaming próprio da nossa ferramenta.\
**Requisito(s) obrigatório(s):** Ter o OBS Studio ou algum outro tipo de encoder já instalado em seu computador.

### **Instalando o OBS Studio**

O primeiro passo é obter o encoder que será usado. [**Clique aqui e faça o download do OBS Studio**](https://obsproject.com/pt-br/download).

**⚠ IMPORTANTE:** certifique-se de escolher a versão correta para o sistema operacional usado pelo seu computador.

Após o download, faça a instalação e abra o OBS Studio. Você já será direcionado para a tela principal.

![](https://legado.leadlovers.site/wp-content/uploads/2020/10/99Webinar\_-Como-usar-o-Streaming-nativo-\_-360025592553\_99w-streaming-nativo-1.png)

### **Configurando as opções de Saída e Vídeo**

**1 –** No canto inferior esquerdo da tela principal do OBS Studio, procure o quadro chamado Controles. Dentre as opções disponíveis, clique em “Configurações”.

![](https://legado.leadlovers.site/wp-content/uploads/2020/10/99Webinar\_-Como-usar-o-Streaming-nativo-\_-360025592553\_99w-streaming-nativo-2.png)

**2 –** Na próxima tela, clique na opção **Saída**, listada no lado esquerdo.\
Os itens desta opção vão aparecer do lado direito. Configure-os da seguinte forma:

**3 –** Em **Modo de Saída**, escolha a opção **Simples**.

**4 –** Em **Taxa de Bits do Vídeo**, selecione **2500 Kbps**.

**5 –** Em **Encoder**, escolha a opção **Software (x264)**.

**6 –** Em **Taxa de Bits do Áudio**, escolha **160**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/10/99Webinar\_-Como-usar-o-Streaming-nativo-\_-360025592553\_99w-streaming-nativo-3.png)

Verifique as informações inseridas, **mas não feche esta tela**. Vamos para a próxima etapa!

**7 –** Clique na opção **Vídeo**, listada também no lado esquerdo.\
Novamente, os itens estarão do lado direito. Configure-os da seguinte forma:

**8 –** No item **Resolução de Saída** **(escala)**, selecione **852×480**.

**9 –** Em **Filtro de Resolução**, escolha **Bicúbico (escalamento nítido, 16 amostras)**.

**10 –** Em **Valor de FPS Comum**, escolha a opção **30**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/10/99Webinar\_-Como-usar-o-Streaming-nativo-\_-360025592553\_99w-streaming-nativo-4.png)

**11 –** Verifique as informações inseridas. Depois, no canto inferior direito da tela, clique no botão **Aplicar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/10/99Webinar\_-Como-usar-o-Streaming-nativo-\_-360025592553\_99w-streaming-nativo-9.png)

Mantenha esta janela de **Configurações** aberta e abra o 99Webinar em seu navegador!\
O próximo passo, agora, é criar o webinar.

### **Criando e configurando o webinar**

[**Clique aqui e siga os passos deste material**](https://suporte.love/criacao-webinar/), para dar início a criação do seu webinar.\
Você será direcionado para a tela de **Configurações Gerais** dele.

**12 –** Ative a opção **Utilizar streaming nativo**. Depois, faça as demais configurações que deseja para seu Webinar.

**13 –** Verifique todas as configurações feitas, e clique no botão **Criar**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/10/99Webinar\_-Como-usar-o-Streaming-nativo-\_-360025592553\_99w-streaming-nativo-5.png)

Logo após a criação, você será direcionado para o **Gerenciamento do Webinar**. No lado direito desta tela, na seção de **Controles do Webinar**, você verá as opções, similares à da imagem acima.

**14 –** Clique neste botão para copiar a **URL para o Encoder**. Salve esta URL, pois usaremos ela em breve (pode usar um Bloco de Notas, para ficar mais prático).

**15 –** Agora, clique neste botão para copiar a **StreamKey o Encoder**. Novamente, salve a StreamKey, para usarmos nos próximos passos (pode usar o Bloco de Notas, como sempre). Este campo “esconde” a chave, quando inserimos ela. Se quiser ver o que foi colocado (para ter certeza), clique no botão **Exibir**, que fica na frente deste campo.

![](https://legado.leadlovers.site/wp-content/uploads/2020/10/99Webinar\_-Como-usar-o-Streaming-nativo-\_-360025592553\_99w-streaming-nativo-6.png)

### **Inserido os dados de transmissão no OBS Studio**

**16 –** Retorne para tela de **Configurações** do **OBS Studio** (a que deixamos aberta lá no fim do passo **10**). Clique na opção **Transmissão**, listada no lado esquerdo.\
Novamente, vamos incluir os dados nos campos da direita.

**17 –** Em **Serviço**, escolha **Personalizado…**

**18 –** Em **Servidor**, coloque o link copiado no passo **14** (a **URL para Transmissão pelo Encoder**).

**19 –** Em **Chave de transmissão**, coloque o código copiado no passo **15** (a a **StreamKey para Transmissão pelo Encoder**).

![](https://legado.leadlovers.site/wp-content/uploads/2020/10/99Webinar\_-Como-usar-o-Streaming-nativo-\_-360025592553\_99w-streaming-nativo-10.png)

**20 –** Verifique as informações inseridas. Depois, no canto inferior direito da tela, clique no botão **Aplicar**, e depois em **OK**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/10/99Webinar\_-Como-usar-o-Streaming-nativo-\_-360025592553\_99w-streaming-nativo-9-2.png)

Agora, você está de volta à tela principal do OBS, e tudo está pronto para seu webinar. Vamos iniciar a transmissão!

### **Iniciando a transmissão**

**21 –** Na tela principal do OBS Studio, localize novamente o quadro **Controles**. Clique na opção **Iniciar transmissão**.

![](https://legado.leadlovers.site/wp-content/uploads/2020/10/99Webinar\_-Como-usar-o-Streaming-nativo-\_-360025592553\_99w-streaming-nativo-2-2.png)

A opção, agora, se transformou em **Interromper transmissão**. Algumas outras informações ficam disponíveis, para você, durante sua transmissão:

**A –** Aqui, você vê o tempo total de transmissão.\
**B –** O quadro na cor verde indica que sua transmissão está em andamento. Caso ele mude para a cor vermelha, significa que há problemas na transmissão. Em **kb/s**, fica visível a taxa de transmissão de dados, em kilobytes por segundo. Quanto maior a taxa de transmissão, melhor.

![](https://legado.leadlovers.site/wp-content/uploads/2020/10/99Webinar\_-Como-usar-o-Streaming-nativo-\_-360025592553\_99w-streaming-nativo-8.png)

#### **INFORMAÇÕES IMPORTANTES:**

**–** Iniciar a transmissão no OBS Studio não inicia seu Webinar! Ele começa a ser exibido no 99Webinar na data e hora que você configurou na criação do Webinar.

**–** É bom iniciar a transmissão no OBS, pelo menos, 10 segundos antes do início do Webinar. Isso dá tempo para que exista algo “pré-carregado”, e assim evita que os espectadores acessem seu link e vejam algum erro de exibição de vídeo.

**–** Da mesma forma, também é bom dar alguns segundos (entre 10 e 20) entre a finalização do Webinar e apertar o botão **Interromper Transmissão** no OBS.

**–** Caso você ainda não tenha usado o OBS Studio, o produtor da ferramenta mantém documentação com as principais instruções de uso:

[**OBS Studio Quickstart**](https://obsproject.com/wiki/OBS-Studio-Quickstart)

[**OBS Studio Overview**](https://obsproject.com/wiki/OBS-Studio-Overview)\


**🏁 É isso, terminamos por aqui!**\
com amor ❤\
equipe **99Webinar™**
