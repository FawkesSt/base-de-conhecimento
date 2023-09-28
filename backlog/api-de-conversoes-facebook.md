# API de Conversões Facebook

**Objetivo:** ensinar como conectar a leadlovers com a API de Conversões do Facebook.\
**Para que serve:** rastrear efetivamente eventos/pixel do Facebook em casos onde o lead está usando iOS 14 com o bloqueio de rastreio na web ou qualquer outro dispositivo com bloqueador de anúncios.\
**Requisito(s) necessário(s):** **1.** ter o pixel e seus eventos [já instalados](https://suporte.love/pixel-fb-eventos/) e **2.** ter instalado [_manualmente_ os eventos](https://suporte.love/pixel-fb-eventos/) via código nas páginas (e não com a ferramenta de Configuração de Eventos).

#### **Configuração no Facebook** <a href="#facebook" id="facebook"></a>

**Nº1–** Acesse o link do [Gerenciador de Eventos](https://business.facebook.com/events\_manager2) ou clique no atalho no seu perfil pessoal do Facebook.

**Nº2–** Selecione o pixel que já está [configurado e metrificando](https://suporte.love/instalar-pixel-fb/) suas páginas da leadlovers.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem1.png)

**Nº3–** Vá até a aba “Configurações”.

**Nº4–** Role a tela até encontrar “API de Conversões” e clique no botão “Começar”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem2.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem2.png)

**Nº5–** Serão mostradas informações sobre a configuração, é importante lê-las, então avance.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem3.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem3.png)

**Nº6–** Leia as informações e prossiga.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem4.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem4.png)

**Nº7–** Agora serão mostradas as últimas instruções, atente-se a elas. Clique em “Configurar” para prosseguir.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem5.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem5.png)

**Nº8–** Aqui será mostrado um breve resumo de como é feita a configuração, proceda.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem6.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem6.png)

**Nº9–** Selecione os eventos que deseja que sejam enviados pela API de conversões, o ideal é utilizar todos que configurou previamente no pixel.

**Nº10–** Clique em “Continuar”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem7.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem7.png)

**Nº11–** Clique sobre o evento.

**Nº12–** Ative a opção “Identificação do evento”, essencial para o bom funcionamento da configuração, pois com ela os eventos identificados pelo pixel (navegador) e API (servidor) não serão **duplicados** para um usuário que permita ambas as identificações.

**Nº13–** As demais opções da seção “Parâmetros de detalhes do evento” são opcionais.

**Nº14–** Escolha ao menos um dos “Parâmetros de informações do cliente”. Resumidamente, esses dados do usuário são enviados para o Facebook por cada um dos eventos, permitindo que a plataforma entenda melhor o seu público e direcione seus anúncios às pessoas certas. A escolha aqui dependerá de sua estratégia e negócio.

**Nº15–** Repita os passos 11 ao 14 para cada evento que será metrificado.

**Nº16–** Clique em “Continuar”, isso te levará para uma tela de revisão das configurações feitas.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem8.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem8.png)

**Nº17–** Analise se cada evento está com a configuração da forma desejada, o ponto mais importante aqui é verificar se todos possuem a “Identificação do evento” (destacado na imagem abaixo).

**Nº18–** Se estiver tudo certo, confirme a configuração.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem9.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem9.png)

**Nº19–** Conclua-a para iniciarmos a implementação!

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem10.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem10.png)

#### **Implementação** <a href="#configuracao" id="configuracao"></a>

Após configurar quais eventos serão metrificados e suas especificidades, iremos pegar algumas informações no Facebook, inseri-las na leadlovers e então validá-las.

#### **Dados do Facebook** <a href="#pegando-dados" id="pegando-dados"></a>

No Facebook iremos coletar dois dados, que são: o token de acesso e o código de teste de eventos. É bacana manter o Bloco de Notas, ou semelhante, aberto para facilitar a configuração.

