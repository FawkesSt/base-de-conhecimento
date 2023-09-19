# Como usar fontes do Google Fonts no Construtor por blocos

**Objetivo:** ensinar como utilizar fonte do Google Fonts nas páginas construídas na leadlovers.\
**Para que serve:** personalizar os textos de uma página criada além das fontes disponibilizadas por cada construtor.\
**Requisito(s) Obrigatório(s):** **1.** possuir uma página já criada no editor por blocos ou pelo editor por componentes.

**IMPORTANTE:** Vale ressaltar que essas configurações _**não são válidas para o editor Modelos Prontos**_ pois neste não é possível alterar os códigos HTML da página.\
Lembrando também que cada editor possui diversas alternativas de fontes.

### **Escolhendo a fonte no site do Google Fonts** <a href="#escolhendo-a-fonte" id="escolhendo-a-fonte"></a>

**Nº1–** Acesse fonts.google.com para escolher a fonte que utilizará na sua página.

**Nº2–** No campo Search, busque pelo nome da fonte que deseja utilizar.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem1.png)

**Nº3–** Depois de ter escolhido a fonte, clique em Select this style.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem2.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem2.png)

**Nº4–** Um menu lateral esquerdo se abrirá. Copie o script que surgiu e salve em um bloco de texto. Iremos utilizar este script logo mais.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem3.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem3.png)

Agora, vamos voltar para a edição da sua página na leadlovers.

### **Inserindo o script nas páginas** <a href="#inserindo-o-script" id="inserindo-o-script"></a>

#### **Configurações Avançadas** <a href="#configuracoes-pagina" id="configuracoes-pagina"></a>

Com o script da fonte em mãos, dentro da aba Páginas da máquina em questão, localize a página desejada.

**Nº5–** Clique no ícone de engrenagem ao lado da miniatura da página.

**Nº6–** Depois, selecione a opção Configurações.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem4.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem4.png)

**Nº7–** Irá abrir um pop-up, acesse a aba Configurações Avançadas.

**Nº8–** E em Scripts do Cabeçalho (HEAD), cole o script da fonte escolhida que copiou no site do Google Fonts ([passo 04](broken-reference) deste tutorial) e clique em **Salvar**.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem5.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem5.png)

**Observação:** o script utilizado neste tutorial é apenas demonstrativo, em sua página, será exibido o script da fonte que você escolheu.

Agora que você já inseriu o script da fonte no campo HEAD da página em questão, deverá definir em qual texto a fonte personalizada será aplicada. Abaixo mostramos como fazer isso em cada editor.

#### **Construtor por Blocos** <a href="#blocos" id="blocos"></a>

Para definir em qual texto a fonte será utilizada no editor por blocos inserimos diretamente no HTML do texto.

**Nº9–** Dentro da edição da página, escolha qual é o texto que deseja aplicar a fonte. Passe o cursor sobre o bloco onde o texto está e clique no botão “\</>HTML”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem1-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem1-1.png)

Feito isso abrirá a edição de HTML do bloco. Agora você irá encontrar o texto que deseja alterar nesse bloco dentro do código HTML.\
Nesse exemplo iremos alterar o texto “leadlovers, a plataforma completa para criação de estratégias de marketing digital.”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem2-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem2-1.png)

Quando localizar o texto dentro do HTML, procure o último “style” que aparece antes do mesmo e dentro dessa linha haverá um “font-family: fonte+atual;”

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem3-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem3-1.png)

**Nº10–** Você substituirá todo o font-family até o próximo ponto e vírgula ( ; ) pelo segundo código que o Google Fonts disponibilizou. Caso existam espaços no nome da fonte, substitua-os por “+”. Insira “!important” ao final do script antes do ponto e vírgula. No nosso exemplo resultando em:

font-family:’Hachi+Maru+Pop’,cursive!important;

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem4-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem4-1.png)

**Nº11–** Clique em “Salvar” no bloco.

**Nº12–** Salve as edições feitas na página.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem5-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem5-1.png)

**Resultado**

Fonte alterada com sucesso!

[![](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem6.png)](https://legado.leadlovers.site/wp-content/uploads/2021/01/Imagem6.png)



&#x20;**É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
