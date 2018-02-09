---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-04"

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

É possível gerenciar seus dispositivos no ambiente mais seguro possível usando a rede privada de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}. Quando possível, interaja com seus dispositivos usando uma conexão VPN e permita a ampliação da rede para que seus sistemas se comuniquem na rede privada. Para acessar a rede privada, edite o acesso do usuário à VPN na [Lista de Usuários ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/account/user/list){:new_window}. Use as instruções da [Rede Privada Virtual ![Ícone de link externo](../icons/launch-glyph.svg)](http://www.softlayer.com/vpn-access){:new_window} para conectar-se a uma das várias opções de VPN.

### Não deixe RDP, SSH ou portas de controle na rede pública
{: #cp_bpnordpsshcponpubnet}

A rede pública é ótima para muitas coisas, mas há certos aspectos que, quando disponibilizados na rede pública por meio de portas abertas, podem deixar seu sistema vulnerável. Proteja-se desativando o RDP ou restringindo o SSH na rede pública. Se esses serviços devem estar disponíveis na rede pública, considere mover o RDP ou o SSH para um número de porta customizado.

## Proteja seus dados por meio de backups regulares
{: #cp_bpsafedataregback}

A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} oferece diversas soluções de backup para assegurar que você possa recuperar seus dados no caso de falha da unidade ou de erro do usuário. As soluções de backup atualmente incluem NAS, EVault Backup e R1Soft CDP, que estão todos disponíveis em uma variedade de opções de armazenamento. Consulte a página [Armazenamento ![Ícone de link externo](../icons/launch-glyph.svg)](http://www.softlayer.com/services/storagelayer/){:new_window} para obter mais informações sobre cada solução de backup.

### Não suponha que você tem uma redundância; saiba que você tem
{: #cp_bpknowredundant}

A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} oferece várias redundâncias complementares, incluindo caminho duplo, fontes de alimentação redundantes e configurações RAID. Verifique se você tem provisionado um ou mais desses recursos para assegurar que você esteja trabalhando em um ambiente redundante e que esteja protegido no caso de uma falha.

### Confirme se suas informações foram submetidas a backup antes de executar um recarregamento do S.O.
{: #cp_bpnoperfOSwobackupconf}

O recarregamento de seu sistema operacional remove todos os dados do disco rígido do dispositivo. Antes de iniciar o recarregamento do S.O., faça backup de suas informações e verifique o sucesso desse backup para que nenhuma informação seja perdida. Após a conclusão de um recarregamento do S.O., as informações perdidas não poderão ser recuperadas.

## Não remova o Adaptec Storage Manager (ASM)
{: #cp_bpsupdontremovasm}

 A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} usa o ASM para monitorar o status da matriz RAID. Se você excluir esse software, a equipe de suporte não poderá monitorar seu dispositivo. Se o ASM for removido de seu dispositivo, os alertas de falha de RAID no dispositivo não ficarão disponíveis e você não será notificado da falha por meio do sistema de notificação automática.
