# Como criar uma entrada de subdomínio na GoDaddy?

**Objetivo:** Passo a passo de como criar uma entrada de _**subdomínio**_\
no GoDaddy.\
**Para que serve:** Um mesmo subdomínio/domínio não pode ser\
usado em mais de uma máquina ao mesmo tempo, aqui na leadlovers.\
Junto a isso, nestes tipos de caso, aconselhamos criar um novo subdomínio.\
**Requisito(s) Obrigatório(s):** **1.** Possuir\
um domínio próprio; **2.** Possuir acesso a hospedagem\
do domínio.

Este artigo abrange os seguintes tópicos:

* [Como acessar a Zona de DNS de seu domínio](broken-reference)
* [Realizando as configurações](broken-reference)
* [Apontamento configurado, e agora?](broken-reference)

### **Em quais casos eu posso utilizar um subdomínio?**

Situações comuns são:

* Meu domínio principal está sendo usado em outro site/ferramenta;
* Meu domínio principal já está sendo usado em outra máquina na leadlovers.

**📢 IMPORTANTE:**

**–** Os passos a seguir devem ser feitos\
**somente se o seu domínio for administrado pelo RegistroBR.**\
Se ele estiver sob administração de outro serviço, é preciso que as configurações\
sejam realizadas no Painel de Controle específico deste segundo serviço. [Nesse artigo aqui](https://suporte.love/descobrir-cpanel/) nós\
mostramos como você pode confirmar qual é o painel do seu domínio.\
**–** As alterações realizadas, seguindo estas instruções,\
podem levar **até 24 horas** para propagar e surtir seus efeitos.

### **Acessando a conta na GoDaddy**

**Nº1–**\
[Acesse a página principal da GoDaddy](https://www.godaddy.com/pt-br).\
No canto superior direito, localize as informações mostradas na imagem abaixo,\
e clique sobre a opção **Entrar**.

![](https://suporte.love/wp-content/uploads/2020/07/Copia-de-Como-como-criar-uma-entrada-de-subdominio-na-GoDaddy\_-360035321133\_mceclip0-300x27.png)

**Nº2–** Novas opções aparecerão abaixo, em uma faixa cinza. Clique\
sobre o botão verde **Entrar**. Ele estará no quadro chamado Usuários\
registrados.

![](https://suporte.love/wp-content/uploads/2020/07/Copia-de-Como-como-criar-uma-entrada-de-subdominio-na-GoDaddy\_-360035321133\_mceclip1-300x97.png)

Na próxima tela, localize o quadro indicado na imagem abaixo.

**Nº3–** Aqui, informe o seu **nome de usuário**,\
**e-mail de acesso** ou **número do cliente**.

**Nº4–** Já aqui, informe sua **senha**.

**Nº5–** Clique em **Entrar** para acessar.

![](https://suporte.love/wp-content/uploads/2020/07/Copia-de-Como-como-criar-uma-entrada-de-subdominio-na-GoDaddy\_-360035321133\_mceclip2-290x300.png)

### **Acessando o Tela de Registros de sua Zona DNS** <a href="#h_01ffn7deh6xtxw8kb1tm46jspk" id="h_01ffn7deh6xtxw8kb1tm46jspk"></a>

**Nº6–** Na próxima tela, você verá as diversas opções de serviços\
e configurações acessíveis em sua conta. No quadro **Domínios**,\
localize o qual você deseja utilizar nas suas páginas, aqui no leadlovers (no\
exemplo, vamos usar o leadlovers.com.br). Clique no botão **DNS**,\
logo à frente dele.

![](https://suporte.love/wp-content/uploads/2020/07/Copia-de-Como-como-criar-uma-entrada-de-subdominio-na-GoDaddy\_-360035321133\_mceclip3-300x32.png)

### **Criando a Entrada de Subdomínio** <a href="#h_01ffn7dq16cf0r1exxr1abvjqg" id="h_01ffn7dq16cf0r1exxr1abvjqg"></a>

Dentro da próxima tela, chamada **Registros**, você vai ver diversas\
entradas já criadas e que direcionam o funcionamento das diversas funções de\
seu domínio.

![](https://suporte.love/wp-content/uploads/2020/07/Copia-de-Como-como-criar-uma-entrada-de-subdominio-na-GoDaddy\_-360035321133\_subdomain-godaddy-1.png)

**Nº7–** No fim da tela de Registros, abaixo do quadro das entradas,\
localize a opção **Adicionar** e clique sobre ela. Uma nova faixa\
de opções vai aparecer, que é utilizada para adição de novas entradas.

**IMPORTANTE:** nos próximos passos, utilize as imagens como apoio\
visual e confira sempre as informações inseridas. A grafia (modo de escrever)\
delas é muito importante.\
Se qualquer informação for inserida em formato diferente, ou com espaços em branco\
antes ou depois dela, pode causar falha no reconhecimento pelo sistema.

**Nº8–** Em **Tipo**, escolha a opção\
**CNAME**. As demais opções desta faixa aparecerão logo em seguida

**Nº9–** Em **Host**, coloque a palavra que você quer\
que apareça antes do domínio principal.

**EXEMPLO:** se quero que minha entrada de subdomínio seja\
**click.leadlovers.com.br**, a palavra que vou colocar tem que ser\
**click**.

**Nº10–** Em **Aponta para**, insira o número de o\
nosso servidor: **cname.leadlovers.site**

**Nº11–** Em **TTL**, escolha a opção\
**1 hora**

**Nº12–** Verifique todos os dados inseridos. O botão\
**Salvar** ficará disponível quando todos eles estiverem preenchidos.\
Clique sobre ele.

![](https://suporte.love/wp-content/uploads/2020/07/Copia-de-Como-como-criar-uma-entrada-de-subdominio-na-GoDaddy\_-360035321133\_mceclip0-1-300x96.png)

A nova entrada ficará salva, junto com as outras que já existem em sua tela de\
Registros. Ela ficará similar a esta da imagem abaixo.

![](https://suporte.love/wp-content/uploads/2020/07/Copia-de-Como-como-criar-uma-entrada-de-subdominio-na-GoDaddy\_-360035321133\_mceclip1-11-300x17.png)

Pronto! Ela está criada e corretamente apontada para o nosso servidor!

**IMPORTANTE:** Pode levar até 24 horas para as configurações sejam\
totalmente validadas na sua Hospedagem.

### **Próximos passos** <a href="#h_01ffmry545dtyhtmvjm767j5pq" id="h_01ffmry545dtyhtmvjm767j5pq"></a>

Depois de configurado o apontamento, você precisa adicionar seu subdomínio\
em sua máquina. Para maiores detalhes, [**clique aqui e veja nosso tutorial, explicando como incluir seu subdomínio em uma máquina!**](https://suporte.love/como-cadastrar-dominio-maquina/)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante\
este procedimento, por favor entre em contato com o nosso suporte!

**🏁 É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
