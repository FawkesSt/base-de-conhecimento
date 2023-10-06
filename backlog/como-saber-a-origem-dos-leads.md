# Como saber a origem dos leads?

Objetivo: Ensinar como inserir um parâmetro SRC nos leads.\
Para que serve: Ao aplicar esse parâmetro, é possível saber a origem do lead e organizar melhor a sua estratégia.\
Requisitos obrigatórios: 1. Ter uma página ou um formulário de captura criado na leadlovers.

### O que é? <a href="#o-que-e" id="o-que-e"></a>

Se deseja saber a origem dos seus leads e organizar melhor a sua estratégia, pode aplicar neles um parâmetro SRC.&#x20;

Para isso, basta inserir um código **na URL** que será compartilhada e, quando divulgá-la em diferentes mídias (por exemplo, no seu Facebook ou nas descrições de seus vídeos no Youtube), todos os leads que se capturarem pelos links que contém esse código receberão um parâmetro SRC. Essa informação será inserida nos seus detalhes aqui na leadlovers para consulta posterior.&#x20;

Neste tutorial, te ensinaremos como inserir, consultar e testar os parâmetros em poucos passos.

### Como inserir em uma página de captura <a href="#pagina-captura" id="pagina-captura"></a>

Nº1– Se criou o seu formulário direto na sua página de captura, acesse a aba **“Páginas”** na sua máquina e clique sobre aquela que deseja aplicar o parâmetro.

