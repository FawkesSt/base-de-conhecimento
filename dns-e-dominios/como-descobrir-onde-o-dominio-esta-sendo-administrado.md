# Como descobrir onde o domínio está sendo administrado

Objetivo: Descobrir o Painel de Controle (cPanel) que administra o domínio atualmente.\
Para que serve: Permite localizar onde o domínio está sendo administrado para fazer configurações no lugar correto.\
Requisito obrigatório: Ter um domínio próprio já contratado.

#### Encontrando a zona DNS do seu domínio <a href="#descobrir-cpanel" id="descobrir-cpanel"></a>

Quando você tem um domínio próprio, é importante saber como localizar o seu Painel de Controle, no qual está a sua Zona de DNS atual, para poder fazer o Apontamento de Domínio ou DNS de E-mail. Nem sempre o painel está onde o domínio foi adquirido, por isso é fundamental saber localizá-lo para fazer as configurações no lugar correto. Se forem feitas alterações na Zona de DNS errada, elas não irão validar.&#x20;

Nesse tutorial utilizaremos o site [Who.is](https://who.is/) para te ensinar como descobrir o Painel de Controle do seu domínio, mas você pode usar também o [whois.com](https://www.whois.com/), o [www.godaddy.com/pt-br/whois](https://www.godaddy.com/pt-br/whois), ou o localizador de sua preferência. Caso o seu domínio seja .br ou .pt, você pode utilizar o WhoIs específico da [RegistroBR](https://registro.br/tecnologia/ferramentas/whois/?search=) ou o de [Portugal](https://www.dns.pt/pt/ferramentas/).&#x20;

Nº1–  Acesse a ferramenta [Who.is](https://who.is/) de sua preferência.

Nº2– Digite somente o seu domínio na ferramenta de busca. Sem o http:// ou https:// no início do link e sem a / no final.

![](https://legado.leadlovers.site/wp-content/uploads/2017/07/Tutorial\_Nameserver\_-\_1.png)

#### Identificando o Painel de Controle <a href="#identificar-cpanel" id="identificar-cpanel"></a>

Nº3– Localize os Name Servers, essa é a informação que indica onde a zona DNS do domínio está sendo administrada atualmente (caso esteja utilizando o WhoIs da RegistroBR, localize os Servidores DNS).

Observação: Caso o seu domínio esteja em transição, ou seja, se você estiver migrando o gerenciamento de um Painel de Controle para o outro, o Name Server só atualizará quando a migração for concluída.&#x20;

Nº4– Identifique de qual Painel de Controle são os Name Servers. Isso significa que, sempre que quiser fazer alguma configuração na zona DNS de seu domínio, deve fazer de acordo com o Painel de Controle atual que os Name Servers estiverem indicando, nesse caso, seria o Cloudflare.

![](https://legado.leadlovers.site/wp-content/uploads/2017/07/Tutorial\_Nameserver\_-\_2.png)

Nº 5– Há alguns Painéis de Controle que são mais difíceis de identificar quais são somente olhando os Name Server, como no exemplo abaixo.

![](https://legado.leadlovers.site/wp-content/uploads/2017/07/Tutorial\_Nameserver\_-\_3.png)

Nº 6– Se não conseguir identificar onde está o Painel de Controle quando encontrar os Name Servers, uma rápida pesquisa no Google deve te informar de onde eles são. No exemplo que trouxemos, identificamos que os Name Servers ns1.dns-parking.com e ns2.dns-parking.com são da Hostinger.&#x20;

![](https://legado.leadlovers.site/wp-content/uploads/2017/07/Tutorial\_Nameserver\_-\_4.png)

#### Lista de Name Servers <a href="#lista" id="lista"></a>

Para facilitar, nós trouxemos uma lista atualizada dos Name Servers e seus respectivos Painéis de Controle mais conhecidos:

* RegistroBR: b.sec.dns.br, c.sec.dns.br
* Cloudflare: exemplo.ns.cloudflare.com, exemplo.ns.cloudflare.com
* **HostGator:** ns01.hostgator.com.br, ns02.hostgator.com.br
* **GoDaddy:** ns51.domaincontrol.com, ns52.domaincontrol.com
* **Locaweb:** ns1.locaweb.com.br, ns2.locaweb.com.br, ns3.locaweb.com.br
* Hostinger hPanel: ns1.dns-parking.com, ns2.dns-parking.com
* Hostinger cPanel: cdns1.main-hosting.eu, cdns2.main-hosting.eu
* **KingHost:** dns1.kinghost.com.br, dns2.kinghost.com.br, dns3.kinghost.com.br, dns4.kinghost.com.br, dns5.kinghost.com.br, dns6.kinghost.com.br
* Uolhost: ns1.dominios.uol.com.br, ns2.dominios.uol.com.br, ns3.dominios.uol.com.br\

* **Builderall:** ns1.l4dns.com, ns2.l4dns.com, ns3.l4dns.com, ns4.l4dns.com
* Amazon: ns-2048.awsdns-64.com, ns-2049.awsdns-65.net, ns-2050.awsdns-66.org, ns-2051.awsdns-67.co.uk
* Weblink: cdns1.weblink.com.br, cdns2.weblink.com.br
* **ValueHost:** ns1.valueserver.com.br, ns2.valueserver.com.br, ns3.valueserver.com.br, ns4.valueserver.com.br

Agora que você conseguiu localizar o seu domínio, sabe em qual Painel de Controle está a sua Zona de DNS!&#x20;

**Artigos Sugeridos**

– Se você caiu aleatoriamente aqui e não sabe o que é um domínio e nem como pode usá-lo dentro do nosso sistema, veja primeiro este artigo: [o que é um domínio](../backlog/o-que-e-um-dominio.md).

– Confira os nossos tutoriais de como fazer os apontamentos de [domínio](apontamento-de-dominio/), ou [subdomínio](../backlog/como-apontar-subdominio-no-registro.br.md).

– Aprenda como realizar as configurações de [DNS de E-mail.](dns-de-email/)

