# Enviando link de boleto por e-mail

**Objetivo:** Ensinar como enviar através da leadlovers, por e-mail, o link do boleto de pagamento para seus clientes.

### **O que é?** <a href="#o-que-e" id="o-que-e"></a>

Quando é possível contratar o seu produto utilizando Boleto como forma de pagamento, você observa que nem sempre o boleto é pago assim que emitido. Alguns clientes deixarão para pagá-lo depois, talvez na Data de Vencimento, ou precisarão confirmar com o Financeiro de suas empresas antes ou, simplesmente, esquecerão.

No momento em que um boleto é emitido, as próprias plataformas de pagamento enviam uma mensagem padrão deles, geralmente por e-mail, para o comprador com o link do boleto. Essa é uma forma do comprador conseguir localizar esse boleto mais tarde.

Mas, através da integração da plataforma de pagamento com o nosso sistema é possível personalizar essa mensagem enviada. Com o mesmo propósito – lembrar ao seu cliente que pague o boleto que está pendente – só que utilizando a comunicação característica de sua empresa.

### **Como usar?** <a href="#como-usar" id="como-usar"></a>

Antes de integrar, é preciso que a mensagem personalizada já esteja criada dentro da sua máquina.\
E para realizar a integração de forma correta, é preciso que **tenha um funil exclusivo para essa comunicação** de cobrar o pagamento de boletos.

