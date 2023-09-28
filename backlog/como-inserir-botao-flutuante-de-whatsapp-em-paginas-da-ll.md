# Como inserir botão flutuante de WhatsApp em páginas da LL?

**Atenção:** Artigo da versão 4.0 da leadlovers, disponível a partir\
de 08/06/2022.

**Objetivo:** Demonstrar como inserir um botão flutuante de\
WhatsApp em páginas da leadlovers.

Este artigo abrange os seguintes tópicos:

* [Inserindo o botão de WhatsApp que redireciona para a página do WhatsApp](broken-reference)
* [Inserindo o botão de WhatsApp, do tipo CHAT, que redireciona para a página do WhatsApp.](broken-reference)

### **Inserindo o botão de WhatsApp que redireciona para a página do WhatsApp.** <a href="#h_01fxaqtcsafdvvq7wwkwdspkje" id="h_01fxaqtcsafdvvq7wwkwdspkje"></a>

A seguir você verá como inserir um botão de WhatsApp em qualquer página da leadlovers.\
Este botão, ao ser clicado, levará o lead para a página do WhatsApp para iniciar uma conversa.\
Este procedimento pode ser realizado com todos os tipos de construtores de páginas: modelos prontos, blocos e componentes.

![](https://suporte.love/wp-content/uploads/2021/01/pagina-1-300x185.png)

\
**1 –** Acesse **a aba máquinas** e encontre a máquina que contém a página que deseja inserir o botão.

**2 –** Acesse a **máquina em questão**.

**3 –** Acesse **a aba páginas** para\
visualizar as páginas da máquina e encontrar a qual deseja editar.

**4 –** Identifique a página que deseja inserir o botão do\
whatsapp e clique no ícone de **engrenagem** para abrir\
as opções de configurações.

![](https://suporte.love/wp-content/uploads/2021/01/img-02-1.png)

**5 –** Clique em **Configurações.**

![](https://suporte.love/wp-content/uploads/2021/01/img-03-1-300x216.png)

**6 –** Clique em **Configurações Avançadas.**\
Em **Scripts do Cabeçalho (HEAD)**, insira o seguinte código:\


```
<style>
    .wpp-btn-fixo {
        position: fixed;
        bottom: 10px;
        right: 10px;
        z-index: 999999999;
    }
</style>

<div class="wpp-btn-fixo">
    <a href="https://api.whatsapp.com/send?phone=5541999999999">
        <img src="https://blob.llimages.com/machine-files/all-images/WhatsApp.svg" width="75px" height="75px" alt="Fale Conosco pelo WhatsApp" />
    </a>
</div>
```

\
&#x20;**Atente-se a mudar o telefone para o seu número de WhatsApp.**

**7 –** Clique em **Salvar**.

#### **Resultado:**

![](https://suporte.love/wp-content/uploads/2021/01/img-04-1-300x133.png)

Após realizar os procedimentos, sua página exibirá um ícone de whatsapp no canto inferior direito da página.\
Ao clicar sobre ele, o lead será direcionado para a página do whatsapp para iniciar uma conversa com seu número de whatspp.

### **Inserindo o botão de WhatsApp, do tipo CHAT, que redireciona para a página do WhatsApp.**  <a href="#h_01fxaqthw1g6kxrykq73fjsnra" id="h_01fxaqthw1g6kxrykq73fjsnra"></a>

A seguir você verá como inserir um botão de WhatsApp, do tipo CHAT, em qualquer página da leadlovers.\
Este botão, ao ser clicado, levará o lead para a página do WhatsApp para iniciar uma conversa.\
Este procedimento pode ser realizado com todos os tipos de construtores de páginas: modelos prontos, blocos e componentes.

![](https://suporte.love/wp-content/uploads/2021/01/botao-whatsapp-300x217.png)

**1 –** Acesse a opção de **Ferramentas** em sua conta. Encontra-se no canto superior direito.

**2 –** Passe o mouse sobre **Páginas** e\
selecione **Botão de WhatsApp**.

![](https://suporte.love/wp-content/uploads/2021/01/img-06-300x126.png)

Você será direcionado para essa página de configuração do gerador de chat whatsapp.

**3 –** Insira o texto do botão inicial (CTA)

**4 –** Insira o texto que será exibido na descrição do chat.

**5 –** Insira o texto que será exibido no botão para iniciar\
a conversa.

**6 –** Clique em Adicionar contato para configurar o contato\
deste chat/whatsapp.

![](https://suporte.love/wp-content/uploads/2021/01/img-07-300x124.png)\
**7 –** Na configuração do contato, você irá adicionar um **nome para o atendente deste chat**.

**8 –** Em **Foto**, você irá inserir o link\
da imagem que será exibida no chat/whatsapp, em sua página.

**9 –** Em **Número de WhatsApp**, irá inserir o seu número de whatsapp. Pois ao clicar no botão, o lead será direcionado a falar contigo e você receberá uma mensagem neste número.

**10 –** Em **Mensagem inicial da conversa no whatsap**p,\
insira o texto que deseja que aparecerá para seu lead no início da conversa.

**11 –** Clique em **Salvar atendente**.

![](https://suporte.love/wp-content/uploads/2021/01/img-08-300x122.png)

**12 –** Voltará para a página de configuração do gerador de chat.\
Agora que tudo foi configurado, clique em **Criar Chat.**

![](https://suporte.love/wp-content/uploads/2021/01/img-09-300x123.png)

**13 –** Mais uma etapa será exibida. Preencha seu nome.

**14 –** Insira seu e-mail.

**15 –** Insira seu telefone.

**16 –** Clique em **Ver código do chat.**

![](https://suporte.love/wp-content/uploads/2021/01/img-10-300x112.png)

**17 –** O código do chat configurado será exibido. **Copie este código** em\
algum lugar seguro pois iremos utiliza-lo logo mais. Um bloco de notas pode lhe\
ajudar a guardar este código.

![](https://suporte.love/wp-content/uploads/2021/01/img-11-300x126.png)

Acesse as configurações da página que deseja inserir o código do chat/whatsapp\
que acabou de criar.

**18 –** Entre nas Configurações Avançadas da página.

**19 –** Em Script do Corpo (BODY), cole o código que foi copiado\
no passo 17 deste tutorial.

**20 –** Clique em Salvar.

#### **Resultado:**

![](https://suporte.love/wp-content/uploads/2021/01/img-12-300x67.png)

Após realizar os procedimentos, sua página exibirá um ícone de whatsapp no canto inferior direito da página. Ele será exibido como um tipo de chat. O lead ao clicar em Iniciar conversa, será direcionado para a página do whatsapp para iniciar uma conversa com seu número de whatspp.

**Suporte**

Se surgir qualquer dúvida ou situação, ou se precisar de qualquer ajuda durante\
este procedimento, por favor,\
**entre em contato com o nosso suporte**!

🏁 **É isso, terminamos por aqui!**\
com\
amor ❤\
equipe **leadlovers™**
