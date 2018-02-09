---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-05"

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

Use as etapas a seguir para reinicializar o servidor:
1. No portal do cliente, clique na guia **Suporte**.
2. Clique em **Reinicializar**.
3. Selecione o servidor a ser reinicializado e clique em **Reinicializar**.
4. Selecione um dos métodos a seguir para reinicializar o servidor:
  * Padrão (tentar a reinicialização com IPMI e, em seguida, com o cabo de alimentação)
  * IPMI
  * Cabo de alimentação
5. Clique em reinicializar.

Essa página também oferece a capacidade de inicialização no kernel de resgate, que é muito útil se você está tendo um problema no qual o servidor não pode inicializar no S.O. devido a um problema de configuração. Após a inicialização no kernel de resgate, é possível montar a unidade, ou unidades, de seu servidor e, em seguida, corrigir o problema de configuração. Depois que o problema tiver sido corrigido, será possível reinicializar o servidor da linha de comandos e o servidor será reinicializado no kernel padrão para seu servidor. Depois de ter emitido o comando de reinicialização, você verá um tempo estimado de conclusão.
