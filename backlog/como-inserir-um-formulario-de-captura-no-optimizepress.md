# Como inserir um formulário de Captura no Optimizepress

Se você caiu aqui aleatoriamente e não conhece o [**WordPress**](https://br.wordpress.com/) e nem sabe como o mesmo pode ser integrado ao leadlovers, confere primeiro este artigo: [**Integração leadlovers com WordPress**](https://legado.leadlovers.site/integracao-leadlovers-com-wordpress/).

**Objetivo**: Mostrar como integrar a leadlovers com o plugin Optimizepress, caso o usuário opte por criar as páginas na plataforma **WordPress**.\
**Para quê serve:** Ao criar um formulário na Aba Formulários de Captura, na leadlovers, irá gerar o formulário em código HTML. É possível inserir esse código HTML dentro das páginas criadas através do plugin Optimizepress, assim, todas as pessoas que se cadastrarem nesse formulário serão capturadas como leads na sua máquina, funil e sequência.\
**Requisito(s) obrigatório(s): 1.** É necessário ter o [**Optimizepress**](https://www.optimizepress.com/?fpr=fernando63) instalado em seu [**WordPress**](https://wordpress.org/) e **2.** ter um **Formulário de Captura** ([estático](https://suporte.love/criar-formulario-estatico/) ou [dinâmico](https://suporte.love/como-criar-campos-dinamicos-e-como-criar-formulario-dinamico/)) aqui na leadlovers.

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

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/optm1.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/optm1.png)

**1 –** Após logar no **WordPress**, Acesse aba **páginas** > **todas as páginas**.

**2 –** Encontre a página em que o formulário está inserido e clique em “**Live Editor**”

Após abrir a edição da página, clique duas vezes em cima do formulário inserido nela.\
Será evidenciado um pop-up de configurações.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/cdigo2.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/cdigo2.png)

**3 –** Neste popup, na aba “**Form HTML**“, insira o **código do formulário** criado na leadlovers (**o segundo código**).

Salve.

**Observação:** Se você utiliza o formulário do tipo Estático Simples (sem script) o código CSS, o primeiro código, que ele possui pode ser inserido também direto no corpo da página junto ao corpo do formulário.\
É muito importante que a aplicação seja na ordem dos códigos: CSS primeiro e depois o restante.

### **Inserindo script HEAD e BODY na página.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/save3.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/save3.png)

**4 –** Ao retornar para a tela na página, clique no **ícone de engrenagem** do formulário.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/script1.png)](http://legado.leadlovers.site/wp-content/uploads/2020/09/script1.png)

**5 –** Aparecerá outro popup de configurações.\
No campo **Code before Element**, insira o **primeiro código do formulário**, chamado de “**Arquivo CSS**“.

**6 –** No campo **Code after Element**, insira o **terceiro código do formulário**, chamado de “**Arquivos JS**“.

**7-** Salve.

**OBSERVAÇÃO:** É preciso _testar_ se o formulário estático do tipo Padrão (com script) ou o formulário Dinâmico funcionará nos pop-ups nativos do plugin Optimizepress.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
