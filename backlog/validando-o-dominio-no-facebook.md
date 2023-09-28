# Validando o domínio no Facebook

**Objetivo:** mostrar como validar no Facebook um domínio ou subdomínio usado em páginas criadas na leadlovers via MetaTag.\
**Para que serve:** configurar para que você possa utilizar seu domínio ou subdomínio em campanhas no Facebook.\
**Requisito(s) obrigatório(s):** **1.** ter uma conta _empresarial_ no [Business Manager do Facebook](https://business.facebook.com/); **2.** ter um domínio ou subdomínio próprio [apontado e cadastrado](https://suporte.love/o-que-e-um-dominio/) na leadlovers; **3.** ter uma [página ativa criada](https://suporte.love/componentes-visao-geral/) na máquina em que o domínio está cadastrado e **4.** a rota do domínio [não pode ser aleatória](https://suporte.love/como-cadastrar-dominio-maquina/).

Visando preservar a segurança de seus usuários, o Facebook agora exige que todo domínio compartilhado na rede social seja verificado com um código de validação, entrada DNS ou arquivo no diretório raiz do domínio. Esse procedimento garante a eles que a pessoa possui total controle do domínio usado.

Aqui na leadlovers, você pode fazer esse procedimento para compartilhar suas páginas criadas na plataforma com o seu domínio próprio. Para isso, utilizaremos o método de validação via MetaTag.

#### **Gerando o código Metatag** <a href="#copiando-codigo" id="copiando-codigo"></a>

**Nº1–** Acesse seu perfil [Business Manager do Facebook](https://business.facebook.com/). No menu lateral esquerdo, clique em “Configurações”.

**Nº2–** Selecione a seção “Mais configurações do negócio”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem1.png)

**Nº3–** Acesse a categoria “Segurança da marca”.

**Nº4–** Vá até a opção “Domínios”. Feito isso, novas informações serão mostradas no centro da tela.

**Nº5–** Clique em “Adicionar” para cadastrar um novo domínio/subdomínio.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem2.png)](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem2.png)

**Nº6–** Na pop-up que abrir, insira o domínio/subdomínio que será utilizado. Vale frisar que nessa parte não é necessário o uso de “http”, “https” ou “www”.

**Nº7–** Clicando em “Adicionar” você será redirecionado para a tela que mostra as opções de validação.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem3.png)](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem3.png)

**Nº8–** Escolha a opção “Adicione uma metatag ao seu código fonte HTML”. Por padrão ela já vem selecionada, mas, caso necessário, altere.

**Nº9–** Clique sobre o código que se inicia com “\<meta name=…” para que seja copiado para a sua área de transferência. Guarde-o em um local seguro, o bloco de notas pode ser um grande aliado.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem4.png)](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem4.png)

#### **Inserindo o código na leadlovers** <a href="#inserindo-codigo" id="inserindo-codigo"></a>

Para que o Facebook possa validar um domínio é necessário que o código de verificação esteja em todas as páginas do domínio/subdomínio em questão. Então bora fazer?

Mantenha a sua aba do Facebook aberta e em uma outra aba, acesse a leadlovers.

**Nº10–** Na leadlovers acesse a aba “Configurações” dentro da máquina em que o domínio está cadastrado.

**Nº11–** Vá até a seção “Scripts Globais (HEAD)”. Feito isso, abrirá um campo de texto para adicionar scripts em todas as páginas da máquina em questão.

**Nº12–** Insira o código copiado no [passo 09](broken-reference) neste campo.

**Observação:** caso já tenha algum código ou códigos aqui, vá até o fim desse(s) script(s) e pule a linha duas vezes usando a tecla “Enter”. Depois é só colar o código de verificação do Facebook.

**Nº13–** **Salve** as alterações.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem5.png)](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem5.png)

#### **Verificando a configuração** <a href="#validando" id="validando"></a>

Agora que todas as configurações foram feitas, volte ao Facebook onde iremos validar se o mesmo consegue identificar o código inserido nas páginas. Após essa etapa, o domínio estará pronto para ser utilizado em campanhas.

**Nº14–** Novamente no Business Manager, na tela em que pegamos o código da MetaTag, clique em “Verificar domínio”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem6.png)](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem6.png)

**Nº15–** No pop-up que abrir, conclua a configuração.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem7.png)](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem7.png)

#### **Resultado** <a href="#resultado" id="resultado"></a>

Se toda a configuração for validada, sua tela de domínios do Facebook ficará semelhante à imagem abaixo:

[![](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem8.png)](https://legado.leadlovers.site/wp-content/uploads/2021/09/Imagem8.png)

Caso o domínio não fique como “Verificado”, revise os passos desse tutorial e, se ainda assim não funcionar, entre em contato com nosso time de suporte.

**Artigos recomendados**

– [O que é Pixel do FB](https://suporte.love/o-que-e-pixel-do-facebook/);

– Como [inserir um script](https://suporte.love/inserir-script/) nas páginas da leadlovers.

🏁 **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
