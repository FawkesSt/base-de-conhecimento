# Formulário Estático

**Objetivo:** Explicar o que é Formulário Estático de captura da leadlovers.\
**Para quê serve:** Permite integrar a leadlovers com páginas e sites criados externamente.\
**Requisito(s) Obrigatórios:** Possuir uma máquina de e-mail criada no leadlovers.

#### **O que é**

O jeito mais comum de integrar a leadlovers com sites externos é através dos Formulários de Captura criados na aba da máquina de mesmo nome.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/aba-formularios.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/aba-formularios.png)

Uma vez criado esse formulário você consegue pegar o código HTML dele e é esse código que será inserido no seu site de fora.\
Quando alguém se cadastrar por esse formulário entrará automaticamente como lead na sua Máquina dentro da leadlovers.

#### **Campos de Captura**

O formulário do tipo Estático possui 8 campos padrões:

* E-mail
* Nome
* Telefone
* Empresa
* Cidade
* Estado
* Data de Nascimento
* Mensagem

É possível “personalizar” os campos através do Placeholder.\
Exemplo: no campo de telefone, você pode colocar no placeholder “Informe seu WhatsApp”, assim, você mantém o uso de um campo Padrão, mas sem a necessidade de criar um formulário Dinâmico apenas para ter o campo “whatsapp” no seu formulário.

**⚠ Importante:**\
Caso queira saber como criar um formulário Dinâmico, com campos personalizados, [_**clique aqui e veja o material específico para este tipo de formulário**._](https://suporte.love/como-criar-campos-dinamicos-e-como-criar-formulario-dinamico/)

#### **Tipos de formulário**

Existem 2 tipos de Formulário Estático cuja distinção está no “**tipo de envio**“: _**Padrão**_ (com script) e _**Simples**_ (sem script).\
O Envio é a maneira como a informação do lead será enviada para o nosso sistema.\
Na prática, o que muda mesmo para o lead é como ele verá a mensagem de erro caso haja algum problema no preenchimento do formulário.

Outra principal diferença entre os formulários é a possibilidade de utilizar um Captcha.\
O Captcha é uma confirmação de cadastro para identificar que a ação foi feita por humanos e evita a entrada de bots/robôs em sua lista.\
Nós explicamos melhor sobre essa opção nesse tutorial aqui \[em breve].

**Observação:** Essa opção funciona apenas com o formulário do tipo Padrão.\
Recomenda-se ativar o uso do Captcha e, por isso, sugerimos o uso do tipo Padrão.

Abaixo detalhamos melhor as diferenças entre os Tipos.

**SIMPLES (sem script)**

Se você é cliente leadlovers antes de Setembro de 2020 esse é o “antigo” formulário estático.\
Houve uma mudança em sua estrutura de HTML e agora mostra separadamente um código de CSS que precisa ser inserido na HEAD.\
Esse código CSS sempre existiu, mas antes ficava junto ao corpo do formulário. Por diversos motivos, foi decidido que o melhor era separar essa parte do código e orientar que sua aplicação seja feito direto nos códigos HEAD da página.

Apesar de ser altamente recomendado que esse código seja inserido nas configurações de seu site na parte própria para aplicação de códigos HEAD, o mesmo não é obrigatório. Você pode inserir ele junto ao restante do corpo do formulário ou não inseri-lo.\
O principal objetivo desse código é o layout, ou seja, não tê-lo aplicado em sua página não irá afetar suas capturas.

Veja como fica o visual do formulário com e sem o CSS:

**SEM**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/sem.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/sem.png)

**COM**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/com.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/com.png)

Apesar dessa mudança no HTML o código desse formulário é bem simples e, por isso, ele pode ser facilmente aplicado em diversos construtores de sites externos.

Um outro ponto sobre esse tipo de formulário é que quando dá algum erro no cadastro o lead sai da página atual e é redirecionado para uma outra página que contém a seguinte mensagem:

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/unknown1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/unknown1.png)

**PADRÃO (com script)**

Esse é o “novo” formulário.\
Seu principal diferencial é a possibilidade de utilizar o Captcha e sua estrutura HTML é divida em 3 partes: códigos HEAD – corpo do formulário – códigos BODY.\
Cada um desses códigos precisam ser inseridos em locais específicos dentro da edição de sua página/site externo.

Por ter essa estrutura mais “complexa” e a necessidade de inserir os códigos em locais próprios é preciso _testar_ o uso desse formulário nos editores de fora.

Ao acontecer algum problema na captura, a mensagem de erro aparecerá na mesma página em que o lead já está:

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/unknown.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/unknown.png)

**TABELA DAS DIFERENÇAS ENTRE PADRÃO x SIMPLES**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/comparacao.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/comparacao.png)

#### **Criando o formulário**

Agora que você já sabe a diferença entre os 2 tipos de formulários, você já pode criar um Formulário Estático igual mostramos [nesse artigo aqui](https://suporte.love/criar-formulario-estatico/)!

#### **Inserindo nossos formulários em sites externos** <a href="#artigos" id="artigos"></a>

Se você já tem o formulário criado, dá uma olhada nessa lista de artigos que temos em nossa base ensinando como inserir nosso Formulário de Captura em diferentes construtores de páginas e temas/plugins do WordPress.

[KlickPages](https://suporte.love/formulario-captura-klickpages/)

[WIX](https://suporte.love/formulario-captura-wix/)

[WordPress tema básico](https://suporte.love/formulario-captura-wordpress/)

[Via Widget](https://suporte.love/wordpress-widget-integracao-leadlovers/)

[Plugin Boom](https://suporte.love/wordpress-plugin-bloom-integracao-leadlovers/)

[Plugin Ninja Popups](https://suporte.love/integrar-ninjapopups-leadlovers/)

[Plugin Thrive Architect](https://suporte.love/formulario-captura-thrive-architect/)

[Plugin Elementor (grátis)](https://suporte.love/formulario-captura-elementor/)

[Plugin Elementor PRO](https://suporte.love/wordpress-plugin-elementor-integracao-leadlovers/)

[Plugin OptimizePress](https://suporte.love/formulario-captura-optimizepress/)

[Plugin OptimizePress3](https://suporte.love/integracao-optimizepress3/)

[Tema Épico](https://suporte.love/tema-epico/)

[Tema Wolf](https://suporte.love/formulario-captura-tema-wolf/)

[Tema Avenger](https://suporte.love/formulario-captura-avenger/)

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
