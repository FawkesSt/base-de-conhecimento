# Integração leadlovers e MemberKit

**Objetivo:** aprender como realizar a integração entre a leadlovers e o MemberKit\
**Para que serve:** Ao integrar sua conta Memberkit, você pode gerenciar de forma automática a liberação ou bloqueio do aluno aos cursos e treinamentos hospedados nessa plataforma.\
**Requisito Obrigatório:** Possuir uma conta no MemberKit. [Clique aqui](https://memberkit.com.br/) e crie a sua.

Veremos nesse tutorial:

* Passo 1: Obter Token API
* Passo 2: Ativar a integração
* O Que Fazer a Seguir

### **Como obter o token e a Url de notificações do MemberKit**

Neste primeiro passo, você irá copiar as informações do token da MemberKit para adicionar na leadlovers.\
Obs: O token nada mais é do que uma chave de segurança que é utilizada para realizar a integração entre ferramentas.

**Copie a Chave Secreta de sua conta no MemberKit**

**N1º** – Acesse a [sua conta na Memberkit](https://memberkit.com.br/) com seu usuário e senha.

**N2º –** No menu lateral esquerdo clique em Opções avançadas > **configurações.**

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Capturar-1.png" alt="" height="382" width="342"><figcaption></figcaption></figure>

**N3º** – Na seção **Código**, copie a chave secreta (Token). Guarde esta chave para ser utilizada nos próximos passos.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_1-3-1024x566.png" alt="" height="566" width="1024"><figcaption></figcaption></figure>

**Criando a URL de notificações na sua conta no MemberKit**

**N4º** – Retorne ao menu lateral do MemberKit, e clique em **Integrações.**

**N5º** – Clique no botão **Integrar**.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_4-2-1024x178.png" alt="" height="146" width="845"><figcaption></figcaption></figure>

**N6º** – Na tela seguinte contém todas as ferramentas que podem ser integradas com a MemberKit.\
Como a leadlovers não está na lista, clique em **Webhook.**

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_5-1.png" alt="" height="301" width="361"><figcaption></figcaption></figure>

**N7º** – Na próxima tela, cole essa URL: [**https://machine.leadlovers.com/payment/sbcmk**](https://machine.leadlovers.com/payment/sbcmk)

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_6-1-1024x243.png" alt="" height="243" width="1024"><figcaption><p>Criando URL de notificação</p></figcaption></figure>

**N8º** – Após isso, logo abaixo, assinale os eventos que essa URL poderá enviar.\
**Obs:** Caso você queira enviar o lead apenas após a assinatura criada, utilize a opção “Assinatura criada”.\


Após configurar os eventos, clique em **SALVAR CONFIGURAÇÃO.**

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_7-1-1024x576.png" alt="" height="576" width="1024"><figcaption><p>Caso prefira, você poderá assinalar todos os eventos.</p></figcaption></figure>

### &#x20;**Autenticando a Integração**

Após criar a URL de notificação e copiar o token no MemberKit, é preciso realizar as configurações dentro da leadlovers.

**Área Produtos de Integração leadlovers**

**N9º** – Acesse a leadlovers, no menu lateral a esquerda, clique em **Integrações.**

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_2-1.png" alt="" height="172" width="309"><figcaption></figcaption></figure>

**N10º** – Na aba integrações, dentre as plataformas localize o **MemberKit**

**N11º** – Cole a chave secreta no campo token e clique em salvar.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_3-1-1024x586.png" alt="" height="405" width="709"><figcaption></figcaption></figure>

**N12º** Acessando a aba de **Configurações**, você poderá realizar as configurações das máquinas e funis que o membro será adicionando após compra.

Após isso, sua integração foi realizada com sucesso.

**Área Produtos EAD**

Em produtos EAD a configuração é bem similar.

**N13º** No menu lateral, acesse **Cursos online (EAD).**\
**N14º** Localize seu produto, dentro do seu produto clique na aba **Integrações.**]\
**N15º** Dentre as plataformas, localize o MemberKit.\
**N16º** Adicione a chave secreta (token) no campo em branco.\
Depois clique em Salvar.

<figure><img src="https://suporte.love/wp-content/uploads/2023/06/Screenshot_8-1-1024x641.png" alt="" height="641" width="1024"><figcaption></figcaption></figure>

#### **O Que Fazer a Seguir**

Uma vez que a integração com a Memberkit está ativa, e seus funis e máquinas estão criados.\
Você deve realizar um teste para verificar se a integração está funcionando corretamente.

**Como fazer:**

* Dentro da leadlovers, ative a opção: **Liberar acesso na emissão do boleto** e salve as configurações.
* Após isso, acesse seu produto e realize uma compra **via boleto**.
* Após alguns você deverá ser adicionado como membro dentro do seu produto EAD.
* Caso seja produto integrações, confira a máquina e funil configurados, você deverá ser\
  adicionado como lead.\