**Token de Acesso**

**Nº20–** Vá até a aba “Configurações” no pixel que está sendo configurado.

**Nº21–** Na seção “API de Conversões” clique em “Gerar token de acesso”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem11.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem11.png)

**Nº22–** Quando o token for gerado,clique sobre o campo onde ele está para copiá-lo. Então guarde-o em um local seguro. Essa é uma boa hora para usar o Bloco de Notas!

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem12.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem12.png)

**Código de teste de eventos**

Agora iremos copiar o segundo código necessário para realizar a implementação da API de conversões.

**Nº23–** Acesse a aba “Eventos de teste”.

**Nº24–** _**SE**_ já houver feito teste de eventos anteriormente, clique em “Limpar atividade”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem13.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem13.png)

**Nº25–** Clique sobre o campo onde é mostrado o código de teste do evento,. Ele será copiado para a área de transferência de seu dispositivo, armazene-o em um local seguro, assim como fez com o Token de Acesso.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem14.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem14.png)

#### **Inserindo os dados na leadlovers** <a href="#leadlovers" id="leadlovers"></a>

Agora iremos inserir os dados nas configurações de sua máquina leadlovers.

**Nº26–** Acesse a máquina onde estão as páginas metrificadas pelo pixel e vá até a aba “Configurações”.

**Nº27–** Em seguida, no menu lateral esquerdo, acesse a opção “Api de Conversões Facebook”.

**Nº28–** Escolha o pixel pelo ID do mesmo, então clique sobre ele.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem15.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem15.png)

**Nº29–** Marque a opção “Habilitar API de Conversão”.

**Nº30–** Cole aqui o token de acesso, que foi copiado no [passo 22](broken-reference).

**Nº31–** Ative “Habilitar evento de teste”.

**Nº32–** Cole aqui o código de teste do evento, copiado no [passo 25](broken-reference).

**Nº33–** Salve as configurações.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem16.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem16.png)

Os dados inseridos ficarão salvos. A configuração está concluída, agora basta validá-la.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem17.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem17.png)

#### **Validando a configuração** <a href="#validacao" id="validacao"></a>

É sempre muito importante validar todos os pontos da sua estratégia para se certificar de que está tudo funcionando corretamente e como desejado.

**Nº34–** Acesse uma das páginas que está sendo metrificada pelo pixel.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem18.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem18.png)

**Nº35–** Volte ao gerenciador de eventos do Facebook, ainda na aba “Eventos de Teste”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem19.png)](https://legado.leadlovers.site/wp-content/uploads/2021/06/Imagem19.png)

Esse é o resultado esperado! Visto que o evento foi identificado pelo navegador (pixel) e pelo servidor (API) e também foi desduplicado, ou seja, cada acesso único contabilizará somente um evento por ação.

**Importante:** O Facebook pode levar no _mínimo_ 20 minutos para exibir os eventos.

Caso não apareça o evento recebido pelo servidor, revise os passos desse tutorial e, se ainda assim não funcionar, entre em contato com nosso time de suporte.

**Pós validação**

Após ter validado o funcionamento da API de conversões é muito **importante **_**desativar**_** o evento de teste** (habilitado no [passo 30](broken-reference)) e salvar a edição. Isso porque, caso este permaneça ativo, todos os eventos serão contabilizados como teste e suas métricas da API de conversões não serão concretas.

**Artigos recomendados**

– [O que é Pixel do FB](https://suporte.love/o-que-e-pixel-do-facebook/);

– [Como gerar o Pixel FB](https://suporte.love/gerando-pixel-fb/);

– [Como instalar o Pixel FB](https://suporte.love/instalar-pixel-fb/);

– [Instalando Eventos do Pixel FB;](https://suporte.love/pixel-fb-eventos/)

– [API de Conversões FB](broken-reference);

– Como [inserir um script](https://suporte.love/inserir-script/) nas páginas da leadlovers.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
