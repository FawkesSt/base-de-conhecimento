# Avançando na segurança de e-mails: Gmail e BIMI

**Objetivo:** esclarecer futuras alterações anunciadas pelo Google sobre o BIMI.

A **Google** anunciou no último dia 12/07/2021 o suporte às configurações **BIMI**, um segmento de negócio voltado para a adoção de medidas de configurações de segurança mais rígidas que as atuais para todo o ecossistema de envios de e-mail.

As configurações **BIMI** funcionam como uma “prova de legitimidade” para quem recebe os e-mails e para os sistemas de segurança de seus provedores, aumentando a confiança no remetente desses envios e permitindo que você crie uma experiência exclusiva e mais imersiva para toda sua audiência.

“Quando configurado corretamente, os registros **BIMI** alteram a imagem de miniatura do seu envio no Gmail, fazendo com que a audiência identifique sua logo mais facilmente.”

[![](https://legado.leadlovers.site/wp-content/uploads/2021/07/gws\_bimi.gif)](https://legado.leadlovers.site/wp-content/uploads/2021/07/gws\_bimi.gif)

[![](https://legado.leadlovers.site/wp-content/uploads/2021/07/gws\_bimi\_1.gif)](https://legado.leadlovers.site/wp-content/uploads/2021/07/gws\_bimi\_1.gif)

O **BIMI** permite a todos que utilizam as configurações **DMARC** (uma configuração que por padrão já é bem rígida e permite aos sistemas um melhor controle, separando mensagens legítimas de possíveis tentativas de spam) a validação da propriedade de sua logo e a veiculação dela através do **Google** com segurança. O **BIMI** foi criado para ser fácil: organizações com o DMARC devidamente configurado vão exibir a logo de sua marca nos e-mails enviados através de seus domínios ou subdomínios.

#### **O que é o registro BIMI?**

Na tradução literal são “Indicadores de marca para identificação de mensagens” ou, na sigla em inglês, **BIMI**. É uma característica de customização de e-mail que vem crescendo em popularidade nos últimos anos, ela permite que a logo da sua marca apareça no recebimento de e-mails dos provedores que tiverem suporte a essa função. Esse registro funciona em conjunto com o registro **DMARC**, fazendo com que sua logo apareça na caixa de entrada da sua audiência.

#### **Como funciona?**

Todos que realizaram as configurações de **SPF**, **DKIM** e **DMARC** corretamente podem fornecer sua logo ao Google através de um Certificado de Marca Verificada (VMC). O BIMI faz uso de autoridades de verificação de marca, como autoridades de certificação, para aferir a propriedade do logotipo e fornecer uma “prova de certificação” em um VMC. Assim que esses e-mails autenticados passam pelos filtros de averiguação anti-spam o Gmail começa a exibir a logo no lugar do avatar do e-mail.

#### **Apenas o começo**

A iniciativa da Google espera expandir o suporte para todos os formatos e validadores.\
Atualmente, a [**Entrust**](https://www.entrust.com/newsroom/press-releases/2021/entrust-announces-general-availability-of-verified-mark-certificates-to-improve-email-authentication) e a [**DigiCert**](https://www.digicert.com/about/news/digicert-announces-availability-of-verified-mark-certificates-companies-can-add-logo-in-email-to-improve-brand-recognition-engagement) indicam o BIMI como uma autoridade de certificação e, em um futuro não muito distante, os grupos BIMI pretendem expandir essa lista, ganhando mais confiança como um órgão de validação confiável. Para mais informações sobre o grupo BIMI, visite o [**website da organização**](https://bimigroup.org/).

#### **Conclusão**

Para desfrutar das vantagens das configurações BIMI, garanta que sua organização mantenha as configurações de DMARC autenticadas e tenha sua logo validada através de um VMC.

Diversos testes de implementação ainda estão sendo realizados, visto que a função é relativamente nova e exige, além de conhecimento em zonas DNS para alteração das entradas, alguma experiência com arquivos de propriedade SVG (vetorial) e edição HTML das mesmas para alteração de versão.

Existe um [guia de implementação](https://bimigroup.org/implementation-guide/) no site oficial do grupo (em inglês).

**Fontes:**

[Advancing email security for Gmail and beyond with BIMI](https://cloud.google.com/blog/products/identity-security/bringing-bimi-to-gmail-in-google-workspace) – Google\
[BIMI Group Website](https://bimigroup.org/) – BIMI

![](https://legado.leadlovers.site/wp-content/uploads/2020/09/1f3c1.svg) **É isso, terminamos por aqui!**\
com amor ❤\
equipe **leadlovers™**
