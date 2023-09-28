# \[EDITORES ANTIGOS] Blocos e Modelos Prontos: Como colocar autoplay em um vídeo do Youtube ou Vimeo

Objetivo: Mostrar o passo a passo de como colocar o autoplay em um vídeo do Youtube ou Vimeo nos editores de páginas da leadlovers.\
Para que serve: O autoplay permite que assim que o lead entre na página, o vídeo seja executado automaticamente.

&#x20;**IMPORTANTE:**\


**–** Atualmente, o editor padrão de páginas é o **“Construtor por Componentes”**. Os editores **“Construtor por Blocos”** e **“Editor de Modelos Prontos”** foram descontinuados da plataforma, portanto estão disponíveis somente em **planos antigos**.

### &#x20;Colocando o autoplay no vídeo <a href="#colocando-autoplay" id="colocando-autoplay"></a>

Para ativar a função de autoplay em vídeos do Youtube, é preciso acrescentar a informação ?autoplay=1\&mute=1 no final do ID do link. No caso do Vimeo, o código a ser inserido é: ?autoplay=1\&muted=1.&#x20;

Abaixo vamos mostrar como fazer essa configuração.

&#x20;**ATENÇÃO:**\


– Para que o autoplay funcione no Google Chrome, é necessário que o vídeo inicie mutado de acordo com uma [atualização que foi feita no browser em 2018](https://developer.chrome.com/blog/autoplay/). É por isso que é necessário incluir um código para ativar o autoplay e mutar o vídeo ao mesmo tempo.\
– O código precisa ser aplicado no **iframe do vídeo**. Ao inserir somente no link, podem haver problemas em seu comportamento. Para que funcione corretamente, siga à risca os passos abaixo.

### Construtor por Blocos <a href="#blocos" id="blocos"></a>

Nº1– Dentro do editor, escolha a opção **“**Detalhes”.

Nº2– Clique em cima do vídeo.

Nº3– Abrirá uma janela do lado esquerdo, acesse a aba **“**vídeo”.

Nº4– No campo de edição, após o ID do seu vídeo do [Youtube](https://suporte.love/como-pegar-o-id-do-video-no-youtube/) ou [Vimeo](https://suporte.love/como-pegar-id-do-video-no-vimeo/), insira o código do autoplay. Confira qual é o correto dependendo do lugar em que o vídeo foi hospedado:

Youtube: ?autoplay=1\&mute=1\
Vimeo: ?autoplay=1\&muted=1

Observação: Esse código será acrescentado posteriormente ao iframe do vídeo dentro do código HTML do bloco.

Nº5– Clique em **“**Salvar Alterações”.

Nº6– Salve as edições da página.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/11/img03-3.png)](https://legado.leadlovers.site/wp-content/uploads/2021/11/img03-3.png)

### Editor de Modelos Prontos <a href="#modelos-prontos" id="modelos-prontos"></a>

No Editor de Modelos Prontos, para habilitar o autoplay é necessário ter escolhido um modelo que já tenha um vídeo, pois nesse editor somente é possível substituir os elementos já existentes na página, mas não adicionar novos.&#x20;

Nº1– Dentro da edição da página, encontre a aba em que está o campo de edição do vídeo. Verifique se no modelo escolhido ele foi inserido por iframe, pois caso seja somente o link não será possível aplicar o autoplay.

Nº2– No campo identificado, substitua a informação pelo iframe do seu vídeo (caso não saiba como encontrá-lo, consulte[ esse material](https://suporte.love/componentes-videos-iframe/)) e acrescente o código do autoplay. Confira qual é o correto dependendo do lugar em que o vídeo foi hospedado:

Youtube: ?autoplay=1\&mute=1\
Vimeo: ?autoplay=1\&muted=1

Em um vídeo do Youtube, ficaria similar a esse exemplo:&#x20;

\<iframe width=”560″ height=”315″ src=”https://www.youtube.com/embed/RCLbZgIJhJY?autoplay=1\&mute=1” title=”YouTube video player” frameborder=”0″ allow=”accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture” allowfullscreen>\</iframe>

Já em vídeos do Vimeo, pode ser gerado um código extra depois do seu ID no iframe. Nesse caso, identifique o ID (é o código numérico que vem depois da parte “video/”) e cole o código do autoplay logo após ele, como demonstramos abaixo:

\<iframe src=”https://player.vimeo.com/video/100365326?autoplay=1\&muted=1?h=297a62510e” width=”640″ height=”360″ frameborder=”0″ allow=”autoplay; fullscreen; picture-in-picture” allowfullscreen>\</iframe>

O ID é a série de números sublinhados depois de “video/”. Assim que o localizamos, logo após inserimos o código: ?autoplay=1\&muted=1 (em negrito no exemplo).

Nº3– Salve a página para aplicar essa configuração.&#x20;

[![](https://legado.leadlovers.site/wp-content/uploads/2021/11/img04-3.png)](https://legado.leadlovers.site/wp-content/uploads/2021/11/img04-3.png)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, entre em contato com o nosso suporte!

**Artigos relacionados**

– Como [encontrar o iframe](https://suporte.love/iframe/) de um vídeo;\
– Como inserir um vídeo por iframe no [Construtor por Componentes](https://suporte.love/componentes-videos-iframe/);\
– Como pegar o ID de um vídeo do [Youtube](https://suporte.love/como-pegar-o-id-do-video-no-youtube/) e do [Vimeo](https://suporte.love/como-pegar-id-do-video-no-vimeo/).

🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™