**Nº1–** Se ainda não tem uma Máquina nesse artigo [aqui](https://www.youtube.com/watch?v=qPuUhRWVtns) mostramos como fazer.\
Caso já tenha uma máquina, você pode criar o novo funil igual ensinamos [aqui](https://suporte.love/como-criar-um-funil-e-sequencia-de-e-mails/).

**Nº2– Crie sua mensagem personalizada**. Temos [esse artigo aqui](https://suporte.love/como-criar-um-funil-e-sequencia-de-e-mails/) que mostra como criar um novo e-mail em seu funil através do Editor [Simples](https://www.youtube.com/watch?v=gVkM1eTXCFM\&list=PLtgvM3V6P-9Gi0TTr1zttfrTeSY0165sb\&index=4), mas você pode usar também o Editor [Avançado](https://www.youtube.com/watch?v=blep5ZjZocg\&list=PLtgvM3V6P-9Gi0TTr1zttfrTeSY0165sb\&index=5).

**Nº3–** No corpo da mensagem que irá disparar, na parte do texto em que deseja que o link do boleto seja inserido, **insira a tag de e-mail \*|BOLETO|\*** .\
Essa é a informação que será substituída automaticamente para o link do boleto de cada lead quando a mensagem for disparada.

Você pode inserir essa tag direto no corpo da mensagem e o link aparecerá ali, em cima de uma palavra/frase como hyperlink para o lead clicar ou no como o link de um botão.

Agora que seu funil e sua mensagem estão prontos, vamos integrá-los com a sua plataforma de pagamento externa.

### **Como integrar?** <a href="#como-integrar" id="como-integrar"></a>

Você pode integrar sua plataforma de pagamento com a leadlovers através de um [Produto EAD](broken-reference), um [Produto integrações](broken-reference) ou [via API](broken-reference).

O **Produto EAD** deve ser utilizado somente se o curso/treinamento que está vendendo estiver hospedado leadlovers.\
Caso seu curso não esteja em nosso sistema ou o produto que está comercializando não seja um treinamento e você queira integrar a plataforma de pagamento direto com sua máquina de e-mail, nesse caso, você pode usar o **Produto Integrações**.



**IMPORTANTE:**\


**–** Em ambos os Produtos, só é possível integrar a função de cobrar boletos se a sua plataforma de pagamento for a **Hotmart**, o **PagSeguro** ou a **Monetizze**.\
Os Produtos integram com várias outras ferramentas, mas, para esse objetivo específico, somente essas 3 plataformas funcionam.

**–** Com as demais plataformas de pagamento, você pode integrar [via API](broken-reference) se estas também tiverem suas APIs aberta assim como nós.

**–** A **tag \*|BOLETO|\* não funciona** nas integrações feitas pelo **ListBoss** da Hotmart e pela **Automação de leads** da Monetizze.

**–** Atualmente, essa integração só pode ser feita com Máquinas de E-mail.

#### **Produto EAD** <a href="#ead" id="ead"></a>

Como explicado acima, o EAD deve ser utilizado se for através dele que entregará o treinamento/curso que seus clientes contratarão.

Além de criar seus módulos e aulas dentro do EAD, esse Produto servirá tanto para liberar o acesso personalizado de seus alunos como para integrar com suas máquinas e apoiar no gerenciamento desses leads.

A integração da sua plataforma de pagamento deverá ser feito com o Produto EAD e então vincular este à sua máquina. O caminho será esse:

**Plataforma de pagamento → Produto EAD → Funil de Pós-Venda → Máquina**

Serão 3 níveis na integração sendo o Produto EAD o intermediador:

Seu Cliente compra seu curso → entra como Aluno no EAD criado na leadlovers → e então o Funil de Pós venda atualiza o Lead na máquina.

A atualização no lead pode ser desde inserir um novo e-mail na máquina ou até mover um lead já existente para um outro lugar (máquina ou funil) para, por exemplo, retirar o lead da comunicação onde ainda está vendando o produto e inseri-lo na comunicação de quem já comprou.

**Passo a passo**

**Nº1–** O primeiro passo é **criar o Produto EAD** em sua conta na leadlovers. Nesse artigo [aqui](https://suporte.love/nova-area-de-membros-como-criar-um-curso/) ensinamos como fazer isso.

_**Observação:**_ caso o seu Curso ainda não esteja completamente criado no EAD, recomendamos que deixe o envio automático dos dados de acesso do EAD desativado. Do contrário, assim que alguém finalizar a compra já receberá as informações para acessar seu treinamento e verá que o mesmo ainda não existe ou está incompleto.

**Nº2–** Depois será necessário que **integre a plataforma de pagamento** com o EAD.\
Aqui estão os artigos que ensinam como fazer integração com a [Hotmart](https://suporte.love/integracao-hotmart/), [PagSeguro](https://suporte.love/produtos-integracao-pagseguro/) ou [Monetizze](https://suporte.love/integracao-monetizze/).

**Nº3–** E é através dos [Funis de Pós-Vendas](https://suporte.love/funis-pos-venda/) que o EAD é vinculado à sua máquina.\
São os funis de pós-venda que adicionam ou movem o lead dentro da máquina ou aplicam Tags nesses leads, dentre outras opções.

Crie a integração do **Funil de cobrança (boleto)** com sua máquina.\
Você determinará em qual máquina e funil o lead deve entrar para receber a mensagem personalizada da cobrança do boleto.

#### **Produto Integrações** <a href="#integracoes" id="integracoes"></a>

Agora, se o seu treinamento não será hospedado em nosso sistema ou se o produto que está vendendo não é um curso não há a necessidade de criar um Produto EAD.\
Você pode criar um Produto Integrações para vincular sua plataforma de pagamento direto com a máquina. O caminho será:

**Plataforma de pagamento → Produto Integrações → Máquina**

Cliente compra o produto → e o Produto Integrações atualiza o Lead na máquina.

Repare que, diferente do EAD, agora tem mesmo um nível na integração. Não é preciso que o cliente vire um aluno para só então virar um lead.\
Logo após a compra já é feita a Ação no lead. É o equivalente à uma integração direta com a máquina.

**Passo a passo**

**Nº1–** **Crie seu Produto Integrações** igual mostramos [nesse tutorial](https://suporte.love/produto-integracao-com-produtos-externos-versao-4-0/).

**Nº2–** Apesar do layout diferente, a forma de integrar o Produto Integrações com as plataformas de pagamento externas é a mesma de como se integra com um Produto EAD.\
Nesses artigos mostramos como integrar [Hotmart](https://suporte.love/integracao-hotmart/), [PagSeguro](https://suporte.love/produtos-integracao-pagseguro/) ou [Monetizze](https://suporte.love/integracao-monetizze/) com seu Produto aqui da leadlovers.

**Nº3–** Ao invés de configurar os Funis de Pós-Venda, dentro de um Produto Integração, você irá determinar as **Configurações de Ações**.\
Novamente, mesmo com o layout diferente, conseguirá fazer as configurações necessárias igual orientamos [aqui](https://suporte.love/funis-pos-venda/).

#### **Via API** <a href="#api" id="api"></a>

Mesmo que não utilize Hotmart, PagSeguro ou Monetizze como plataforma de pagamento, ainda assim, existe uma maneira de integrar sua plataforma de pagamento conosco.

A única condição é que essa plataforma externa também tenha sua API aberta _**ou**_ uma funcionalidade de integrar com sistemas externos disponível dentro da mesma.\
Verifiquei com sua plataforma se eles possuem algo do tipo e, se sim, então o caminho será.

**Plataforma de pagamento → Máquina**

Compra realizada pelo Cliente → Lead é atualizado na máquina.

Essa sim é uma integração direta pois não há a necessidade de fazer qualquer configuração dentro da leadlovers para que a mesma funcione.

**Passo a passo**

**Nº1–** Aqui está o link da **documentação** de [nossa api](https://suporte.love/api-2/) que poderá passar ao seu programador.

**Nº2–** Em meio a documentação e dentro da categoria Lead haverá a parte do [**BilletLink**](http://apill.azurewebsites.net/#tag/BilletLink) com as informações que precisa para realizar a integração.

**Nº3–** O token que será inserido ao final do link é o **Token Pessoal** de sua conta aqui na leadlovers e, apesar de que a API ensina como fazer isso, temos esse [tutorial aqui](https://suporte.love/como-localizar-o-seu-token-pessoal-na-leadlovers/) mostrando onde obter essa informação.

**Nº4–** Com o link completo em mãos, conseguirá realizar a integração.

Explicando de uma maneira bem resumida, na hora de integrar conosco via API, esse link será inserido como uma das informações que a plataforma externa deve enviar para o nosso sistema.\
Assim como a integração associará o campo Nome com nosso “name”, deve associar o campo de Boleto com esse link.

#### **Resultado** <a href="#resultado" id="resultado"></a>

Com a integração concluída, quando a leadlovers disparar o e-mail para seu lead, ao invés de receber a Tag \*|BOLETO|\*, no corpo da mensagem constará o link do boleto próprio daquele lead.



🏁 É isso, terminamos por aqui!\
com amor ❤\
equipe leadlovers™
