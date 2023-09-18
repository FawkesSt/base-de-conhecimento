# Integração Kiwify com Cursos (EAD)

Objetivo: Realizar integração de um Produto EAD criado na leadlovers com a Kiwify.\
Para que serve: Essa integração é feita entre a venda de um produto criado na Kiwify e um produto EAD criado aqui na leadlovers. Assim, quem fizer a compra pelo seu checkout na Kiwify automaticamente vai ser adicionado como aluno na sua conta leadlovers.\
Requisitos Obrigatórios: 1. Possuir um produto na [Kiwify](https://kiwify.com.br/), esse tipo de integração só pode ser feita na conta do produtor. 2. Ter um [produto EAD](https://suporte.love/nova-area-de-membros-como-criar-um-curso/) criado aqui na leadlovers.

Neste tutorial, te ensinaremos como fazer uma integração entre a plataforma Kiwify, especializada em vendas de infoprodutos, e o produto EAD da leadlovers. Com ela, você pode liberar um acesso à área de membros na leadlovers para os clientes que realizarem a compra do seu infoproduto. Caso queira integrar o Kiwify apenas com as suas máquinas aqui da leadlovers, pode fazer por meio da integração nativa acessando [esse link](https://suporte.love/como-integrar-o-kiwify-com-a-leadlovers/).

### Criando Webhook Kiwify <a href="#webhook-kiwify" id="webhook-kiwify"></a>

Nº1– Já logado em sua conta Kiwify, clique sobre a opção **“**Apps” no menu lateral esquerdo.&#x20;

Nº2– Selecione **“**Webhooks”, feito isso abrirá um menu na lateral direita da tela.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem1-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem1-1.png)

Nº3– Escolha um nome para a integração, apenas para organização pessoal.

Nº4– Nesse campo, cole a seguinte URL:&#x20;

https://machine.leadlovers.com/payment/kiwify

Nº5– Selecione com qual produto da Kiwify fará a integração. Caso tenha mais de um que será integrado com a leadlovers, escolha “Todos os produtos”.

Nº6– Atualmente essa integração é válida somente para o evento “Compra aprovada”, então marque apenas ele.

Nº7– Agora que as preferências foram personalizadas, basta salvar.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem2-2.png)](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem2-2.png)

Após realizar as configurações, sua tela do Kiwify ficará dessa forma:

[![](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem3-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem3-1.png)

### Definindo o produto que o cliente entrará <a href="#escolhendo-produto" id="escolhendo-produto"></a>

Integração configurada, agora iremos vincular um produto da Kiwify com o produto EAD em que deseja que seus alunos sejam adicionados. Primeiramente é necessário pegar o ID do produto Kiwify e então inseri-lo na leadlovers.

#### Kiwify <a href="#kiwify" id="kiwify"></a>

Nº8– No menu na lateral esquerda, vá até a opção **“**Produtos”.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem4-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem4-1.png)

Nº9– Esse passo é crucial para o funcionamento da integração. Clique sobre o nome do produto.\
Observação: essa é a forma correta da configuração, outros modos poderão afetar o funcionamento da mesma.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem5-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem5-1.png)

Feito isso você entrará na edição do produto, o ID deste se encontra na barra de endereços do navegador logo após: https://dashboard.kiwify.com.br/products/edit/.

Nº10– Copie o seu ID e salve-o, o bloco de notas pode ser um grande aliado.

[![](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem6-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem6-1.png)

#### leadlovers <a href="#leadlovers" id="leadlovers"></a>

Agora ensinaremos a fazer as configurações na [Área Antiga](broken-reference) e [Nova do Produto EAD](broken-reference). Siga os passos de acordo com a versão que costuma utilizar.&#x20;

**Produtos EAD – Área Antiga**

Nº11– Agora voltando para a leadlovers, acesse o seu produto EAD e vá até a aba **“**Integrações”.

Nº12– Role a página até localizar o campo **“**Integração com a Kiwify”.

Nº13– Aqui cole o ID do produto que copiamos no [passo 10](broken-reference).&#x20;

Nº14– Depois que concluir esta etapa, basta salvar as alterações e [testar a integração](broken-reference).

[![](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem7-2.png)](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem7-2.png)

Dessa forma, todo cliente que realizar a compra de seu produto na Kiwify será inserido como aluno na área de membros de seu produto EAD da leadlovers.

**Produto EAD – Área Nova**

Nº11– Dentro do seu produto EAD, vá até a aba **“**Integrações”.

Nº12– Localize o menu “Kiwify”.

Nº13– Em **“**Configurações de integração”, cole o ID do produto que foi copiado no [passo 10.](broken-reference)

Nº14– Salve as alterações e [teste a integração](broken-reference).

[![](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem8-1.png)](https://legado.leadlovers.site/wp-content/uploads/2021/11/Imagem8-1.png)

Assim, todos os clientes que realizarem a compra de seu produto na Kiwify serão adicionados como alunos na área de membros de seu produto EAD da leadlovers.\


### Testando a integração <a href="#testando-integracao" id="testando-integracao"></a>

É sempre muito importante testar todas as etapas de sua estratégia, certo? Antes de divulgar o seu produto para os seus clientes, teste o seu funcionamento para garantir que, no momento em que os alunos adquirirem ele, eles sejam inseridos corretamente no produto que foi configurado.

Para testar essa integração, realize a compra do produto e então busque pelo e-mail usado para efetuar a compra no produto EAD especificado na integração. Se a ação de inserir o cliente for realizada com sucesso, a integração está funcionando perfeitamente.\


**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, entre em contato com o nosso suporte!\


**Artigos relacionados**

– Como [localizar o seu Token Pessoal](https://suporte.love/como-localizar-o-seu-token-pessoal-na-leadlovers/) na leadlovers?\
– Como [criar um Produto EAD](https://suporte.love/nova-area-de-membros-como-criar-um-curso/)?\
– Como [integrar o Kiwify com as máquinas](https://suporte.love/como-integrar-o-kiwify-com-a-leadlovers/) da leadlovers?

🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™
