# Integração com Elementor Free

Se você caiu aqui aleatoriamente e não conhece o [**WordPress**](https://br.wordpress.com/) e nem sabe como o mesmo pode ser integrado ao leadlovers, confere primeiro este artigo: [**Integração leadlovers com WordPress**](https://legado.leadlovers.site/integracao-leadlovers-com-wordpress/).

**Objetivo**: Explicar como integrar a leadlovers com o plugin Elementor, caso o usuário opte por criar as páginas na plataforma **WordPress**.\
**Para que serve:** Ao criar um formulário na Aba Formulários de Captura, na leadlovers, irá gerar o formulário em código HTML. É possível inserir esse código HTML dentro das páginas criadas através do plugin Elementor, assim, todas as pessoas que se cadastrarem nesse formulário serão capturadas como leads na sua máquina, funil e sequência.\
**Requisito(s) obrigatório(s): 1.** Ter o plugin [**Elementor**](https://br.wordpress.org/plugins/elementor/) instalado em seu [**WordPress;**](https://wordpress.org/) **2.** ter o plugin [**Insert Headers and Footers**](https://br.wordpress.org/plugins/insert-headers-and-footers/) instalado em seu **WordPress** e **3.** ter um **Formulário de Captura** ([estático](https://suporte.love/criar-formulario-estatico/) ou [dinâmico](https://suporte.love/como-criar-campos-dinamicos-e-como-criar-formulario-dinamico/)) criado aqui na **leadlovers**

**ATENÇÃO**:\
A **ausência e/ou inserção incorreta** dos respectivos códigos nos campos descritos neste tutorial, **resultará em mal funcionamento do formulário!**\
**TODOS os códigos devem ser inseridos!**

A seguir, você terá uma opção do passo a passo em vídeo. Em seguida, o mesmo passo a passo com texto e prints.

### &#x20;**Quais são os códigos do formulário estático de captura?**

Os formulários (Estático Padrão e Dinâmico) possuem três códigos:  CSS – código do formulário – JS . Conforme ilustração abaixo, respectivamente, são esses: primeiro, segundo e terceiro código.\
Códigos esses que devem ser inseridos cada um em seu devido campo dentro de sua página criada através do **WordPress**.

**Observação:** O formulário Estático Simples possui apenas 2 códigos: o CSS (configuração de layout) + o Código do Formulário. Mas, ambos podem ser inseridos juntos direto no corpo da página.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/atencao1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/atencao1.png)**IMPORTANTE:**\
– Caso esteja utilizando o formulário estático do tipo Simples (sem script) faça apenas a parte de [_**Inserindo o código**_](broken-reference).\
– Agora, se estiver usando o formulário estático do tipo Padrão (com script) ou o formulário Dinâmico realize também os passos da parte [_**Inserindo scripts HEAD e BODY**_](broken-reference).

Você pode conferir as diferenças entre os formulários nesse artigo [**aqui**](https://suporte.love/criar-formulario-estatico/).

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/formulrios-de-captura-teste-2-leadlove.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/formulrios-de-captura-teste-2-leadlove.png)

### **Inserindo o código do formulário na página**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/elementor.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/elementor.png)

**1 –** Após logar no **WordPress**, Acesse aba **páginas** > **todas as páginas**.

**2 –** Encontre a página em que o formulário está inserido e clique em “**Editar com Elementor**”

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/denovo.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/denovo.png)

**3 –** Após aparacer a página, no menu do canto esquerdo, arraste para a tela de edição o **widget Form.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/alalalal.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/alalalal.png)

**4 –** Em seguida, clique no formulário.

**5 –** No menu esquerdo, no campo código HTML, insira o **código do formulário** criado na leadlovers (**o segundo código**)

Salve.

**Observação:** Se você utiliza o formulário do tipo Estático Simples (sem script) o código CSS, o primeiro código, que ele possui pode ser inserido também direto no corpo da página junto ao corpo do formulário.\
É muito importante que a aplicação seja na ordem dos códigos: CSS primeiro e depois o restante.

### **Inserindo scripts HEAD e BODY pelo plugin Headers and Footers**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/insert.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/insert.png)

**6 –** Após i[nstalar o plugin **Insert Headers and Footers**](https://suporte.love/wordpress-plugin-scripts/), acesse, no menu lateral esquerdo, a aba **configurações**.

**7 –** Clique em **Insert Heanders and Footers**

**8 –** No campo **Scripts in Header**, insira o **primeiro código do formulário**, chamado de “**Arquivo CSS**“.

**9 –** No campo **Scripts in Footer**, insira o **terceiro código do formulário**, chamado de “**Arquivos JS**“

**10-** Salve.

**OBSERVAÇÃO:** Nos pop-ups nativos do plugin Elementor, os formulários estático do tipo Padrão (com script) e Dinâmico não funcionam.

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