[![](https://legado.leadlovers.site/wp-content/uploads/2016/01/img01-1.png)](https://legado.leadlovers.site/wp-content/uploads/2016/01/img01-1.png)

Nº2– No final de sua URL, insira o código SRC:

_?src=origemdolead_

Substitua a informação origemdolead com o lugar que o lead veio. Por exemplo, para divulgar o link no Facebook você pode inserir:&#x20;

_seudominio.com.br/nomedapagina**?src=facebook**_

[![](https://legado.leadlovers.site/wp-content/uploads/2016/01/img02.png)](https://legado.leadlovers.site/wp-content/uploads/2016/01/img02.png)

Caso queira acrescentar mais de um parâmetro na URL, é necessário adicionar ele depois do primeiro e com a seguinte estrutura:

_\&src=outroparametro_

Seguindo a mesma lógica do exemplo anterior, a divulgação pode ser feita de diferentes maneiras no mesmo lugar. Por exemplo, dentro do próprio Facebook é possível postar o link em uma fanpage e em um grupo.

Para diferenciar os dois locais, você pode acrescentar mais um parâmetro diferente em cada link:

_seudominio.com.br/nomedapagina?src=facebook\&src=grupo_

_seudominio.com.br/nomedapagina?src=facebook\&src=fanpage_

Certifique-se de apertar a tecla “Enter” logo após inserir o parâmetro para que ele seja corretamente incorporado ao link e você possa [testar mais tarde.](broken-reference)&#x20;

### Como inserir em um Formulário de Captura <a href="#formulario-captura" id="formulario-captura"></a>

#### Estático Simples (Sem script)  <a href="#formulario-simples" id="formulario-simples"></a>

Se inserir um formulário do tipo [Estático Simples (Sem script)](https://suporte.love/criar-formulario-estatico/) na sua página, ao aplicar o parâmetro SRC direto na URL dela ele não será adicionado ao lead. Para isso, é necessário acrescentá-lo a uma linha do código HTML. &#x20;

Portanto, quando estiver colocando o formulário na página, localize a linha _**\<input type=“hidden” id=“source” name=“source” value=“” />**_ e insira o parâmetro que desejar dentro das aspas que ficam depois de _**value=“”**_. Por exemplo:

_\<input type=“hidden” id=“source” name=“source” value=“origemdolead” />_

[![](https://legado.leadlovers.site/wp-content/uploads/2016/01/img03-1.png)](https://legado.leadlovers.site/wp-content/uploads/2016/01/img03-1.png)

Se quiser inserir mais parâmetros, basta copiar essa linha do código e inserir uma nova igual logo abaixo, alterando o _**value=“”**_.

**⚠ ATENÇÃO:**\


– Quando o parâmetro é inserido dessa forma, somente é possível consultar esse dado [exportando os leads](https://suporte.love/como-exportar-leads-2/) e marcando a opção “Listar Parâmetros SRC” no momento de gerar o arquivo. Ele virá em uma coluna com o nome “SRC”.

– É importante ressaltar que esse parâmetro é fixo, ou seja, ele não funciona exatamente como o que é inserido diretamente na URL, pois não pode ser alterado dependendo do lugar em que o link estiver sendo divulgado. Você pode sim modificar pelo código quando quiser, mas, enquanto o parâmetro estiver no formulário da página, esse dado será adicionado a todos os leads que se capturarem por ela. Isto é, sempre que fizer uma alteração no parâmetro, todos os novos leads capturados ganharão o SRC mais recente.&#x20;

**Dica:** Se inserir o parâmetro direto no código do formulário e quiser divulgar em diferentes lugares, você pode criar uma página para cada plataforma em que deseja promover e inserir o mesmo formulário em cada uma delas, alterando apenas o campo _**value=“”**_ do seu código.&#x20;

#### Estático Padrão (Com script) e Dinâmico <a href="#formulario-padrao-dinamico" id="formulario-padrao-dinamico"></a>

Caso esteja utilizando um formulário do tipo [Estático Padrão (Com Script)](https://suporte.love/criar-formulario-estatico/) ou [Dinâmico](https://suporte.love/como-criar-campos-dinamicos-e-como-criar-formulario-dinamico/), basta adicioná-lo à sua página inserindo corretamente os três códigos gerados e então aplicar o parâmetro na URL da página como ensinamos anteriormente no [passo 02](broken-reference).

Se algum dos três códigos gerados não for inserido na página (especialmente o **“Código do Formulário”** e os **“Arquivos JS”**), a aplicação do parâmetro pode não ocorrer corretamente, além do funcionamento do próprio formulário ser afetado.

Observação: o parâmetro SRC inserido na URL só irá funcionar nas páginas externas que o nosso formulário seja inserido via código. Por enquanto, não é possível aplicar parâmetros em integrações diretas.

### Consultando os parâmetros do lead <a href="#consultando-parametros" id="consultando-parametros"></a>

Nº3– Dentro da máquina em que está a página ou formulário de captura, vá até a aba “Leads”.

Nº4– Clique sobre aquele que deseja conferir a origem.

Observação: em um primeiro momento, o parâmetro SRC aparecerá em “Origem” na listagem de leads. No entanto, essa informação que fica disponível nesta tela não é fixa e sempre é alterada de acordo com a movimentação mais recente. A melhor maneira de verificar é consultando a aba “Parâmetros” como ensinaremos a seguir.

[![](https://legado.leadlovers.site/wp-content/uploads/2016/01/img04-1.png)](https://legado.leadlovers.site/wp-content/uploads/2016/01/img04-1.png)

Nº5– Vá até a aba “Parâmetros”.

Nº6– O parâmetro aplicado aparecerá com a informação “src” em cima. Se houver mais de um, todos eles serão listados nesse mesmo local.

[![](https://legado.leadlovers.site/wp-content/uploads/2016/01/img05-1.png)](https://legado.leadlovers.site/wp-content/uploads/2016/01/img05-1.png)

### Testando a aplicação os parâmetros <a href="#testando" id="testando"></a>

A única forma de testar a aplicação correta dos parâmetros SRC é simulando uma captura real. Para isso, siga as seguintes orientações:

– Acesse a página com o parâmetro SRC já aplicado na URL ou no código HTML do formulário.

– Faça um teste de captura. Consulte [este material](https://suporte.love/testar-captura/) para mais informações sobre como fazer esse procedimento.

– Aguarde de 5 a 30 minutos enquanto o sistema processa a informação e então consulte os detalhes do lead como ensinamos no [tópico anterior](broken-reference) ou exporte um arquivo caso tenha inserido direto pelo [código HTML.](broken-reference)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, entre em contato com o nosso suporte!

**Artigos relacionados**

– Como fazer um [teste de captura](https://suporte.love/testar-captura/)?\
– Como criar um [Formulário Estático](https://suporte.love/criar-formulario-estatico/) ou [Dinâmico](https://suporte.love/como-criar-campos-dinamicos-e-como-criar-formulario-dinamico/) de captura?\
– Índice de [como criar e aplicar tags](https://suporte.love/como-criar-uma-tag/) aos leads.

🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™
