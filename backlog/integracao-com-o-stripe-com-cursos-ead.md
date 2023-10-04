# Integração com o Stripe com Cursos (EAD)

**Objetivo**: Mostrar o passo a passo de uma configuração do leadlovers com o Stripe.\
**Para que serve:** Para quem busca fazer a venda de seu infoproduto ou serviço através da plataforma Stripe e entregar o acesso ao produto dentro do EAD da leadlovers e/ou também utilizar das configurações de pós vendas para se relacionar de forma exclusiva com seus clientes.\
**Requisitos obrigatórios:**\
**1.** Este tipo de integração só pode ser feita na conta Stripe do produtor.\
**2.** É necessário já possuir um produto EAD ou Produto Integração criado dentro da leadlovers.\
**3.** Será necessário um programador para analisar a documentação e criar o checkout do seu produto, pois o Stripe não disponibiliza o checkout como outras plataformas. [Clique aqui](https://stripe.com/docs/payments/accept-a-payment) para acessar a documentação de como criar um checkout no Stripe.

### **Acessando sua conta no Stripe.**

**Nº1–** Acesse o site do Stripe clicando [aqui](https://stripe.com/br).

**Nº2–** Clique no botão **Entrar.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-11-1024x522.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-11.png)\


**Nº3–** Insira seu e-mail para login.

**Nº4–** Insira sua senha.

**Nº5–** Clique em continuar.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-12-1024x557.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-12.png)

### **Acessando o seu produto no Stripe.**

Após fazer o login, você será direcionado para essa tela:

**Nº6–** No menu lateral esquerdo, clique em **Produtos**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-3-1024x509.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-3.png)

**Nº7–** Você pode adicionar um novo produto neste momento ou **acessar um produto já existente**. Clique no produto que deseja integrar com seu produto EAD na leadlovers. Neste tutorial, o produto que iremos integrar foi criado previamente.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-4-1024x350.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-4.png)

**Nº8–** Em **Detalhes,** encontre o ID do produto e **copie este código**. Cole o código em algum lugar de fácil acesso (como um arquivo de bloco de notas, por exemplo). Vamos precisar dele mais tarde!

Mantenha esta aba aberta em seu navegador! Abra outra aba e acesse sua conta leadlovers.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/8-1024x491.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/8.png)

### **Acessando o produto EAD que será integrado ao Stripe**

**Nº9–** No menu lateral esquerdo, cliente no ícone referente a área de Produto EAD e encontre o produto que deseja integrar com o Stripe. Clique sobre ele.

**Nº10–** Clique na aba Integrações do seu produto EAD.

**Nº11–** Localize nesta página a opção de integração com o Stripe e c**opie a URL de Notificação do WebHook Stripe.** Cole a URL copiada em algum lugar de fácil acesso (como um arquivo de bloco de notas, por exemplo). Logo mais, precisaremos dela!\


Agora, **retorne à aba onde o Stripe está aberto!**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-5-1024x476.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-5.png)

### &#x20;**Criando o WebHook no Stripe**

**Nº12–** No menu lateral esquerdo, clique na opção **Desenvolvedores**.

**Nº13–** Clique em **Webhooks**.

**Nº14–** No canto superior direito, clique no botão: **Adicionar endpoint**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-6-1024x485.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-6.png)

**Nº15–** Em URL do endpoint, **cole a URL de Notificação do WebHook Stripe** que você copiou no passo 11 deste tutorial.\
\
**Nº16–** Em Eventos para enviar, **você deve selecionar qual evento** dentro do produto criado na Stripe fará a ativação deste webhook.

**Importante:** Os eventos vinculados aintegração com leadlovers são:

* **customer.subscription.deleted (ordem de pagamento deletada)**
* **customer.subscription.created (ordem de pagamento criada)**
* **invoice.payment\_failed (boleto não foi pago)**
* **invoice.payment\_succeeded (boleto foi pago)**
* **invoice.created (boleto gerado)**

Você pode escolher **mais de um evento para o mesmo Webhook**, caso deseje.

**Nº17–** Clique em **Adicionar endpoint.**

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-7-1024x495.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-7.png)

### **Copiando a API Secret Key**

Logo em seguida, você vai ser direcionado para uma tela com os **detalhes do WebHook criado**_**.**_

**Nº18–** Localize o quadro **Assinando chave secreta**. Nesta seção, clique em: **Clique para revela**r.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-8-1024x498.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-8.png)

**Nº19–** Esta é a API Secret Key. **Copie-a** e e deixe-a em algum lugar de fácil acesso (como um arquivo de bloco de notas, por exemplo).

Agora, volte de novo para a aba onde o seu produto da leadlovers está aberto.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-9.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-9.png)

### **Preenchendo dados da integração no produto**

Retorne na aba **Integrações**, dentro do seu produto e localize o quadro **Integração com Stripe**.

**Nº20–** Cole aqui o **Código ID do produto**, que salvamos no [passo 8](broken-reference) deste material.

**Nº21–** Cole aqui o **API Secret Key**, que salvamos no [passo 19](broken-reference) deste material.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-10.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/1-10.png)

**Nº22–** Confira todas as informações, vá até o fim da página e clique no botão **Salvar Integrações**.

[![](https://legado.leadlovers.site/wp-content/uploads/2020/07/22.png)](https://legado.leadlovers.site/wp-content/uploads/2020/07/22.png)

**Importante:**  Será necessário um programador para analisar a documentação e criar o checkout do seu produto, pois o Stripe não disponibiliza o checkout como outras plataformas. [Clique aqui](https://stripe.com/docs/payments/accept-a-payment) para acessar a documentação de como criar um checkout no Stripe.

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante este procedimento, por favor, **entre em contato com o nosso suporte**!

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ![❤](https://legado.leadlovers.site/wp-content/uploads/2020/09/2764.svg)\
equipe **leadlovers™**
