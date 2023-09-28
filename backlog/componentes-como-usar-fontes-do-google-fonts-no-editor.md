# Componentes: Como usar fontes do Google Fonts no editor

**Objetivo:** ensinar como utilizar fonte do Google Fonts nas\
páginas construídas na leadlovers.\
**Para que serve:** personalizar os textos de uma página criada\
além das fontes disponibilizadas por cada construtor.\
**Requisito(s) Obrigatório(s):** **1.** possuir\
uma página já criada no editor por blocos ou pelo editor por componentes.

Este artigo abrange os seguintes tópicos:

* [Escolhendo a fonte no site do Google Fonts](broken-reference)
* [Inserindo o script nas páginas](broken-reference)

### **Escolhendo a fonte no site do Google Fonts** <a href="#escolhendo-a-fonte" id="escolhendo-a-fonte"></a>

**Nº1–** Acesse fonts.google.com para escolher a fonte que\
utilizará na sua página.

**Nº2–** No campo Search, busque pelo nome da fonte que deseja\
utilizar.

![](https://suporte.love/wp-content/uploads/2022/12/img01-5-300x137.png)

**Nº3–** Depois de ter escolhido a fonte, clique em Select\
this style.

![](https://suporte.love/wp-content/uploads/2022/12/img02-5-300x137.png)

**Nº4–** Um menu lateral esquerdo se abrirá. Copie o script\
que surgiu e salve em um bloco de texto. Iremos utilizar este script logo mais.

![](https://suporte.love/wp-content/uploads/2022/12/img03-6-300x145.png)

Agora, vamos voltar para a edição da sua página na leadlovers.

### **Inserindo o script nas páginas** <a href="#inserindo-o-script" id="inserindo-o-script"></a>

#### **Configurações Avançadas** <a href="#configuracoes-pagina" id="configuracoes-pagina"></a>

Com o script da fonte em mãos, dentro da aba Páginas da máquina em questão, localize\
a página desejada.

**Nº5–** Clique no ícone de engrenagem ao lado da miniatura\
da página.

**Nº6–** Depois, selecione a opção Configurações.

![](https://suporte.love/wp-content/uploads/2022/12/img04-6.png)

**Nº7–** Irá abrir um pop-up, acesse a aba Configurações Avançadas.

**Nº8–** E em Scripts do Cabeçalho (HEAD), cole o script da\
fonte escolhida que copiou no site do Google Fonts ([passo 04](broken-reference) deste\
tutorial) e clique em **Salvar**.

![](https://suporte.love/wp-content/uploads/2022/12/img05-7-300x176.png)

**Observação:** o script utilizado neste tutorial é apenas\
demonstrativo, em sua página, será exibido o script da fonte que você escolheu.

Agora que você já inseriu o script da fonte no campo HEAD da página em questão,\
deverá definir em qual texto a fonte personalizada será aplicada. Abaixo mostramos\
como fazer isso em cada editor.

#### **Editor por Componentes** <a href="#componentes" id="componentes"></a>

Já no editor Componentes, a nova fonte a ser utilizada é definida nas configurações\
gerais da página.

**Nº13–** Dentro da edição da página, determine qual é o texto\
que deseja aplicar a fonte do Google Fonts ec lique sobre o texto escolhido.

**Nº14–** No menu lateral direito, ao final do menu, existe\
uma opção chamada **Identificador do bloco**, habilite-a.

**Nº15–** Logo abaixo surgirá um campo com o ID do bloco que\
você selecionou. Você pode alterar o ID e escrever qualquer palavra que lhe ajude\
a identificar que este ID se refere ao texto no qual deseja trocar a fonte. Neste\
exemplo, o ID ficou: textoinicial.\
Salve as novas alterações feita na página.

![](https://suporte.love/wp-content/uploads/2022/12/img12-2-300x141.png)

Guarde a identificação que criou pois iremos utilizá-la.

**Nº16–** Dentro das Configurações Avançadas da página, no\
campo Scripts do Cabeçalho (HEAD) – que você viu como acessar a partir do [passo 05](broken-reference) deste\
tutorial – insira um novo script.

O script é:

\<style>\
\#textoinicial{font-family:’Hachi+Maru+Pop’,cursive!important;}\
\</style>

Em “textoinicial”, substitua pelo nome do ID que você definiu no [passo 15](broken-reference).

E onde se encontra “font-family:’Hachi+Maru+Pop’,cursive;”, altere pelo código\
da fonte que você escolheu no Google Fonts.

![](https://suporte.love/wp-content/uploads/2022/12/img13-1-300x175.png)

Após realizar essas modificações, clique em **Salvar**.

**Resultado**

O texto da página que você alterou será exibida com a nova fonte que você definiu.

![](https://suporte.love/wp-content/uploads/2022/12/img14-1-300x154.png)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante\
este procedimento, por favor,\
**entre em contato com o nosso suporte**!

🏁 **É isso, terminamos por aqui!**\
com\
amor ❤\
equipe **leadlovers™**
