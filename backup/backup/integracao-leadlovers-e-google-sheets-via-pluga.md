# Integração Leadlovers e Google Sheets via Pluga

**Objetivo**: Simplificar a forma de integração do **Google sheets** via Pluga\
**Para que serve:** Com esta integração você pode **adicionar uma nova** linha no Google Sheets a partir de algumas ações na leadlovers ou quando uma nova linha for criada no Google Sheets, você pode criar/atualizar um lead na leadlovers.

### **O que é a Pluga?** <a href="#o-que-pluga" id="o-que-pluga"></a>

A [Pluga](https://pluga.co/?utm\_source=central+de+ajuda\&utm\_id=leadlovers) é uma plataforma de integração que ajuda diversas empresas a eliminarem as tarefas manuais e trabalhosas do dia a dia, tornando, assim, suas equipes mais estratégicas e poupando aqueles esforços que podem ser automatizados. E o melhor: sem precisar ter nenhum tipo de conhecimento técnico.

Além disso, a **Pluga** oferece um período de testes **100% gratuito por 7 dias** que permite experimentar todas as funcionalidades disponíveis.\
Uma excelente notícia: Para _clientes leadlovers_ a Pluga também disponibilizou um **cupom de desconto** “LOVE” com 20% de desconto nos 3 primeiros meses.

Confira [aqui](https://pluga.co/precos/?utm\_source=central+de+ajuda\&utm\_id=leadlovers) todas as funcionalidades, planos e preços da Pluga.

Neste tutorial, ensinaremos como você pode adicionar uma linha no Google Sheets ou criar e atualizar leads na leadlovers a a partir da realização de algumas ações, são elas:

* Quando o lead atender o(s) filtro(s) Pré-definidos.
* ou quando um novo lead for criado na leadlovers\


### &#x20;**Criando uma integração entre Google Sheets (origem) e leadlovers (destino)** <a href="#o-que-preciso-saber" id="o-que-preciso-saber"></a>

Acessando a [**página do leadlovers na Pluga**](https://www.google.com/url?q=https://pluga.co/ferramentas/leadlovers/integracao/\&sa=D\&source=docs\&ust=1677251797979937\&usg=AOvVaw2pU1zNG6IM73o6wQjSmLwe), você terá uma variedade de possíveis integrações, utilize a barra de busca para localizar o Google Sheets, ou [**clique aqui**](https://pluga.co/ferramentas/leadlovers/integracao/google\_sheets/).

![](https://suporte.love/wp-content/uploads/2023/02/1-1-1024x479.png)

Acessando a página da **leadlovers+Google Sheets**, você poderá configurar 3 tipos de ações, são elas:

* Quando uma nova linha for criada no Google Sheets, criar/atualizar lead na leadlovers
* Quando um novo lead for criado na leadlovers, inserir no Google sheets
* Quando o lead atender os filtros (ex: tags, leadscore…) um gatilho inteligente da leadlovers adicionará o lead ao Google Sheets.

Após ter escolhido uma das automações citadas acima, clique em “Fazer essa automatização”.

**Login da Ferramenta**\
**Em seguida, você vai conectar a sua conta do Leadlovers e Google Sheets para que a Pluga consiga integrar as duas ferramentas.**

#### ![](https://suporte.love/wp-content/uploads/2023/02/2-2.png)

Em uma nova aba acesse a leadlovers e faça login na sua conta.

![](https://suporte.love/wp-content/uploads/2023/02/2.jpg)

1. Dentro da leadlovers, no canto superior direito clique no ícone com suas iniciais/ou sua foto de perfil
2. clique em meu perfil, você será direcionado a uma nova página![](https://suporte.love/wp-content/uploads/2023/02/4.jpg)
3. Agora é só rolar a página e copiar seu Token Pessoal.\
   _Lembrando que, caso você ainda tenha dúvidas de como localizar seu token, clicando em “encontrar seu token pessoal” você terá acesso a um tutorial detalhado._

![](https://suporte.love/wp-content/uploads/2023/02/3.png)

Retorne ao pluga, cole seu **token pessoal** na área descrita acima.

![](https://suporte.love/wp-content/uploads/2023/02/4-1.png)

Com as contas já conectadas, é só clicar em “Continuar”.

### Configure a planilha para funcionar com a automação

Para esse passo você vai precisar criar e configurar a planilha que será utilizada nessa integração. Seguindo as seguintes instruções:

![](https://suporte.love/wp-content/uploads/2023/02/5.png)

1. Crie uma nova planilha em branco no google sheet
2. A primeira linha na planilha precisa ser o cabeçalho, isso se aplica a todas as colunas.
3. Essa integração requer alguns campos obrigatórios, nas colunas especificas, como:\
   **Coluna A**: E-mail\
   **Coluna B:** Nome\
   Esses campos são obrigatórios.
4. Você poderá adicionar outros campos nas demais colunas.**Importante:** É preciso utilizar uma planilha nova e não deletar nenhuma linha após a configuração da automação.\
   É extremamente importante seguir esses passos acima antes de criar a automação.

#### Configurando a integração entre Google Sheets e leadlovers

![](https://suporte.love/wp-content/uploads/2023/02/6.png)

Agora retornando ao pluga,  Você irá selecionar qual a planilha, aba da planilha e coluna de gatilho.\
A coluna gatilho é aquela que irá disparar essa automação. Ou seja, depois que ela for preenchida os robôs entenderão que toda a linha está completa (por isso sugerimos que selecione a última coluna a ser preenchida).

Após selecionar as opções da sua planilha no Google Sheets, você irá ajustar as opções do Leadlovers, indicando qual máquina, funil e sequência irá receber o novo lead:

![](https://suporte.love/wp-content/uploads/2023/02/7.png)

### Personalizando os dados

Chegamos então na última etapa de criação da sua automatização que vai integrar sua planilha do Google Sheets com a leadlovers: a etapa de personalização dos dados.\
É nessa etapa que você vai dizer quais dados da sua planilha do Google Sheets irão para a leadlovers.

![](https://suporte.love/wp-content/uploads/2023/02/8.png)

Terminando a personalização desses campos, você pode descer a tela e clicar em “Finalizar automatização”. Dessa forma, está criada a sua automatização.

#### **Criando uma integração com Gatilho Inteligente da leadlovers (origem) e Google Sheets (destino):**

Inicie a página da leadlovers no pluga conforme informado nos passos anteriores e selecione o tipo de integração.

![](https://suporte.love/wp-content/uploads/2023/02/9.png)

Clicando aqui, você receberá um aviso que **todos os leads** inclusive os antigos, que _**atenderem os filtros selecionados**_ serão enviados para sua planilha do Google Sheets através dessa automatização. Caso seja isso que deseja e é só clicar em continuar para acessar a tela de login

Em seguida, você **vai precisar conectar a sua conta da leadlovers e Google Sheets** para que a Pluga consiga integrar as duas ferramentas.\
Caso tenha dúvidas de como fazer isso, basta acessar o passo a passo descrito anteriormente, clicando aqui #logindaferramenta

![](https://suporte.love/wp-content/uploads/2023/02/10.png)

Próximo passo é adicionar a URL do pluga dentro da área de gatilho inteligentes da leadlovers.

![](https://suporte.love/wp-content/uploads/2023/02/12.png)

1. Copie a URL do pluga\
   ![](https://suporte.love/wp-content/uploads/2023/02/659.jpg)
2. Dentro da leadlovers, acesse:\
   – No menu superior clique em ferramentas\
   – Gestão de contatos\
   – Ações automatizadasVocê será direcionado para a página de Gatilhos Inteligentes, clique em **+** para criar seu **novo gatilho** para essa automação.\
   ![](https://suporte.love/wp-content/uploads/2023/02/13.png)
3. Escolha o  nome do gatilho de acordo com a automatização que irá criar, assim você poderá editá-lo ou desativá-lo com facilidade.\
   Após criar seu gatilho, você poderá observá-lo na lista de gatilhos.![](https://suporte.love/wp-content/uploads/2023/02/888.jpg)
4. O próximo passo é criar um filtro para segmentar seus leads. Clique no número  na coluna Filtros.\
   ![](https://suporte.love/wp-content/uploads/2023/02/14.png)**Obs:**Caso não tenha nenhum filtro criado ainda, o número que aparecerá nesse espaço selecionado, será zero. Clicando no número\
   abrirá um Popup em sua tela, clique no botão novo filtro.\
   \
   ![](https://suporte.love/wp-content/uploads/2023/02/dfg.png)
5. Agora, SELECIONE o tipo de filtro que deseja usar para segmentar os leads, depois clique em **SALVAR.**![](https://suporte.love/wp-content/uploads/2023/02/cccc.jpg)
6. Após salvar você retornará a tela anterior, agora o próximo passo é criar uma AÇÃO para esse gatilho. Para isso, clique no número 0 na coluna Ações e em seguida em “Criar Ação”.![](https://suporte.love/wp-content/uploads/2023/02/fgv.png)
7. Abrirá um pop up em sua tela, selecione o Tipo da Ação: ExecutarHttpPost Simples.
8. Lembra que copiamos a URL no começo do tutorial? Cole a URL do pluga dentro da ação no campo URL.\
   Caso não tenha certeza se copiou o link, sem problemas, volte na Pluga e no campo da URL, clique no botão para copiar a URL.\
   Após copiá-la, retome no ponto em que estávamos na página do leadlovers.![](https://suporte.love/wp-content/uploads/2023/02/dgt.png)
9. Para terminar a configuração da Ação, clique no campo Tipo de comunicação e selecione: POST. E por último, mas não menos importante, clique em SALVAR.

Pronto, a ação foi criada com sucesso! Só que para ativá-la, é preciso Testar execução. Sendo assim, clique no símbolo de avião de papel, para realizar o teste e validar a ação.

![](https://suporte.love/wp-content/uploads/2023/02/dfre.jpg)\


Com seu teste realizado com sucesso, clique em OK para fechar. Seu gatilho está ATIVO, agora é só continuar sua automatização na Pluga.

![](https://suporte.love/wp-content/uploads/2023/02/15.png)

Conecte com a próxima ferramenta que irá automatizar, nesse caso, o Google Sheets e clicar em “Continuar”.

No passo seguinte, você ajusta as opções do **Google Sheet**s, escolhe qual planilha e página receberá os dados do lead e é só clicar em continuar para avançar para próxima etapa.

![](https://suporte.love/wp-content/uploads/2023/02/16.png)

Chegamos então na última etapa de criação da sua automatização que vai integrar o Leadlovers com sua planilha do Google Sheets, nessa etapa você irá selecionar quais informações do Leadlovers você quer levar para cada coluna da planilha.

![](https://suporte.love/wp-content/uploads/2023/02/18.png)

Além de uma série de colunas já pré-definidas (que você pode remover se não achar necessário), você pode acrescentar novas colunas, precisando apenas nomear o cabeçalho da coluna (1º campo) e selecionando no 2º campo qual informação quer puxar do Leadlovers para essa coluna através do botão “+ inserir infos da Leadlovers”.

![](https://suporte.love/wp-content/uploads/2023/02/19.png)

Terminando a personalização desses campos, você pode descer a tela e clicar em “Finalizar automatização”. Dessa forma, está criada a sua automatização

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, entre em contato com o nosso suporte!

🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™
