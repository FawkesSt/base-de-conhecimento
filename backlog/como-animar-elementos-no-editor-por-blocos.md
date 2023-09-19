# Como animar elementos no editor por blocos

Objetivo: Ensinar como configurar animações nos elementos (botões, imagens, etc.) de uma página.\
Para quê serve: Permite que um elemento de sua página seja animado (apareça somente depois de um tempo, pulse ou pisque na tela, por exemplo) para chamar a atenção do visitante.\
Requisito obrigatório: 1. Ter uma página feita pelo Editor de Modelos Prontos ou Construtor por Blocos em sua máquina.&#x20;

&#x20;**IMPORTANTE:**\


**–** Atualmente, o editor padrão de páginas é o **“Construtor por Componentes”**. Os editores **“Construtor por Blocos”** e **“Editor de Modelos Prontos”** foram descontinuados da plataforma, portanto estão disponíveis somente em **planos antigos**.\
**–** Por enquanto, esta configuração não está disponível no **“Construtor por Componentes”**.\


### Editor de Modelos Prontos <a href="#modelos-prontos" id="modelos-prontos"></a>

As páginas construídas por esse editor já vem com os elementos e configurações pré-determinados, com a maioria deles sendo estáticos e não permitindo alterações. Caso prefira maior liberdade na construção de sua página, recomendamos que dê uma olhada nas animações que podem ser feitas pelo [Construtor por Blocos. ](broken-reference)

Para animar um elemento no Editor de Modelos Prontos, se certifique que o modelo escolhido já tenha essa configuração, em alguns ela está pré-configurada em botões. Por exemplo, na imagem abaixo, na opção **“**Tempo do Botão” é possível definir quantos segundos o mesmo levará para aparecer na página. Para que a animação funcione, basta definir os segundos que deseja e salvar as suas alterações.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/08/Tutorial-Animando-elementos-1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/08/Tutorial-Animando-elementos-1.png)

### Construtor por Blocos <a href="#blocos" id="blocos"></a>

Diferente do Editor de Modelos Prontos, o Construtor por Blocos tem mais configurações possíveis de serem feitas nos elementos. O melhor de tudo é que elas estão disponíveis no editor, ou seja, você consegue aplicá-las em qualquer um dos blocos. No nosso exemplo, faremos a animação em um botão de Call to Action.

Nº1– No canto superior esquerdo, há três opções: **“**Blocos”, **“**Conteúdo” e **“**Detalhes”. Selecione **“**Detalhes”.

Nº2– Clique no item da página em que deseja aplicar a configuração. No nosso exemplo, utilizamos um botão.&#x20;

[![](https://legado.leadlovers.site/wp-content/uploads/2020/08/Tutorial-Animando-elementos-2.png)](https://legado.leadlovers.site/wp-content/uploads/2020/08/Tutorial-Animando-elementos-2.png)

Nº3– No menu que surgir do lado esquerdo da tela, clique na aba **“**Style”. É nela que a animação vai ser criada. No exemplo deste tutorial, nós vamos configurar para que o botão apareça na página depois de um determinado tempo.&#x20;

Nº4– Animation: aqui escolha qual tipo de animação seu elemento vai ter. Dentre todas as opções, escolha alguma animação e veja o efeito que mais te atrai. No nosso caso, seguindo o exemplo, vamos fazer com que o botão comece invisível e apareça depois. Para isso, utilizaremos a animação **“FadeIn”**, que fará com que o elemento apareça aos poucos.

Nº5– Data-wow-duration: nessa opção, determine quanto tempo em segundos a animação vai durar. Então, quanto maior o número aqui, mais lenta e longa ela será. Se você utilizar, por exemplo, a opção que faz com que o elemento pisque na tela, é aqui que deve determinar por quanto tempo ele ficará piscando.

Nº6– Data-wow-delay: nesse campo, configure quanto tempo vai levar até que a animação se inicie. Ou seja, depois de quantos segundos o botão deve aparecer na tela com o efeito que foi definido.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/08/Tutorial-Animando-elementos-3.png)](https://legado.leadlovers.site/wp-content/uploads/2020/08/Tutorial-Animando-elementos-3.png)

Observação: só é possível determinar os tempos (**“**data-wow-duration” e **“**data-wow-delay”) após escolher um efeito no campo **“**animation”. Caso ele esteja configurado como **“**none” (nenhum efeito), essas opções estarão desativadas para edição.

No gif a seguir, mostramos na prática como fica um botão com a animação **“**FadeIn”, em que o **“**data-wow-delay” foi configurado para 5s (cinco segundos) e o **“**data-wow-duration” para 2s (dois segundos):

[![](https://legado.leadlovers.site/wp-content/uploads/2020/08/ani-re.gif)](https://legado.leadlovers.site/wp-content/uploads/2020/08/ani-re.gif)

### Existe um limite de tempo para as animações? <a href="#tempo-limite" id="tempo-limite"></a>

Não existe, mas você precisa colocar esse tempo em segundos para ela funcionar.

Por exemplo: caso deseje que uma animação dure 1 minuto, basta incluir 60s (sessenta segundos) na opção **“**data-wow-duration”.

### Sincronizando um botão a um vídeo <a href="#sincronizando-botao" id="sincronizando-botao"></a>

Primeiro, verifique em que momento de seu vídeo deseja que o botão apareça.

Vamos considerar, por exemplo, que quero que o botão surja em 1:35 do meu vídeo. Para configurar o tempo que o botão aparecerá, eu precisarei converter esse tempo em segundos. Como 1:35 são 95 segundos, vou colocar 95s na opção **“**data-wow-delay”. Assim que o lead entrar na minha página, o vídeo irá reproduzir e o botão aparecerá 95 segundos depois.

**Observações:**

– O vídeo e o botão são elementos distintos na página e não ficarão interligados. Se o lead não assistir ao vídeo, o botão vai aguardar os 95 segundos e aparecer da mesma forma.

– A contagem dos segundos só começa quando o lead “visualiza” o bloco em que o elemento está. Vamos supor que você defina alguma animação em um botão que está um dos últimos blocos, enquanto o lead não rolar a página para baixo e “ver” o bloco, os segundos não começarão a contar.

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, **entre em contato com o nosso suporte**!

**Artigos Relacionados**

**–** Como criar uma [página de captura](https://suporte.love/como-criar-e-configurar-uma-pagina-de-captura-no-editor-por-componentes/)?\
**–** Como criar e configurar uma [página de recompensa](https://suporte.love/como-criar-e-configurar-uma-pagina-de-recompensa-no-editor-por-componentes/)?





🏁 **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
