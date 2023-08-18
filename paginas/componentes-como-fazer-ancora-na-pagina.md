# Componentes: Como fazer âncora na página

Objetivo: Ensinar como vincular um link, botão ou menu a outro elemento da página.\
Para que serve: Com uma âncora configurada, é possível fazer com que ao clicar em um link, botão ou menu a página role até a parte desejada.\
Requisitos obrigatórios: Ter uma página criada no Construtor por Componentes, o editor padrão da leadlovers.

### Configurando a âncora <a href="#configurando-ancora" id="configurando-ancora"></a>

Nº1– Dentro do editor, vá até o componente que deverá ser o destino do botão, link ou menu. Por exemplo: se deseja que ao clicar em um botão a página role até um vídeo, localize este vídeo e clique sobre ele.

Nº2– No menu da lateral direita, encontre a opção “Identificador do bloco” e a ative.

Nº3– Em “ID” substitua a informação que vem de amostra por um nome que o ajude a localizar este bloco mais tarde. Não pode haver acentos ou espaços, então no nosso exemplo colocamos: _video-saiba-mais_.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/12/img01-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/12/img01-1.png)

Nº4– Selecione agora o botão, link ou menu que, ao clicar, deverá levar para o bloco que foi identificado.

Nº5– Em “Tipo do link” escolha a opção “Link interno”.

Nº6– No campo “Rolar para” selecione o bloco que você renomeou.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/12/img02-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/12/img02-1.png)

Agora basta salvar e conferir na sua página se está tudo certo! O resultado deverá ser similar ao do gif abaixo.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/12/img03.gif)](https://legado.leadlovers.site/wp-content/uploads/2021/12/img03.gif)

### E se eu quiser uma rolagem mais suave? <a href="#rolagem-suave" id="rolagem-suave"></a>

Por padrão, a configuração de âncora do editor apenas leva o usuário até o local da página indicado. No entanto, é possível deixar essa rolagem mais suave inserindo um código extra. Nos próximos passos ensinaremos a fazer este procedimento.

Nº7– Vá até a aba “Páginas” da sua máquina.

Nº8– Clique no ícone de engrenagem da miniatura

Nº9– Selecione a opção “Configurações”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/12/img04-2.png)](https://legado.leadlovers.site/wp-content/uploads/2021/12/img04-2.png)

Nº10– No pop-up que abrir, clique na aba “Configurações avançadas”.

Nº11– Em “Scripts do Corpo (Body)” insira o seguinte código:

\<style>\
html {\
&#x20;   scroll-behavior: smooth!important;\
}\
\</style>

Caso já tenha algum outro código já inserido, basta pular uma linha e colocá-lo logo abaixo.

Nº12– Salve as alterações.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/12/img05-2.png)](https://legado.leadlovers.site/wp-content/uploads/2021/12/img05-2.png)

Depois que inserir o código a rolagem da página ficará suave, assim como no exemplo:

[![](https://legado.leadlovers.site/wp-content/uploads/2021/12/img06.gif)](https://legado.leadlovers.site/wp-content/uploads/2021/12/img06.gif)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, entre em contato com o nosso suporte!

**Artigos relacionados**

– Como criar uma [página de captura](https://suporte.love/como-criar-e-configurar-uma-pagina-de-captura-no-editor-por-componentes/) no Construtor por Componentes?\
– Como criar uma [página de recompensa](https://suporte.love/como-criar-e-configurar-uma-pagina-de-recompensa-no-editor-por-componentes/) no Construtor por Componentes?\
– Como [criar um formulário](https://suporte.love/componentes-como-criar-um-formulario-dentro-do-editor/) no Construtor por Componentes?

🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™
