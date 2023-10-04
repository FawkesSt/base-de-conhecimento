# Integração PagSeguro – Curso (EAD)

**Objetivo:** Mostrar o passo a passo de uma configuração de integração entre seu produto no leadlovers e o PagSeguro.\
**Para que serve:** Integração feita para que o cliente que fizer a compra do seu produto no PagSeguro, entre no seu Produto criado no leadlovers.\
**Requisitos Obrigatórios:** Possuir um produto criado no leadlovers e no Pagseguro.

### **Realizando a integração** <a href="#realizando-integracao" id="realizando-integracao"></a>

#### **Fazendo login em sua conta PagSeguro:** <a href="#fazendo-login" id="fazendo-login"></a>

**Nº1–** Primeiro [**acesse o PagSeguro**](https://pagseguro.uol.com.br/) e faça login em sua conta.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip0.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip0.png)

#### **Gerando e copiando código Token:** <a href="#gerando-codigo" id="gerando-codigo"></a>

**Nº2–** No menu lateral esquerdo, procure a opção **Venda Online**, e clique sobre ela.\
**Nº3–** Agora, nas opções que apareceram logo abaixo, clique sobre a opção **Integrações**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip1.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip1.png)

**Nº4–** Se for sua primeira vez gerando o **código token**, localize no lado direito o botão **Gerar token.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip2.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip2.png)

**Nº5–** O código será gerado, como mostrado na imagem. Basta copiar!

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip3.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip3.png)

**Importante:** Caso não seja a sua primeira vez gerando o código token e você já tenha botões criados, clique em **\[Enviar por e-mail]** e copie o código token que você irá receber através do e-mail de sua conta PagSeguro.

◽ É preciso **muita atenção** nesta parte! Se você clicar no botão **Gerar token** após já ter um criado, um novo código vai ser gerado e os botões que você já havia criado vão parar de funcionar, sendo necessário recriá-los e inseri-los novamente onde os utiliza atualmente.

◽ Não feche essa aba em seu navegador, abra outra e acesse sua conta LeadLovers.

#### **Acessando o produto no LeadLovers** <a href="#produto-leadlovers" id="produto-leadlovers"></a>

**Nº6–** Agora em sua conta LeadLovers clique na opção **Produtos** do menu Lateral.\
**Nº7–** Acesse o **produto** que deseja realizar a **integração**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip4.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip4.png)

#### **Gerando URL de Notificação:** <a href="#url-notificacao" id="url-notificacao"></a>

**Nº8–** Após acessar o produto na LeadLovers, clique na aba **Integrações**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip5.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip5.png)

Dentre as opções disponíveis, procure o quadro **Integração com o PagSeguro**, igual ao da imagem acima.

**Nº9–** Insira neste campo o **e-mail usado para acessar a sua conta do PagSeguro**.\
**Nº10–** Cole o **código token** de sua conta PagSeguro que você copiou no **passo 5**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip7.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip7.png)

**Nº11–** Depois de ter inserido o e-mail de sua conta e o token, clique em **Gerar URL de Notificação.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip8.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip8.png)

#### **Copiando URL de notificação** <a href="#copiando-url-notificacao" id="copiando-url-notificacao"></a>

**Nº12–** Após clicar o botão será alterando, e no campo aparecerá a **URL de Notificação**.\
Agora, só copiar!

**Observação:** A URL de notificação será **a mesma para todos os produtos**, o que mudará é o seu código de referência que será utilizado no momento de [criar o botão de vendas](broken-reference).\
[\
![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip9.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_mceclip9.png)

Salve as alterações, mas **não feche essa aba em seu navegador!**\
Mantenha estas opções abertas e **retorne para a aba do PagSeguro.**

#### **Inserindo URL de Notificação no PagSeguro** <a href="#inserindo-url-notificacao" id="inserindo-url-notificacao"></a>

Em baixo de onde gerou o seu código token, acesse a opção **Notificação de Transação**.

**Nº13–** Cole a URL de notificação que copiou no **passo 12**.\
**Nº14–** Clique em **Salvar configurações**.\
**Nº15–** Perceba que, o botão que antes estava como **Não configurado**, agora mudou para a cor **verde** e está como **Habilitado**.[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/pag-seguro-notificacao-de-transacao.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/pag-seguro-notificacao-de-transacao.png)

### **Criando o botão de vendas** <a href="#criando-botao-vendas" id="criando-botao-vendas"></a>

Integração feita! Agora, o próximo passo **é aprender a configurar o link ou botão de venda**, que encaminhará seu cliente para o **checkout do Pagseguro**. É muito importante fazer esta etapa para poder divulgar os links dos seus produtos.&#x20;

[**Clique aqui e veja o passo a passo de como criar um botão para venda rápida!**](https://suporte.love/integracao-pagseguro-botao-de-venda-rapida/)

Lembre-se de voltar a este tutorial para [testar a integração](broken-reference) assim que terminar de configurar seu botão.

**Observação:** Atualmente, não é possível integrar o Pagseguro com produtos de recorrência/assinatura.

### **Testando a Integração** <a href="#testando-integracao" id="testando-integracao"></a>

Após [criar o botão de sua preferência](https://suporte.love/integracao-pagseguro-botao-de-venda-rapida/), siga os passos abaixo para **testar a integração entre PagSeguro** e seu produto criado na leadlovers:

**A–** Acesse o seu produto e clique na aba **Integrações.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_pagseguro-botao-venda-a.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_pagseguro-botao-venda-a.png)

**B–** Localize novamente o quadro **Integração com o PagSeguro** e marque a opção **Liberar acesso na emissão do boleto** e salve as modificações.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_pagseguro-botao-venda-b.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_pagseguro-botao-venda-b.png)

**IMPORTANTE:** após a conclusão do teste, não esqueça de desabilitar esta opção.

Feita a liberação por emissão de boleto, **simule uma compra de seu produto, usando o botão de venda que foi criado mais cedo**. No método de pagamento, escolha por **boleto bancário**. Não será preciso pagar o boleto, apenas faça a emissão.

**C–** Depois de simular a compra e emitir o boleto, retorne no seu produto dentro da leadlovers e clique na aba **Clientes**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_pagseguro-botao-venda-c.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_pagseguro-botao-venda-c.png)

**D–** O e-mail usado no momento da simulação da compra deverá aparecer dentro da lista de alunos cadastrados no produto.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_pagseguro-botao-venda-d.png)](https://legado.leadlovers.site/wp-content/uploads/2020/09/produtos\_-integrao-pagseguro-360023637454\_pagseguro-botao-venda-d.png)

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, entre em contato com o nosso suporte!

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
