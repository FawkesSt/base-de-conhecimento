# Estratégia de segmentação por Engajamento

**Objetivo:** Ensinar como segmentar seus leads, dos mais quentes aos mais frios, com base na informação de Engajamento de Leads.

### **O que é**

Para obter bons resultados com o e-mail marketing é essencial fazer a correta manutenção da sua lista de leads, mantendo uma comunicação apenas com leads engajados, isto é, aqueles que interagem com seus e-mails. A limpeza da lista deve ser feita com uma frequência que varia de acordo com o fluxo de seus envios, mas não deve ultrapassar um mês.

Um dos principais motivos de remover os leads frios da sua base é manter uma boa reputação perante os provedores de e-mail, que possuem filtros anti-spam que monitoram o seu comportamento e analisam a qualidade dos seus envios. O motivo disso é proteger os usuários contra e-mails indesejados, então, se você insistir em fazer envios para leads que não estão interagindo com seus e-mails, você será reconhecido como _spammer_, e seus e-mails não serão mais entregues na caixa de entrada dos destinatários.

Bem, agora que você já entendeu a importância de realizar a higienização da sua lista com a frequência correta, vou te mostrar uma das maneiras de fazer isso com a leadlovers, usando uma estratégia que tem apresentado muito resultado positivo.

A finalidade dessa estratégia é segmentar a sua base de leads em grupos, de acordo com sua “temperatura”, isto é, os que engajam nos seus e-mails e então remover os leads desengajados.

Existe uma pontuação interna do sistema que é aplicada automaticamente aos leads conforme as interações deles com os e-mails. Ela funciona assim:

* A cada e-mail que o lead **recebe**, o sistema aplica **-1 ponto**
* A cada e-mail que o lead **abre**, o sistema aplica **10 pontos**
* A cada e-mail que o lead **clica**, o sistema aplica **20 pontos**

De acordo com essa pontuação, conforme os leads forem interagindo e recebendo “pontos” pelo engajamento, eles são divididos em quatro grupos:

* Quentes
* Mornos
* Indefinidos
* Frios

### **Como fazer**

Vamos ao passo a passo de como configurar essa estratégia:

Nº1– [Crie 4 tags](https://suporte.love/como-criar-uma-tag/) em sua conta:

➜ Quente\
➜ Morno\
➜ Indefinido\
➜ Frio

DICA: Crie uma categoria com o nome “engajamento” e insira essas tags dentro dela.

Nº2– [Crie 4 gatilhos inteligentes](https://suporte.love/criar-e-configurar-gatilhos-inteligentes/):

* **Leads quentes**

_➜_ Filtro: leads com engajamento entre 29 e infinito\
➜ Ações:

➢ Aplicar a tag Quente\
➢ Remover a tag Morno\
➢ Remover a tag Indefinido\
➢ Remover a tag Frio

* **Leads mornos**

➜ Filtro: leads com engajamento entre 1 e 28\
➜ Ações:

➢ Aplicar a tag Morno\
➢ Remover a tag Quente\
➢ Remover a tag Indefinido\
➢ Remover a tag Frio

* **Leads indefinidos**

➜ Filtro: leads com engajamento entre -4 e 0\
➜ Ações:

➢ Aplicar a tag Indefinido\
➢ Remover a tag Quente\
➢ Remover a tag Morno\
➢ Remover a tag Frio

* **Leads frios**

➜ Filtro: leads com engajamento entre -infinito e -5\
➜ Ações:

➢ Aplicar a tag Frio\
➢ Remover a tag Quente\
➢ Remover a tag Morno\
➢ Remover a tag Indefinido

DICAS:\
– Aqui também você pode criar a categoria “engajamento” para esses gatilhos.\
– Use um número grande para o infinito, como por exemplo: 1000000000

Nº5– Ative a recursividade em todos esses gatilhos inteligentes.

Nº6– Remova da conta, com a frequência de pelo menos um mês, os leads com a tag Frio.

**É isto, terminamos por aqui!**\
com amor**❤**\
equipe **leadlovers™**
