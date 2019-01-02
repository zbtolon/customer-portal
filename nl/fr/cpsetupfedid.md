---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-28"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Configuration de la fédération d'identité
{: #cp_setupidfed}

Vous pouvez configurer la fédération d'identité afin d'activer un fournisseur de services tel que {{site.data.keyword.BluSoftlayer_full}} Infrastructure Management System (IMS), pour consommer les jetons de sécurité générés à partir d'un système d'identité digne de confiance à des fins d'authentification et d'autorisation.
{:shortdesc}

Vous pouvez configurer la fédération d'identité dans l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} de l'une des façons suivantes :
* Création d'utilisateurs dans le fournisseur d'identité et l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}
* Création d'utilisateurs dans le fournisseur d'identité

Un rôle définit, pour le fournisseur de services, ce que l'utilisateur est autorisé à faire (via des droits) sur le système une fois qu'il a été authentifié. Par exemple, le rôle *Utilisateur* peut être autorisé à uniquement afficher différents écrans mais pas à les mettre à jour ou ajouter.

Un rôle unique peut être affecté à plusieurs utilisateurs. De même, si un rôle dans le fournisseur d'identité mais pas dans l'infrastructure {{site.data.keyword.BluSoftlayer}}, l'utilisateur peut toujours se connecter à l'infrastructure {{site.data.keyword.BluSoftlayer}} mais il ne dispose d'aucun droit affecté à un rôle.
{: tip}


