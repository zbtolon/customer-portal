---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-30"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Protegendo seus sistemas
{: #customerportal_protsys}

A proteção de seus sistemas assegura que seus sistemas sejam executados sem problemas e sem interrupções desnecessárias.

## Use a rede privada
{: #cp_bpuseprivnet}

É possível gerenciar seus dispositivos no ambiente mais seguro possível usando a rede privada da infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}. Quando possível, interaja com seus dispositivos usando uma conexão VPN e ative a ampliação de rede para que seus sistemas se comuniquem sobre a rede privada. Para acessar a rede privada, edite o acesso do usuário à VPN na [Lista de Usuários ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/account/user/list){:new_window}. Use a lista [Rede privada virtual ![Ícone de link externo](../icons/launch-glyph.svg)](http://www.softlayer.com/vpn-access){:new_window} para se conectar a uma das várias opções de VPN.

Para obter mais informações sobre como usar uma conexão de VPN, veja [Sobre a VPN](/docs/infrastructure/iaas-vpn/about-vpn.html).

### Não deixe RDP, SSH ou portas de controle na rede pública
{: #cp_bpnordpsshcponpubnet}

A rede pública é ótima para muitas coisas, mas certos aspectos, quando disponibilizados na rede pública por meio de portas abertas, podem deixar seu sistema vulnerável. Proteja-se desativando o RDP ou restringindo o SSH na rede pública. Se esses serviços devem estar disponíveis na rede pública, considere mover o RDP ou o SSH para um número de porta customizado.

## Proteja seus dados por meio de backups regulares
{: #cp_bpsafedataregback}

Planeje backups para assegurar que seus dados sejam armazenados com segurança fora do seu dispositivo e para poder recarregá-los se forem perdidos.

A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} oferece várias soluções de backup para assegurar que você possa recuperar seus dados se a unidade falhar ou se o usuário cometer um erro. As soluções de backup atualmente incluem NAS, backup EVault e R1Soft CDP, que estão todos disponíveis em várias opções de armazenamento.
Por exemplo, é possível escolher um dos serviços de backup para armazenar seus dados em um local seguro:
  * O backup EVault é um sistema de backup automatizado e baseado em agente e uma solução popular "configurar e esquecer" para gerenciar seu dispositivo. Ele é compatível com o software Microsoft que inclui o Exchange e o SQL por meio de plug-ins. Os usuários do EVault interagem com esse serviço por meio do aplicativo baseado na web WebCC do EVault.
  * O R1Soft Continuous Data Protection (CDP) pode ser instalado em seu servidor ou na máquina virtual autogerenciada. Será possível usá-lo se estiver procurando uma única interface para gerenciar todos os seus backups. Você interage com o R1Soft CDP por meio de seu sistema de gerenciamento de proprietário, que permite que os agentes sejam instalados em máquinas virtuais e ofereça plug-ins de banco de dados para mais funções.

 Veja a página [Armazenamento ![Ícone de link externo](../icons/launch-glyph.svg)](http://www.softlayer.com/services/storagelayer/){:new_window} para obter mais informações sobre cada solução de backup e veja [Introdução aos serviços de backup](/docs/infrastructure/Backup/index.html) para obter mais informações sobre como fazer backup de seus dados.

### Não presuma que você tem redundância; saiba que você tem
{: #cp_bpknowredundant}

A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} oferece várias redundâncias complementares, que incluem caminho duplo, fontes de alimentação redundantes e configurações do RAID. Verifique se você forneceu um ou mais desses recursos para assegurar que esteja trabalhando em um ambiente redundante e de que esteja protegido se houver uma falha.

### Confirme se suas informações foram submetidas a backup antes de recarregar seu S.O.
{: #cp_bpnoperfOSwobackupconf}

Recarregar seu sistema operacional remove todos os dados do disco rígido do dispositivo. Antes de iniciar o recarregamento do S.O., faça backup de suas informações e verifique o sucesso desse backup para que nenhuma informação seja perdida. Após um recarregamento de S.O. ser concluído, as informações perdidas não poderão ser recuperadas.

## Não remova o Adaptec Storage Manager (ASM)
{: #cp_bpsupdontremovasm}

 A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} usa o ASM para monitorar o status da matriz RAID. Se você excluir esse software, a equipe de suporte não poderá monitorar seu dispositivo. Se o ASM for removido de seu dispositivo, os alertas de falha de RAID no dispositivo não ficarão disponíveis e você não será notificado da falha por meio do sistema de notificação automática.
