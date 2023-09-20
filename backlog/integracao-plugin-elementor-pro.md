# Integração plugin Elementor PRO

Se você caiu aqui aleatoriamente e não conhece o [WordPress](https://br.wordpress.com/), não sabe o que é um [Plugin](https://br.wordpress.com/install-plugins/) nem como isso pode ser integrado ao leadlovers, confere primeiro este artigo: [Integração leadlovers com WordPress](https://suporte.love/integracao-leadlovers-com-wordpress/)

**Objetivo:** Mostrar o passo a passo de como configurar um formulário de captura integrado ao Plugin Elementor PRO no WordPress.\
Para saber mais sobre o plugin Bloom e sua instalação no WordPress, consulte: [Bloom Email optin plugin for WordPress](https://www.elegantthemes.com/plugins/bloom/)

Para que serve: Capturar leads para sua máquina no Leadlovers, através de um formulário de captura, que foi criado pelo plugin Elementor Pro na sua página do WordPress.

**Requisitos:**

* Ter o **plugin Elementor Pro** instalado em seu WordPress;
* Ter o [**plugin leadlovers for Elementor**](https://wordpress.org/plugins/leadlovers-for-elementor/#utm\_medium=referral\&utm\_source=facebook.com\&utm\_content=social) instalado em seu WordPress.

#### Integrando leadlovers com Elementor

Primeiramente, dentro do painel do WordPress, será preciso instalar o plugin que vai possibilitar essa integração entre Elementor e leadlovers.

**ATENÇÃO**: Para que esta integração funcione, é necessário que você tenha o plugin Elementor instalado e a versão do **Elementor Pro** também. Isso porque na versão gratuita não há elementos, dentro do construtor de páginas, que possibilitem a criação de formulários, por exemplo.

**Nº 1** Acesse a aba **Plugins**, dentro do menu principal, no canto esquerdo da tela

**Nº 2** Clique em **Adicionar novo**\
\
**Nº 3** Na barra de pesquisa, busque por **leadlovers**\
\
**Nº 4** Assim que aparecer o plugin, clique em **instalar agora**. Após instalar, será evidenciado o botão **Ativar**. Clique nele para ativar o plugin em seu wordpress.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-9.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-9.png)

**Nº 5** Após ativar o plugin, acesse a aba **Elementor**, do menu esquerdo do seu WordPress

**Nº 6** Clique em **Configurações**\
\
**Nº 7** Clique na aba **Integrações**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-10.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-10.png)

**Nº 8** Role a página para baixo até encontrar a seção **leadlovers**

**Nº 9** Insira, no campo solicitado, o **Token pessoal** da sua conta leadlovers\
_(Não sabe como encontrar seu token?_ [_**Clique aqui**_](https://suporte.love/como-localizar-o-seu-token-pessoal-na-leadlovers/) _para saber como localizá-lo)_

**Nº 10** Clique em **Validar Token Pessoal. Ao validar, será possível verificar se ele consegue uma conexão do token com a sua conta**

**Nº 11** Clique em **Salvar alterações.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-11.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-11.png)

Para saber mais sobre o plugin leadlovers for Elementor e sua instalação no WordPress, consulte: [**leadlovers for Elementor**](https://wordpress.org/plugins/leadlovers-for-elementor/#utm\_medium=referral\&utm\_source=facebook.com\&utm\_content=social)

#### Configurando um formulário de captura com o plugin leadlovers for Elementor

Acessando o painel inicial do WordPress:

**Nº 1** Clique em **Páginas**\
\
**Nº 2** Clique em **Todas as páginas** e selecione a página a qual deseja editar.\


[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-13.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-13.png)

**Nº 3** Acesse o campo **Formulário** dentro das opções de edição do Elementor

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-14.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-14.png)

**Nº 4** Clique em **Actions After Submit**\
\
**Nº 5** No campo abaixo de **Add Action**, escolha a opção Leadlovers

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-15.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-15.png)

Ao Selecionar a opção Leadlovers, serão disponibilizados campos para a integração ser efetuada.

**Nº 7** Em **Máquina**, selecione a máquina desejada para capturar os leads.

**Nº 8** Em **Funil**, selecione o funil desejado.

**Nº 9** Em **Sequência**, selecione o nível do e-mail que deseja enviar ao lead, pós captura.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-16.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-16.png)

Abaixo das configurações de destino, você deverá configurar o mapeamento dos campos do seu formulário.

**ATENÇÃO!** Os campos elencados à esquerda representam as informações disponibilizadas pela leadlovers, na construção do formulário. Já os campos da direita, os quais são selecionáveis, representam as informações que você escolheu capturar dentro do formulário, no Elementor.

Em nosso exemplo, utilizaremos apenas os campos “nome” e “e-mail”.

**Nº 10** Em **Email**, selecione o campo correspondente ao e-mail do lead

**Nº 11** Em **Nome**, selecione o campo correspondente ao nome do lead.

**Nº 12** Clique em **Publicar/Atualizar**, para salvar as alterações e verificar como ficou sua integração.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-17.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/t1-17.png)

É importante evidenciar que, para cada campo inserido em seu formulário, você deverá realizar o mesmo procedimento de seleção, conforme ilustrado acima, afim de capturar todos os dados necessários e trazê-los até a leadlovers.

Campos descritos como **“None”** se referem às informações que estarão em branco, dentro do cadastro do lead, após a captura.

**ATENÇÃO!**\
O campo “Email” apresentará um asterisco em vermelho, de obrigatoriedade, **sempre** que se tratar de captura através de **máquinas de e-mail**.

Dentro da integração com o Elementor, também será possível vincular as informações dos leads às máquinas de SMS e Whatsapp. Nestes casos, o campo obrigatório **sempre** será o de telefone.

**Informações complementares:**

**1.** Caso seja necessário, dentro da opção “**leadlovers**“, antes da aba “**mapeamento dos campos**“, também há a possibilidade de **atribuir TAG’s aos leads** capturados pelo seu formulários Elementor.

**2.** **Mensagens de alerta também são customizáveis!** Você pode (des)habilitar opções de exibição de uma mensagem de erro aos seus leads, as quais aparecem assim que eles tentarem se cadastrar e já estiverem ativos na sua máquina, quando inserirem alguma informação que o sistema julga ser incorreta ou deixarem de inserir algum dado importante.





🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™\
