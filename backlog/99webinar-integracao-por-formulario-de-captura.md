# 99Webinar: Integração por Formulário de Captura

**Objetivo:** ensinar como integrar o 99webinar a sua plataforma de gerenciamento de leads/contatos.\
**Para que serve:** faz com que os leads capturados no cadastro do webinar também sejam capturados para dentro da ferramenta externa que você utiliza.\
**Requisito(s) obrigatório(s):** **1.** Já ter o Formulário de Captura criado lá no seu sistema externo e **2.** esse formulário precisa fornecer um código HTML do mesmo.

#### **O QUE É?**

Este tipo de integração permite que você use um formulário HTML, criado em outra ferramenta, para fazer com que os leads capturados no cadastro para o seu Webinar também sejam capturados para dentro desta ferramenta terceira.

Para isso, esta ferramenta (para onde deseja também enviar seus leads) precisa te fornecer o código de um formulário de captura, **do tipo \<form>**. Veja, abaixo, um exemplo de código desse tipo:

![](https://legado.leadlovers.site/wp-content/uploads/2019/04/99Webinar-%E2%80%93-Integracao-por-Formulario-de-Captura-360040814514\_1.jpeg)

#### **INSERINDO O FORMULÁRIO**

Todos os passos à seguir são feitos na tela de Integrações de seu Webinar.

Para chegar até essa tela, acesse o webinar onde deseja fazer a integração e clique no ícone de integrações, disponível no canto direito superior da tela, como mostra a figura abaixo:

![](https://legado.leadlovers.site/wp-content/uploads/2019/04/99Webinar-%E2%80%93-Integracao-por-Formulario-de-Captura-360040814514\_1-1.jpeg)

**1 –** Clique na opção **Outros**.\
**2 –** Copie o código do formulário que deseja integrar e cole-lo aqui.

![](https://legado.leadlovers.site/wp-content/uploads/2019/04/99Webinar-%E2%80%93-Integracao-por-Formulario-de-Captura-360040814514\_7.jpeg)

**CONFIGURANDO AS REFERÊNCIAS DE CAMPOS**

Agora, precisamos identificar quais os campos do formulário vão trazer os dados E-mail e Nome do lead. Volte ao exemplo de código que mostramos, e você vai perceber que tem duas linhas dele que começam com o código **\<input**. Este representa um campo onde o lead vai escrever seus dados.

**IDENTIFICANDO O CAMPO E-MAIL**

**3 –** No formulário que você colou na **etapa 2** deste tutorial, identifique quais dos códigos **\<input** representa o campo de E-mail. Nele, procure o atributo **id** e copie o valor dele, que está entre aspas.

No exemplo da imagem acima, localizamos o atributo id. O valor dele é a palavra **email**, que está entre as aspas.

![](https://legado.leadlovers.site/wp-content/uploads/2019/04/99Webinar-%E2%80%93-Integracao-por-Formulario-de-Captura-360040814514\_id.jpeg)

**4 –** Agora, cole o valor no **Campo referente ao E-mail**.

![](https://legado.leadlovers.site/wp-content/uploads/2019/04/99Webinar-%E2%80%93-Integracao-por-Formulario-de-Captura-360040814514\_4.jpeg)

**IDENTIFICANDO O CAMPO NOME**

**5 –** No formulário que você colou na **etapa 2** deste tutorial, identifique quais dos códigos **\<input** representa o campo de Nome. Nele, procure o atributo **id** e copie o valor dele, que está entre aspas.

No exemplo da imagem abaixo, localizamos o atributo id. O valor dele é a palavra **name**, que está entre as aspas.

![](https://legado.leadlovers.site/wp-content/uploads/2019/04/99Webinar-%E2%80%93-Integracao-por-Formulario-de-Captura-360040814514\_5.jpeg)

**6 –** Agora, cole o valor no **Campo referente ao Nome**.

**7 –** Após configurada a integração, clique no botão **Salvar**.

![](https://legado.leadlovers.site/wp-content/uploads/2019/04/99Webinar-%E2%80%93-Integracao-por-Formulario-de-Captura-360040814514\_6.jpeg)

#### **⚠ INFORMAÇÕES IMPORTANTES ⚠**

_**POSSO USAR FORMULÁRIOS COM OUTROS CAMPOS ALÉM NOME E E-MAIL?**_

Usar um código com campos além destes não adiciona novos campos de dados no formulário da página de cadastro do seu Webinar. Por isso, aconselhamos usar apenas os campos Nome e E-mail.

_**É POSSÍVEL USAR UM CÓDIGO DE FORMULÁRIO EM OUTRO FORMATO QUE NÃO SEJA O DO TIPO \<FORM>?**_

Até o momento, esta integração é funcional apenas com formulários do tipo **\<form>**.

**🏁 É isso, terminamos por aqui!**\
com amor ❤\
equipe **99Webinar™**
