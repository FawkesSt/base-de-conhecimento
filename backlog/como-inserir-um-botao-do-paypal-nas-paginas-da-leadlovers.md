# Como inserir um botão do PayPal nas páginas da leadlovers

**Objetivo:** Ensinar como inserir o botão do PayPal nas páginas\
da leadlovers via link e código HTML.\
**Para que serve:** Clicando no botão de venda inserido na sua página, o lead conseguirá fazer a compra do seu produto no PayPal e ser inserido na área de membros aqui na leadlovers.\
**Requisitos obrigatórios: 1.** Ter a integração com o PayPal já configurada. Se ainda não fez este procedimento, consulte [este material.](https://suporte.love/paypal/) **2.** Possuir o link do produto ou o código HTML do botão em mãos.&#x20;

Este artigo abrange os seguintes tópicos:

* [Como inserir o link e o código HTML no Construtor por Componentes?](broken-reference)
  * [Via link](broken-reference)
  * [Via Código HTML](broken-reference)

Nas páginas da leadlovers, é possível inserir o link de compra do seu produto em um botão criado direto pelo nosso editor ou\
até mesmo um código HTML com o botão que é gerado automaticamente no PayPal. Neste tutorial, te ensinaremos como fazer esses dois procedimentos no Construtor por Componentes.\


### **Construtor por Componentes** <a href="#componentes" id="componentes"></a>

Neste editor, é possível inserir o link do produto ou o código HTML do botão gerado pelo PayPal. Nos próximos passos ensinaremos como configurar cada uma das opções.

#### **Via link** <a href="#link-componentes" id="link-componentes"></a>

**Nº1–** Dentro do editor, em **“Conteúdo”** selecione a opção **“Botão**” e arraste até o local de sua página que deseja inseri-lo.

![](https://suporte.love/wp-content/uploads/2022/12/img01-7-195x300.png)

**Nº2–** Clique sobre o botão para configurá-lo e faça a sua customização da maneira que preferir.&#x20;

**Nº3–** Em **“Url”**, insira o link do PayPal que você copiou no\
tópico\
**“Copiando o link”** do tutorial [**“Produtos: Integração PayPal”**.](https://suporte.love/paypal/)

**Nº4–** Lembre-se de salvar a página e testar se o botão está funcionando corretamente antes de divulgá-la.

![](https://suporte.love/wp-content/uploads/2022/12/img02-7-300x151.png)

#### **Via Código HTML** <a href="#html-componentes" id="html-componentes"></a>

**Nº1–** Dentro do editor, em **“Conteúdo”** selecione a opção **“HTML**” e arraste até o local de sua página em que deseja inserir o botão.

![](https://suporte.love/wp-content/uploads/2022/12/img03-7-197x300.png)

**Nº2–** Clique sobre o componente com a frase **“Sou um novo bloco de HTML”**.

**Nº3–** Na janela que abrir na lateral direita, selecione todo o conteúdo que já vem por padrão e o exclua.

![](https://suporte.love/wp-content/uploads/2022/12/img04-7-300x151.png)

**Nº4–** Neste mesmo local, insira o código HTML que você copiou no\
tópico\
**“Copiando o código HTML do botão”** do tutorial[ **“Produtos: Integração PayPal”.**](https://suporte.love/paypal/)

**⚠️ ATENÇÃO:**&#x20;

**–** Para que o botão funcione corretamente, é necessário adicionar logo após a tag **\<form** do código a informação: **formulario-externo=””**. Por exemplo:

\<form **formulario-externo=””** action=”https://www.paypal.com/cgi-bin/webscr” method=”post” target=”\_top”>\
\<input type=”hidden” name=”cmd” value=”\_s-xclick”>\
\<input type=”hidden” name=”hosted\_button\_id” value=”00XXXX0X0X0X0″>\
\<input type=”image” src=”https://www.paypalobjects.com/pt\_BR/BR/i/btn/btn\_buynowCC\_LG.gif” border=”0″ name=”submit” alt=”PayPal – A maneira fácil e segura de enviar pagamentos online!”>\
\<img alt=”” border=”0″ src=”https://www.paypalobjects.com/pt\_BR/i/scr/pixel.gif” width=”1″ height=”1″>\
\</form>

**Nº5–** Depois que inseri-lo, o botão já aparecerá na sua página. Lembre-se de salvá-la e testar também na versão final se ele está funcionando corretamente.

![](https://suporte.love/wp-content/uploads/2022/12/img05-8-300x151.png)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, **entre em contato com o nosso suporte**!

**Artigos relacionados**

– Como fazer a [integração do PayPal com o Produto EAD da leadlovers](https://suporte.love/paypal/)?\
– Como [criar e configurar uma página de captura no Editor por Componentes](https://suporte.love/como-criar-e-configurar-uma-pagina-de-captura-no-editor-por-componentes/)?

**🏁 É isso, terminamos por aqui!**\
com amor **❤**\
**equipe leadlovers™**
