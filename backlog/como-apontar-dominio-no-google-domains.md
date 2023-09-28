# Como apontar domínio no Google Domains

**Objetivo:** Ensinar como fazer o apontamento de domínio no Google Domains.\
**Para que serve:** Com o [**domínio**](https://suporte.love/o-que-e-um-dominio/) apontando para a leadlovers, é possível cadastrá-lo em uma Máquina ou Produto EAD.\
**Requisitos Obrigatórios: 1.** Possuir um domínio próprio comprado. **2.** Ter acesso à zona DNS do seu domínio. Confira [**aqui**](https://suporte.love/descobrir-cpanel/) como descobrir onde ele está sendo administrado.

### **Apontando o domínio** <a href="#apontando-dominio" id="apontando-dominio"></a>

**Atenção:** Se o seu domínio já está apontado para outra plataforma, realizar o processo a seguir tirará seu site externo do ar. Para manter o seu site atual como está e também usar o mesmo domínio na leadlovers, crie uma [**entrada de subdomínio**](https://suporte.love/como-apontar-subdominio-no-google-domains/).

**1.** Acesse o seu painel do Google Domains e clique no menu **DNS**.

**2.** Expanda a seção **Registros personalizados** e verifique se já tem dados criados em sua Zona DNS. Caso tenha, é de extrema importância\
que você abra o menu abaixo e siga o passo a passo descrito dentro dele antes de continuar.&#x20;

Se a sua zona DNS já tiver **entradas criadas**, primeiro siga à risca essas orientações:

1. Encontre a entrada do tipo **A**\
   que o **Nome do Host** esteja preenchido somente com o seu domínio. Copie o número de **IP** que está logo ao lado dela no campo **Dados** e salve-o no Bloco de Notas.&#x20;
2. Localize os registros do tipo **CNAME**\
   que tem o campo **Dados** preenchido com o seu domínio, se tiver alguma informação diferente pode desconsiderar. Copie o primeiro nome de todas elas (o que vem antes do seu domínio, exemplo: **ftp**.seudominio.com) e salve no Bloco de Notas junto com o IP do passo anterior.
3. Exclua todas as entradas que localizou até agora, ou seja, as entradas **A** e **CNAME**\
   que estão apontadas para o seu domínio.
4. Crie novos registros com os dados que salvou. Em **Nome do Host** coloque o nome das entradas **CNAME** que guardou no passo **2** (crie um registro novo para cada entrada salva), em **Tipo** selecione **A**, em **TTL** preencha o valor **14400** e em **Dados** insira o **IP** que salvou na etapa **1**.\
   Agora,\
   siga para o passo\
   [**3**](broken-reference).

Caso a zona DNS esteja sem nenhum dado, prossiga direto para o passo [**3**](broken-reference).&#x20;

**3.** Crie um novo registro com os seguintes dados:

**Nome do host:** deixe o espaço vazio.\
**Tipo:** A\
**TTL:** 14400\
**Dados:** 213.136.68.210

**4.** Ainda com o registro aberto, clique logo abaixo na opção **+ Adicionar mais campos neste registro** e insira o também IP **213.136.70.54**. Salve as alterações.

![img01.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6489074324493/img01.png)

**5.** Para criar a entrada\
**www** (assim o seu domínio abrirá tanto _com_ quanto\
_sem_ www), clique em **Criar novo registro** e preencha\
com os seguintes dados:

**Nome do host:** www\
**Tipo:** CNAME\
**TTL:** 14400\
**Dados:** insira o seu próprio domínio, sem https:// ou www. Exemplo: **dominio.com.br**

**6.** Salve as configurações.

**7.** As entradas criadas devem ficar similares às do print abaixo. Para editá-las, clique em **Gerenciar registros personalizados**.

![img02.png](https://leadloverssupport.zendesk.com/hc/article\_attachments/6489298958221/img02.png)

### **Adicionando na leadlovers** <a href="#adicionando-leadlovers" id="adicionando-leadlovers"></a>

Depois de finalizar o apontamento, aguarde pelo [**período de propagação**](https://suporte.love/como-saber-se-meu-apontamento-propagou/) e então adicione o domínio em [**sua Máquina ou Produto EAD**](https://suporte.love/como-cadastrar-dominio-maquina/).

#### **Suporte**

Se você tiver dúvidas na configuração do seu provedor, dê uma olhada se eles possuem um suporte disponível para te auxiliar. E lembre-se: você sempre pode contar conosco**🥰**

**🏁 É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
