# Como apontar domínio no Registro.br

**Objetivo:** Ensinar como fazer o apontamento de domínio no Registro.br.\
**Para que serve:** Com o [**domínio**](https://suporte.love/o-que-e-um-dominio/) apontando para a leadlovers, é possível cadastrá-lo em uma Máquina ou Produto EAD.\
**Requisitos Obrigatórios:**\
**1.** Possuir um domínio próprio comprado. **2.** Ter acesso à zona DNS do seu domínio. Confira [**aqui**](https://suporte.love/descobrir-cpanel/) como descobrir onde ele está sendo administrado.

Este artigo abrange os seguintes tópicos:

* [Apontando o domínio](broken-reference)
* [Adicionando na leadlovers](broken-reference)

### **Apontando o domínio**

**Atenção:** Se o seu domínio já está apontado para outra plataforma, realizar o processo a seguir tirará seu site externo do ar. Para manter o seu site atual como está e também usar o mesmo domínio na leadlovers, crie uma [**entrada de subdomínio**](https://suporte.love/como-como-criar-uma-entrada-de-subdominio-no-registro-br/).

**1.** Acesse o seu painel do Registro.br e clique no domínio que\
deseja configurar.

**2.** Role até o menu **DNS** e expanda a seção\
**Configurar zona DNS** (pode aparecer também como\
**Configurar endereçamento**).

Verifique se já tem dados criados, caso tenha, é de extrema importância que você abra o menu abaixo e siga o passo a passo descrito dentro dele antes de continuar.&#x20;

Se a sua zona DNS já tiver **entradas criadas**, primeiro siga à risca essas orientações:

1. Encontre a entrada do tipo **A** que o **Nome** esteja preenchido somente com o seu domínio. Copie o número de **IP** que está logo ao lado dela no campo **Dados** e salve-o no Bloco de Notas.&#x20;
2. Localize os registros do tipo **CNAME** que tem o campo **Dados** preenchido com o seu domínio, se tiver alguma informação diferente pode desconsiderar. Copie o primeiro nome de todas elas (o que vem antes do seu domínio, exemplo: **ftp**.seudominio.com) e salve no Bloco de Notas junto com o **IP** do passo anterior.
3. Exclua todas as entradas que localizou até agora, ou seja, as entradas **A** e **CNAME** que estão apontadas para o seu domínio.
4. Clique em **Nova entrada** e crie novos registros com os dados que salvou. Em **Tipo** selecione **A**, em **Nome** coloque o nome das entradas **CNAME** que guardou no passo **2** (crie uma nova entrada para cada nome salvo) e em **Endereço IPv4** insira o **IP** que salvou na etapa **1**.\
   Agora, siga para o passo **3**.

Caso esteja sem nenhum dado e essa seja a primeira vez que estiver sendo configurada, ative o **Modo Avançado** e prossiga direto para o passo **3**.

**3.** Clique em\
**Nova entrada** e\
insira os seguintes dados:

**Tipo:** A\
**Nome:** deixe este campo vazio.\
**Endereço IPv4:** 213.136.68.210

**4.** Repita o procedimento anterior e, no novo registro que estiver criando, preencha com essas informações:&#x20;

**Tipo:** A\
**Nome:** deixe este campo vazio.\
**Endereço IPv4:** 213.136.70.54

**5.** Para criar o registro **www** (assim o seu domínio\
abrirá tanto _com_ quanto _sem_ www), selecione\
**Nova Entrada** e preencha com os seguintes dados:

**Tipo:** CNAME\
**Nome:** www\
**Nome do servidor:**  insira o seu próprio domínio, sem https:// ou www. Exemplo: **dominio.com.br**

**6.** Clique em **Salvar alterações**. As entradas criadas devem ficar similares às do print abaixo.&#x20;

### **Adicionando na leadlovers**

Depois de finalizar o apontamento, aguarde pelo [**período de propagação**](https://suporte.love/como-saber-se-meu-apontamento-propagou/) e então adicione o domínio em [**sua Máquina ou Produto EAD**](https://suporte.love/como-cadastrar-dominio-maquina/).

#### **Suporte**

Se você tiver dúvidas na configuração do seu provedor, dê uma olhada se eles possuem um suporte disponível para te auxiliar. E lembre-se: você sempre pode contar conosco🥰

**🏁 É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
