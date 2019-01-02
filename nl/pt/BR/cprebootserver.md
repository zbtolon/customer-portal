---

copyright:

  years: 1994, 2018

lastupdated: "2017-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Reinicializando seu servidor
{: #customerportal_rebootserver}

Às vezes, ocorrem eventos na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} que requerem a reinicialização do servidor.
{:shortdesc}

Use as etapas a seguir para reiniciar o servidor:
1. No portal do cliente, clique na guia **Suporte**.
2. Clique em **Reinicializar**.
3. Selecione o servidor a ser reinicializado e clique em **Reinicializar**.
4. Selecione um dos métodos a seguir para reiniciar o servidor:
  * Padrão (tente a reinicialização com IPMI e, em seguida, com a faixa de energia)
  * IPMI
  * Cabo de alimentação
5. Clique em **Reinicializar**.

Esta página também oferece a capacidade de inicializar no kernel de resgate, o que será muito útil se você estiver tendo um problema em que o servidor não pode ser inicializado no S.O. devido a um problema de configuração. Após a inicialização no kernel de resgate, é possível montar a unidade, ou unidades, de seu servidor e, em seguida, corrigir o problema de configuração. Depois que o problema tiver sido corrigido, será possível reiniciar o servidor por meio da linha de comandos e o servidor será reiniciado no kernel padrão de seu servidor. Depois de ter emitido o comando de reinicialização, você verá um tempo estimado de conclusão.
