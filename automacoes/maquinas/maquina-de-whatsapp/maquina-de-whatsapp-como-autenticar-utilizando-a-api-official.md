# Máquina de WhatsApp: Como Autenticar utilizando a Api Official

**Objetivo:** Mostrar como conectar a conta de Whatsapp através da API oficial\
Para que serve: orientar os clientes na utilização da máquina de WhatsApp\
**Requisito Obrigatório:** Você precisa já ter uma conta de Whatsapp.

Nesse material, você vai aprender o passo a passo de como conectar seu número\
de Whatsapp via API Oficial para utilizar nas automações da leadlovers.

### Criando a conta no Facebook Developers

**N1º –** Comece acessando a página [http://developers.facebook.com/](https://developers.facebook.com/)

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-43-19.jpg" alt="" height="347" width="643"><figcaption></figcaption></figure>

**N2º** Clique no botão superior **em começar**, caso seu Facebook não esteja logado, clique em Entrar, informe suas credenciais e depois clique em Começar.

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-44-36.jpg" alt="" height="342" width="953"><figcaption></figcaption></figure>

**OBS**: Caso você ainda não tenha uma conta no developers, você cairá nessa tela. Preencha todos os dados solicitados para criar a sua conta de desenvolvedor.

**N3º –** Adicione um **numero de telefone celular valido** para fazer a verificação via SMS.\


<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-45-49.jpg" alt="" height="306" width="919"><figcaption></figcaption></figure>

**N4º –**  Clique em enviar **SMS para verificação** e depois coloque o código recebido no celular. clique em continuar.\


<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-47-04.jpg" alt="" height="336" width="886"><figcaption></figcaption></figure>

**N5º –** Confirme seu endereço de e-mail e clique em confirmar e-mail.

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-47-45.jpg" alt="" height="513" width="962"><figcaption></figcaption></figure>

**N6º –** Abrirá uma nova tela, escolha opção que melhor se enquadra no seu negócio.\


### **Criando o Aplicativo**

Após isso, seguimos para a criação do **app no facebook.**

**N1º –** Logo na tela inicial, clique no botão **“Criar Aplicativo”** para prosseguir.

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-49-41.jpg" alt="" height="358" width="951"><figcaption></figcaption></figure>

**N2º –** Em tipos de aplicativo, selecione o tipo **“Empresa”.** Essa opção é obrigatória. Lembre-se que o tipo de aplicativo não poderá ser alterado posteriormente.

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-50-33-1024x489.jpg" alt="" height="489" width="1024"><figcaption></figcaption></figure>

**N3º –** Escolha o nome de exibição que será o indicador para o seu aplicativo, este nome não ficará público.\
**OBS:** Caso você adicione algum termo não permitido o sistema emitirá um alerta.&#x20;

depois clique em **criar aplicativo**

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-51-35-1024x456.jpg" alt="" height="456" width="1024"><figcaption><p><em>Obs: A palavra WhatsApp não é permitida para o nome do aplicativo.</em></p></figcaption></figure>

**N4º –** Aparecerá uma janela de confirmação, informe a sua senha do Facebook para criar o aplicativo

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-52-55.jpg" alt="" height="537" width="851"><figcaption></figcaption></figure>

**N5º –** Confirme a senha do usuário do facebook e clique em **“Enviar”.**&#x20;

Nesta tela aparecem todos os produtos que podem ser adicionados ao seu

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-54-27-1024x481.jpg" alt="" height="481" width="1024"><figcaption></figcaption></figure>

Após isso, será preciso escolher o tipo de produto você deseja utilizar no Facebook developers.\
**localize o WhatsApp** e clique em configurar.

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-55-43.jpg" alt="" height="789" width="734"><figcaption></figcaption></figure>

Após isso, o sistema informará que uma conta empresarial da meta será criada. Clique em **“Continuar”**, na sequência.&#x20;

Prontinho! O seu aplicativo foi criado com sucesso!

### **Cadastrando seu número**

Agora é preciso adicionar o número de telefone que será utilizado na automação.

**N1º –**Dentro desta mesma tela do final do passo anterior, clique em **Configuração da Api** .

**N2º –** Descendo um pouco nesta página, encontramos a etapa 5º, **Clique em adicionar telefone.**

**N3º –** Preencha os dados da sua empresa corretamente.

**Importante:** Fique atento quanto ao preenchimento dessas informações, pois estas informações serão adicionadas em seu perfil do **WhatsApp Business** e todas elas estarão visíveis a seus clientes.

**N4º –** Após isso, clique em avançar e na tela seguinte adicione as informações do número de telefone. Escolha o país de origem e insira o número do telefone.&#x20;

**Importante:** É importante lembrar que, esse número _**não pode ter nenhum vínculo com nenhuma conta Whatsapp ou Whatsapp Business.**_

Caso você queira utilizar uma conta já utilizada no Business anteriormente, é preciso desvincular o número no business antes de criar essa autenticação.

**N5º –** Para finalizar, já com as informações preenchidas, opte por receber **um SMS de verificação e clique em “Avançar”**.

Você receberá um código de SMS em seu número, digite-o aqui e clique em “Avançar”.

### **Gerando Token de acesso permanente**&#x20;

**1-** Acesse: [https://business.facebook.com](https://business.facebook.com/)

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-57-34.jpg" alt="" height="559" width="961"><figcaption></figcaption></figure>

**2-** Você será direcionado a sua tela pessoal do meta Facebook

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-58-25.jpg" alt="" height="103" width="472"><figcaption></figcaption></figure>

**3-** Acessando essa tela no menu interior a esquerda, clique na engrenagem (Configurações)

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_15-59-28.jpg" alt="" height="657" width="985"><figcaption></figcaption></figure>

Nesse processo adicionaremos o usuário responsável para gerir o aplicativo.

**4-** Agora, **clique em usuários** < **usuários do sistema** < depois em **adicionar**\
**5-** Aceite os **termos do facebook**  e clique em concluir.

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-00-53.jpg" alt="" height="567" width="712"><figcaption></figcaption></figure>

\
\
6- Na nova tela, preencha com as informações solicitadas: de um **nome para o seu usuário** \
Depois só clicar em concluir.

\
**OBS. A função do usuário do sistema mudar para Administrador > Criar usuário do sistema > aceitar os termos de uso.**

#### **Adicionando o ativo ao usuário**

**O ativo nada mais é do que o aplicativo criado anteriormente.**

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-09-52.jpg" alt="" height="334" width="685"><figcaption></figcaption></figure>

**1-** Clique em **adicionar ativos**

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-10-42.jpg" alt="" height="340" width="605"><figcaption></figcaption></figure>

**2-** Escolha a opção aplicativos, e selecione o aplicativo criado anteriormente.

**3-** Habilite a configuração de “controle total”. e depois em salvar alterações.

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-12-20.jpg" alt="" height="141" width="341"><figcaption></figcaption></figure>

Após isso, nesta mesma tela, clique em **Gerar novo token**

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-13-17.jpg" alt="" height="185" width="308"><figcaption></figcaption></figure>

**4-** Abrirá uma nova janela para geração do token, clique em Selecionar aplicativo, e vincule o aplicativo criado anteriormente.

Nesta mesma tela, terá uma lista de comandos, é necessário habilitar duas permissões: **Whatsapp.business\_management  e  Whatsapp.business\_messaging**

Após isso clique em gerar token.

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-16-04.jpg" alt="" height="274" width="302"><figcaption></figcaption></figure>

Perfeito, token gerado com sucesso!

O próximo passo é adicionar esse token na leadlovers.

### Autenticando WhatsApp utilizando CLOUD API

Ainda com a tela anterior aberta, em uma nova aba acesse a leadlovers.

**Primeiro passo é criar uma conta de WhatsApp caso ainda não possua a sua.**\
**Caso possua, avance o tutorial para o passo 4.**&#x20;

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/9.png" alt="" height="233" width="240"><figcaption></figcaption></figure>

**1-** Acesse **contas de Whatsapp**&#x20;

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-19-06.jpg" alt="" height="145" width="403"><figcaption></figcaption></figure>

**2-** Clique em adicionar **nova conta** ( caso seja sua primeira vez)

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-19-46.jpg" alt="" height="366" width="558"><figcaption></figcaption></figure>

**3-** Preencha os dados solicitados, como nome da nova conta. ( será utilizado apenas para identificação).

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-28-18.jpg" alt="" height="466" width="426"><figcaption></figcaption></figure>

**4-** Clique nos 3 pontinhos, e clique em **autenticar**&#x20;

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-29-58.jpg" alt="" height="555" width="713"><figcaption></figcaption></figure>

**5-** Escolha a opção **Cloud API** e clique em **continuar**&#x20;

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-31-01.jpg" alt="" height="642" width="709"><figcaption></figcaption></figure>

**6-** Cole o token que geramos e copiamos anteriormente,

**caso necessário retorne a outra janela copie o token novamente, lembre-se de manter a janela aberta.**

**7-** Próximo e ultimo passo é copiar o **ID do telefone o ID do Whatsapp business.** \
Para isso abra novamente a aba de aplicativos em facebook developers

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-45-32.jpg" alt="" height="220" width="220"><figcaption></figcaption></figure>

**8-** No menu lateral, clique em **Whatsapp < começar**

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-46-19.jpg" alt="" height="218" width="623"><figcaption></figcaption></figure>

**9-** Nessa tela, copie o ID do telefone e adicione na leadlovers, o mesmo para o ID do WhatsApp business.

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-47-39.jpg" alt="" height="334" width="429"><figcaption></figcaption></figure>

Pronto, agora estamos quase lá 🙂

E por último, após autenticar a máquina irá gerar uma URL de retorno, copie essa URL de retorno e adicione em seu aplicativo no Facebook developers.

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-53-26.jpg" alt="" height="334" width="431"><figcaption></figcaption></figure>

### Adicionando URL de retorno no Facebook Developers

Após copiar a URL de retorno;

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-49-37.jpg" alt="" height="172" width="196"><figcaption></figcaption></figure>

**1-** Retorne a área de aplicativos no Facebook developers, na parte de Whatsapp, **clique em Configuração**

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-51-07.jpg" alt="" height="325" width="660"><figcaption></figcaption></figure>

**2-** Em Webhook, clique em Editar e adicione o **URL de retorno da chamada.**&#x20;

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-52-08.jpg" alt="" height="171" width="411"><figcaption></figcaption></figure>

**3-** Após isso, retorne a leadlovers e naquela mesma tela de autenticação copie o **Token de acesso**, e cole logo abaixo da URL de chamadas.

Após isso clique em verificar e salvar.

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-54-46.jpg" alt="" height="164" width="686"><figcaption></figcaption></figure>

Para finalizar, Clique em gerenciar e ative a opção messages  (mensagens)

<figure><img src="https://suporte.love/wp-content/uploads/2023/04/2023-04-19_16-55-11.jpg" alt="" height="423" width="678"><figcaption></figcaption></figure>

Prontinho!

após isso sua automação estará ativa na leadlovers.

[https://www.youtube.com/watch?v=px8tmnbtmaQ](https://www.youtube.com/watch?v=px8tmnbtmaQ)

**Assuntos Relacionados:** \
– [Como criar templates de mensagem ](https://suporte.love/como-criar-uma-sequencia-de-mensagem-na-maquina-de-whatsapp/)\
– [Como funcionam os gatilhos da máquina de whatsapp](https://suporte.love/como-funcionam-os-gatilhos-na-maquina-de-whatsapp/)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante\
este procedimento, por favor, **entre em contato com o nosso suporte**!

🏁 **É isso, terminamos por aqui!**\
com\
amor ❤\
equipe **leadlovers™**
