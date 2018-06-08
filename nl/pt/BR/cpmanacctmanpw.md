---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-22"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Gerenciando senhas
{: #customerportal_manpws}

Se você for um usuário principal ou o proprietário de uma conta, será possível ativar o rastreamento de senha e você também poderá configurar uma senha para acesso único à conta. O rastreamento de senha permite que os usuários armazenem dados de senha de software para dispositivos e seu software associado.
{:shortdesc}

## Ativando o rastreamento de senha
{: #customerportal_enabpwtrak}

O portal do cliente contém uma ferramenta de [rastreamento de senha opcional ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/devices/passwords){:new_window} para cada conta. Os usuários podem recuperar seus nomes de usuário e senhas por meio da ferramenta se as informações são perdidas ou esquecidas.

As equipes de suporte também usam rastreamento de senha se o acesso remoto a um sistema é necessário. Os nomes de usuário e senhas são usados pelo Suporte somente quando necessário e autorizado para resolução de chamado.

O rastreamento de senhas no portal do cliente é opcional. Qualquer usuário com permissões apropriadas pode visualizar todas as senhas armazenadas por essa ferramenta. As informações do usuário e da senha são controladas manualmente para que não sejam sincronizadas automaticamente com um dispositivo ou seu software. Portanto, certifique-se de atualizar a ferramenta de rastreamento de senha ao mesmo tempo que atualizar usuários e senhas em dispositivos e software. Use as etapas a seguir para incluir um usuário na ferramenta de rastreamento de senha.

1. Acesse o portal do cliente usando as suas credenciais exclusivas.
2. Selecione **Dispositivos** > **Gerenciar** > **Senhas** no menu.
3. Clique na guia **Incluir credenciais**.
4. Selecione o **Nome do dispositivo** ao qual o usuário está associado na lista suspensa **Nome do dispositivo**.
5. Selecione o **Software** ao qual o usuário está associado na lista **Software**.

  O software listado é fornecido pela infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} por meio de assinaturas pagas ou gratuitas. Nenhum software de terceiros que tenha sido instalado manualmente no dispositivo está disponível para rastreamento por meio do portal do cliente.
  {: tip}

6. Insira o nome de usuário e a senha para o software nos campos correspondentes.
8. Opcionalmente, é possível inserir qualquer comentário aplicável no campo **Notas**.
9. Clique em **Incluir credenciais**.

Depois que o usuário é incluído na ferramenta de rastreamento de senha, as informações são armazenadas dentro da ferramenta até que sejam excluídas manualmente. Por padrão, todas as combinações de nome de usuário e de senha são armazenadas com base no nome do dispositivo. As entradas são exibidas alfabeticamente por nome de dispositivo, em seguida, por nome de usuário.

### Filtrando informações na ferramenta de rastreamento de senha
{: #cp_filterusinfopwtracktool}

Para visualizar, editar ou excluir informações sobre o usuário da ferramenta de rastreamento de senha, é possível filtrar para localizar rapidamente um usuário. Filtrar para localizar um usuário é útil quando a lista de usuários abrange várias linhas ou páginas. Use as etapas a seguir para filtrar por dispositivo, software ou usuário na ferramenta de rastreamento de senha.

1. Acesse o portal do cliente usando as suas credenciais exclusivas.
2. Selecione **Dispositivos** > **Gerenciar** > **Senhas** no menu.
3. Clique na guia **Filtro**.
4. Selecione ou insira o nome do dispositivo, o software ou o nome de usuário nos campos correspondentes.
5. Clique em **Filtrar**.

É possível selecionar as informações do usuário para visualizar, editar ou remover.

### Editando informações sobre o usuário na ferramenta de rastreamento de senha
{: #cp_editusinfopwtracktool}

Após a inclusão de um usuário na ferramenta de rastreamento de senha, é possível editar os detalhes associados ao usuário ou à senha. Use as etapas a seguir para editar informações para um usuário na ferramenta de rastreamento de senha.

1. Acesse o portal do cliente usando as suas credenciais exclusivas.
2. Selecione **Dispositivos** > **Gerenciar** > **Senhas** no menu.
3. Localize a combinação de usuário do dispositivo na ferramenta. Use o recurso de filtro para localizar rapidamente um usuário.
4. Clique em qualquer lugar na linha para abrir a visualização de detalhes do usuário.
5. Atualize os campos **Nome do Usuário** ou **Senha** conforme necessário.
6. Clique em **Atualizar** para salvar suas mudanças.

Depois que uma senha ou um usuário é editado na ferramenta de rastreamento de senha, as informações são atualizadas imediatamente.

## Configurando uma conta para acesso de senha descartável
{: #cp_confportacc1timpwacc}

Antes que seja possível configurar a conta, deve-se primeiro configurar o aplicativo "VIP Access" da Verisign. Se o VIP Access não estiver configurado, primeiro faça download do aplicativo para um dos dispositivos a seguir:
* Para seu telefone: [https://m.vip.symantec.com/home.v ![Ícone de link externo](../icons/launch-glyph.svg)](https://m.vip.symantec.com/home.v){:new_window}
* Para sua área de trabalho: [https://idprotect.verisign.com/desktop/download.v ![Ícone de link externo](../icons/launch-glyph.svg)](https://idprotect.verisign.com/desktop/download.v){:new_window}

Em seguida, conclua as etapas a seguir:
1. Abra o aplicativo. Localize o ID de credencial e sua senha descartável atual. É possível ignorar a senha inicialmente, mas o ID de credencial será necessário para o portal, portanto, mantenha o aplicativo aberto.
2. Efetue login no portal do cliente como o usuário para o qual você gostaria de configurar a senha descartável.
3. Clique em **Conta** > **Usuários** > **Ações** > **Incluir autenticação externa**.
4. Selecione o tipo de autenticação para incluir. Se você estiver usando o aplicativo da Verisign, escolha **Proteção de identidade da Symantect**.
5. Insira o ID de credencial da etapa 1 e clique em **Continuar**.
6. Conclua o processo de pedido e sua opção de segurança adicional será aplicada automaticamente em apenas alguns minutos.
7. Após vários minutos, selecione **Conta** > **Usuários** na barra de navegação e selecione o usuário para o qual você configurou a senha descartável.
8. Clique no link **Atualizar credencial** sob a seção **Configurações de Validação da Symantec**.
9. Selecione **ativado** para o **Estado da credencial** e clique em **Atualizar credencial**.
10. Depois que a opção de segurança adicional for processada com êxito, será possível efetuar login no portal do cliente normalmente. Depois de enviar seu nome de usuário e senha, será solicitado que insira um código de segurança.
11. Abra o aplicativo Verisign Identity Protection em seu dispositivo preferencial e forneça o código que é exibido para efetuar login.

Guarde seu ID de credencial original do Verisign Identity Protection em um local seguro para referência futura. Sem ele, não será possível acessar o portal.