## Création d'utilisateurs dans le fournisseur d'identité et l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}
{: #cp_scenario1both}

Dans ce modèle, la procédure suivante est exécutée :
* Des utilisateurs sont créés dans le fournisseur d'identité et l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}.
* Des droits utilisateur sont affectés dans {{site.data.keyword.BluSoftlayer}} via le portail client de l'infrastructure {{site.data.keyword.BluSoftlayer}} ou des API.
* Les utilisateurs s'authentifient auprès du fournisseur d'identité et leurs données d'identification sont fédérées.
* L'infrastructure {{site.data.keyword.BluSoftlayer}} consomme les données d'identification et le contrôle d'accès est basé sur les droits définis pour l'utilisateur dans le système IMS de l'infrastructure {{site.data.keyword.BluSoftlayer}}.

Les comptes des utilisateurs ayant besoin d'accéder à l'infrastructure {{site.data.keyword.BluSoftlayer}} sont d'abord créés dans l'infrastructure {{site.data.keyword.BluSoftlayer}} avec des mots de passe aléatoires. Tous les droits doivent être configurés dans l'infrastructure {{site.data.keyword.BluSoftlayer}} pour que l'utilisateur puisse utiliser la connexion unique via le fournisseur d'identité. Actuellement, les droits sont configurés sur la base de l'utilisateur individuel.

### Configuration d'un utilisateur
Utilisez la procédure suivante pour configurer un utilisateur :

1. [Ajout d'utilisateurs à un compte SoftLayer](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct).
2. Affectez des droits dans l'infrastructure {{site.data.keyword.BluSoftlayer}}.
3. Créez des utilisateurs dans le fournisseur d'identité.

La zone **E-mail**, ou **Nom d'utilisateur** du profil d'utilisateur individuel est utilisée pour le jeton SAML&trade; (Security Assertion Markup Language&trade;) 2.0. Le jeton mappe les utilisateurs entre le fournisseur d'identité et l'infrastructure {{site.data.keyword.BluSoftlayer}}.

### Exemple de flux pour authentification de la connexion
{: #exlogauthflowidprovicloud}

L'exemple de flux suivant illustre comment l'authentification de la connexion utilisateur pourrait fonctionner lorsque vous créez des utilisateurs dans le fournisseur d'identité et l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} :
1. L'utilisateur accède à l'URL du fournisseur d'identité depuis une session de navigation.
2. Le fournisseur d'identité authentifie l'utilisateur, par exemple via LDAP.
3. Le fournisseur d'identité renvoie des réponses SAML 2.0.
4. Le fournisseur d'identité envoie une réponse SAML 2.0 au fournisseur de services, dans ce cas l'infrastructure {{site.data.keyword.BluSoftlayer}}, afin d'authentifier l'ID utilisateur.
5. L'infrastructure {{site.data.keyword.BluSoftlayer}} valide la réponse SAML 2.0.
6. L'utilisateur est connecté au portail client de l'infrastructure {{site.data.keyword.BluSoftlayer}} d'après la configuration sécurisée entre le fournisseur d'identité et l'infrastructure {{site.data.keyword.BluSoftlayer}}.


## Création d'utilisateurs dans le fournisseur d'identité
{: #cp_scenario2idp}

Dans ce modèle, les actions suivantes ont lieu :
* Des rôles sont créés dans le fournisseur d'identité et affectés à l'utilisateur.
* Des affectations de rôle et de droits sont configurées dans le système IMS de l'infrastructure {{site.data.keyword.BluSoftlayer}} via des API de l'infrastructure {{site.data.keyword.BluSoftlayer}}.
* Les utilisateurs s'authentifient auprès du fournisseur d'identité et fédèrent leurs données d'identification et attributs de rôle.
* L'infrastructure {{site.data.keyword.BluSoftlayer}} vérifie les données d'identification de l'utilisateur et les attributs de rôle. Si les rôles affectés aux utilisateurs par leur fournisseur d'identité correspondent à ceux dans l'infrastructure {{site.data.keyword.BluSoftlayer}}, des droits correspondant à ces rôles sont octroyés aux utilisateurs lorsqu'ils se connectent à l'infrastructure {{site.data.keyword.BluSoftlayer}}.
* Lorsque le fournisseur d'identité crée des utilisateurs, ceux-ci sont considérés comme fédérés vu que ces utilisateurs, ainsi que leurs rôles, sont authentifiés via SAML 2.0.

### Configuration d'un rôle pour un utilisateur
{: #cp_set-up-user-role}

Utilisez la procédure suivante pour configurer un rôle pour un utilisateur :

1. Configurez des rôles via l'API d'infrastructure {{site.data.keyword.BluSoftlayer}}.
2. Configurez des rôles dans le fournisseur d'identité.
3. Assurez-vous que les rôles définis dans l'infrastructure {{site.data.keyword.BluSoftlayer}} et le fournisseur d'identité portent le même nom.

### Configuration d'un utilisateur
{: #setupuser}

Utilisez la procédure suivante pour configurer un utilisateur :

1. Configurez des utilisateurs dans le fournisseur d'identité.
2. Affectez des rôles aux utilisateurs dans le fournisseur d'identité.

Dans ce scénario, vous n'avez pas besoin de créer manuellement des utilisateurs dans l'infrastructure {{site.data.keyword.BluSoftlayer}}.

### Exemple de flux pour authentification de la connexion utilisateur
{: #exlogauthflowidprov}

L'exemple de flux suivant illustre comment l'authentification de la connexion utilisateur pourrait fonctionner lorsque vous créez des utilisateurs dans le fournisseur d'identité :
1. L'utilisateur accède à l'URL du fournisseur d'identité depuis une session de navigation.
2. Le fournisseur d'identité authentifie l'utilisateur, par exemple via LDAP.
3. Le fournisseur d'identité renvoie des réponses SAML 2.0.
4. Le fournisseur d'identité envoie une réponse SAML 2.0 au fournisseur de services, dans ce cas l'infrastructure {{site.data.keyword.BluSoftlayer}}, afin d'authentifier le rôle utilisateur.
5. L'infrastructure {{site.data.keyword.BluSoftlayer}} valide la réponse SAML 2.0.
6. L'infrastructure {{site.data.keyword.BluSoftlayer}} redirige l'utilisateur vers le portail client.
7. L'utilisateur est connecté au portail client de l'infrastructure {{site.data.keyword.BluSoftlayer}}.

Passez en revue les procédures du fournisseur d'identité pour la configuration de nouveaux rôles et pour savoir comment les associer à l'infrastructure {{site.data.keyword.BluSoftlayer}}.
