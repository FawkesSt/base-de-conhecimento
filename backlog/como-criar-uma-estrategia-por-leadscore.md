# Como criar uma estrategia por leadscore

**Objetivo:** Entender a usabilidade do leadscore.\
**Para que serve:** Uma forma de aprender como utilizar o leadscore em estratégias de marketing.\
**Requisito(s) obrigatório(s): 1.** Ter uma máquina criada. **2.** Ter sua estratégia de vendas/Relacionamento definida.

[**Se você não sabe configurar, saiba mais clicando aqui.** ](https://suporte.love/como-adicionar-leadscore-na-captura-do-lead/)

### Exemplo de como criar uma estratégia por leadscore

Eu importei duas listas de clientes da minha loja, uma com clientes novos e outra com clientes antigos.\
Porém eu importei as duas pra mesma máquina.

#### Parte I : Como trabalhar a lista de leads

Usei o importador avançado, pra importar minha lista de leads com todas as **TAGS** corretas, **TOP** e **MID**.\
Eu preciso separar esses **leads** para que não recebam o mesmo conteúdo, visto que são listas diferentes. Para isso eu criei duas máquinas com o mesmo nome das tags.\
Para mover esses leads, eu vou na aba leads dentro da máquina e uso o **FILTRO AVANÇADO,** dessa forma consigo mover os leads **filtrando pelas tags.**&#x20;

Depois de inserir cada um em suas respectivas máquinas, eles passarão pelas sequências que criei, recebendo o relacionamento que programei.

#### Parte II : Como trabalhar a sequência e gatilhos

Essas sequências tem **GATILHOS DE SEQUÊNCIA** programados para mover os leads para outros funis quando eles clicam no conteúdo do e-mail, **GATILHOS DE ABERTURA** programados para **ADICIONAR** **UM LEADSCORE NEGATIVO** a cada abertura, para cada clique, além de movê-los eu aplico **LEADSCORE POSITIVO** em cada um deles, mostrando que quem tem mais pontuação positiva interagiu com mais e-mails, assim vou escalando eles de funil pra funil.

A lógica da pontuação é a seguinte:\
Abriu um e-mail : **-10**\
Clicou em um e-mail : **+30**\
Portanto, se ele receber abrir e clicar em um e-mail vai ter **20 pontos de leadscore**.

Como minha loja não para, eu continuo cadastrando novos clientes, mas dessa vez em poucas quantidades com a tag **NEW.**&#x20;

#### Parte III : Trabalhando novos leads

Todos esses leads entram na máquina **INICIO**, lá eu configuro um **GATILHO CONDICIONAL** para que permita apenas a passagem dos leads com essa tag **NEW**, assim não permito que nenhum outro cliente antigo receba esse mesmo conteúdo, gerando confusão.

Nessa próxima etapa eu vou começar a enviar e-mails com ofertas de produtos, dando opções para que o lead escolha uma delas, cada uma será um **LINK INTELIGENTE** diferente, com a ação de mover ele para funis diferentes relacionados à opção que escolheram.

#### Conclusão

Após ter tudo isso configurado, eu estou aplicando leadscore em todos os leads que interagem com os meus envios, o que significa que alguns vão estar bem engajados.\
Para todos os engajados eu quero entregar um presente, um cupom de desconto para que ele use na minha loja.\
Para automatizar esse processo eu crio uma máquina chamada **BÔNUS,** em seguida eu vou configurar um **GATILHO INTELIGENTE** que vai identificar todos os leads com leadscore maior que 150 e vai adicioná-los na máquina do cupom.

Para manter minha lista organizada, eu vou criar outro **GATILHO INTELIGENTE** para identificar todos os leads com leadscore negativo de -50 para a máquina **DESENGAJADOS.**\
Como na minha estratégia apenas os leads que clicam no meu conteúdo me interessam, os demais serão mandados pra outra máquina para que eu tente uma ação de recuperação por 5 dias com 1 e-mail por dia. Se não houver interação de nenhum desses 5 dias o **GATILHO DE FIM DE FUNIL** remove o lead da máquina e aplica a tag **DESENGAJADO.**\
\
Assim eu realizo uma ação mensal pra remover todos esses leads da conta.



🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™
