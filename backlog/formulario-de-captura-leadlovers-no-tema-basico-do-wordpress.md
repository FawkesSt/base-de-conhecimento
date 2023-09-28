# Formulário de Captura leadlovers no tema básico do WordPress

Se você caiu aqui aleatoriamente e não conhece o [**WordPress**](https://br.wordpress.com/) e nem sabe como o mesmo pode ser integrado ao leadlovers, confere primeiro este artigo: [**Integração leadlovers com WordPress**](https://legado.leadlovers.site/integracao-leadlovers-com-wordpress/).

**Objetivo**: Mostrar como integrar a leadlovers com o tema básico do WordPress, caso o usuário opte por criar as páginas nessa outra plataforma.\
**Para quê serve:** Ao criar um formulário na Aba Formulários de Captura, na leadlovers, irá gerar o formulário em código HTML. É possível inserir esse código HTML dentro das páginas criadas através do WordPress, assim, todas as pessoas que se cadastrarem nesse formulário serão capturadas como leads na sua máquina, funil e sequência.\
**Requisito(s) obrigatório(s): 1.** Ter acesso ao [**WordPress;**](https://wordpress.org/) e **2.** ter um **Formulário de Captura** ([estático](https://suporte.love/criar-formulario-estatico/) ou [dinâmico](https://suporte.love/como-criar-campos-dinamicos-e-como-criar-formulario-dinamico/)) criado aqui na **leadlovers**.

**ATENÇÃO**:\
A **ausência e/ou inserção incorreta** dos respectivos códigos nos campos descritos neste tutorial, **resultará em mal funcionamento do formulário!**\
**TODOS os códigos devem ser inseridos!**

### **Quais são os códigos do formulário estático de captura?**

Os formulários (Estático Padrão e Dinâmico) possuem três códigos:  CSS – código do formulário – JS . Conforme ilustração abaixo, respectivamente, são esses: primeiro, segundo e terceiro código.\
Códigos esses que devem ser inseridos cada um em seu devido campo dentro de sua página criada através do **WordPress**.

**Observação:** O formulário Estático Simples possui apenas 2 códigos: o CSS (configuração de layout) + o Código do Formulário. Mas, ambos podem ser inseridos juntos direto no corpo da página.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/atencao1.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/atencao1.png)**IMPORTANTE:**\
– Caso esteja utilizando o formulário estático do tipo Simples (sem script) faça apenas a parte de [_**Inserindo o código**_](broken-reference).\
– Agora, se estiver usando o formulário estático do tipo Padrão (com script) ou o formulário Dinâmico realize também os passos da parte [_**Inserindo scripts HEAD e BODY**_](broken-reference).

Você pode conferir as diferenças entre os formulários nesse artigo [**aqui**](https://suporte.love/criar-formulario-estatico/).

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/formulrios-de-captura-teste-2-leadlove.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/formulrios-de-captura-teste-2-leadlove.png)

### **Inserindo o código do formulário na página**

**Nº1–** Dentro da edição da página, clique no ícone de ➕ para **adicionar um novo Bloco**.

**Nº2–** Acesse a categoria **Formatação** e selecione a opção **< > Código**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/unnamed-file.wp.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/unnamed-file.wp.png)

**Nº3–** No novo bloco, cole o Código do Formulário (segundo código).

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/wp1.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/wp1.png)

**Observação:** Se você utiliza o formulário do tipo Estático Simples (sem script) o código CSS, o primeiro código, que ele possui pode ser inserido também direto no corpo da página junto ao corpo do formulário.\
É muito importante que a aplicação seja na ordem dos códigos: CSS primeiro e depois o restante.\
Abaixo eu mostro um exemplo dos 2 códigos inseridos juntos:

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/form-simples-1.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/form-simples-1.png)

A linha destacada em verde é o código CSS e a parte destacada em vermelho o código do formulário.

**Nº4–** Lembre de **salvar** sua página.

### **Inserindo scripts HEAD e BODY na página**

Agora, se você está utilizando o formulário estático Padrão (com script) ou o formulário Dinâmico é preciso inserir os campos de CSS e JS em um local próprio para aplicação de códigos adicionais.\
Nesse tutorial vamos mostrar como fazer isso pelo plugin **Insert Headers and Footers** e nesse [artigo aqui](https://suporte.love/wordpress-plugin-scripts/) nós ensinamos como você pode instalar esse plugin em seu WordPress.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/wp2.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/wp2.png)

**Nº5–** Depois de Ativar o plugin, uma nova opção aparecerá na parte de **Configurações**, clique nela.

**Nº6–** Após clicar no item, você encontrará três campos. Aplique o primeiro código (CSS) na parte de **Scripts in Header**.

**Nº7–** Em Script in Body cole o terceiro código (JS).

**Nº8–** Após colar os scripts, basta clicar em “**Save**”.

E prontinho! O seu formulário de captura leadlovers foi inserido corretamente em sua página.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
