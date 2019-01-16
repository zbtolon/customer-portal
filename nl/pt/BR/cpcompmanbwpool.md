---

copyright:

  years: 1994, 2018

lastupdated: "2019-01-08"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Otimizando seu uso de largura da banda
{: #cp_manbdwpool}

O tráfego de rede pública de dados transferido como Saída dos data centers do IBM Cloud em todo o mundo é avaliado como encargos de Largura de banda de saída. Os encargos dependem de onde o recurso que está transferindo os dados reside, da quantia de dados que sai e de quaisquer dotações de largura de banda para as quais os produtos do IBM Cloud comprados são elegíveis.
{:shortdesc} 

Os clientes podem otimizar o uso da largura da banda "agrupando" todas as larguras de banda para os servidores em um conjunto de largura da banda. Os excedentes de largura de banda para servidores em um conjunto de largura de banda são somados como um todo e os excedentes serão calculados somente se a largura de banda total de todos os servidores exceder o total de largura de banda alocada para todos os servidores versus a medição no nível de servidor individual. 

As definições de conjunto são listadas na tabela a seguir: 

| Conjunto  | Locais          |
| ------------- |:-------------:|
| EUA    | DAL01<br/><br/>DAL02<br/><br/>DAL04<br/><br/>DAL07<br/><br/>DAL09<br/><br/>DAL10<br/><br/>DAL12<br/><br/>DAL13<br/><br/>HOU02<br/><br/>MON01<br/><br/>SEA01<br/><br/>SJC01<br/><br/>SJC03<br/><br/>SJC04<br/><br/>TOR01<br/><br/>WDC01<br/><br/>WDC04<br/><br/>WDC06<br/><br/>WDC07|
| Amsterdã e Londres | AMS01<br/><br/>AMS03<br/><br/>LON01<br/><br/>LON02<br/><br/>LON04<br/><br/>LON05<br/><br/>LON06<br/><br/>PAR01 |
| Austrália | MEL01<br/><br/>SYD01<br/><br/>SYD04<br/><br/>SYD05 |
| Brasil | SAO01 |
| Frankfurt | FRA02<br/><br/>FRA04<br/><br/>FRA05 |
| Índia | CHE01 |
| Itália | MIL01 |
| Coreia do Sul | SEO01 | 
| México | MEX01 | 
| Noruega | OSL01 | 
| Singapura, Hong Kong e Tóquio | HKG02<br/><br/>SNG01<br/><br/>TOK02<br/><br/>TOK04<br/><br/>TOK05 |
{:caption="Tabela 1. Definições de conjunto" caption-side="top"}


## Modificando um conjunto de largura da banda
{: #cp_modbdwpool}

Depois que um conjunto de largura de banda for criado, se você for um usuário autorizado, será possível acessar o conjunto a qualquer momento. É possível acessar o conjunto de largura da banda para visualizar dispositivos associados ao conjunto, incluir dispositivos no conjunto ou remover dispositivos do conjunto. Use as etapas a seguir para acessar um conjunto:

1. Efetue login no portal do cliente com as suas credenciais exclusivas.
2. Selecione **Rede** > **Largura da banda** > **Conjuntos** no menu para acessar a janela Conjuntos de largura da banda.
3. Clique no **Nome do conjunto** para acessar o conjunto. Cada dispositivo associado ao conjunto é exibido.
4. Na guia **Modificar**, é possível renomear o conjunto, incluir um dispositivo ou remover um dispositivo do conjunto:
  * Para renomear o conjunto, insira o novo nome do conjunto no campo que tem o nome do conjunto atual.
  * Para incluir um dispositivo no conjunto, na lista **Incluir servidores**, selecione o nome do dispositivo e, em seguida, clique em **Selecionar**.
  * Para remover um dispositivo de um conjunto, na lista **Remover servidores**, selecione o dispositivo e, em seguida, clique em **Selecionar**.
5. Clique em **Modificar rack**.
6. Clique no link **Visualizar todos os conjuntos de largura da banda** para retornar à janela Conjuntos de largura da banda.
