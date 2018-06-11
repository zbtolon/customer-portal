---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-24"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Configuration de la connexion unique (SSO)
{: #customerportal_confssoserv}

Si vous êtes utilisateur principal d'un compte ou disposez d'un accès administrateur à ce compte, vous pouvez configurer la connexion unique. La configuration de la connexion unique pour l'infrastructure {{site.data.keyword.BluSoftlayer_full}} est un processus en deux étapes.  Dans un premier temps, vous sélectionnez et configurez votre fournisseur d'identité. Vous configurez ensuite l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} pour la réception de la demande d'authentification de votre fournisseur d'identité.
{:shortdesc}

## Sélection et configuration de votre fournisseur d'identité
{: #cp_setupidprov}

Si vous ne disposez pas déjà d'un fournisseur d'identité, commencez par en sélectionner un et le configurer. Vous pouvez utiliser les fournisseurs d'identité suivants avec {{site.data.keyword.BluSoftlayer_notm}}:
* Ping Identity&reg;,
* OneLogin&trade;,
* IBM&reg; Cloud Security Enforcer,
* IBM Cloud Identity Services.
Pour plus d'informations, contactez votre ingénieur commercial pour l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}.

Si vous ne disposez pas déjà d'un fournisseur d'identité configuré, vous pouvez contacter le support de votre fournisseur d'identité pour connaître la procédure spécifique. Vous pouvez aussi utiliser les étapes de haut niveau suivantes pour configurer votre fournisseur d'identité :
1. Préparez l'environnement de votre fournisseur d'identité en téléchargeant et en installant le fichier exécutable correspondant.
2. Configurez votre fournisseur d'identité pour une authentification avec {{site.data.keyword.BluSoftlayer_notm}}.

## Configuration de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} pour la connexion unique
{: #cp_setupsso}

Vous devez extraire les zones requises suivantes des informations de métadonnées SAML&trade; (Security Assertion Markup Language&trade;) 2.0 depuis votre fournisseur d'identité pour une utilisation avec {{site.data.keyword.BluSoftlayer_notm}}.
<dl>
<dt>ID d'entité</dt>
<dd>ID d'entité du fournisseur d'identité.</dd>
<dt>Adresse URL de connexion unique</dt>
<dd>Noeud final du fournisseur d'identité pour la connexion unique.</dd>
<dt>Certificat</dt>
<dd>Certificat du fournisseur d'identité à utiliser pour signer les demandes.</dd>
</dl>

La zone suivante est facultative :
<dl>
<dt>Empreinte de certificat</dt>
<dd>Empreinte digitale du certificat. Cette zone peut être utilisée à la place du certificat complet.</dd>
</dl>

Utilisez la procédure suivante pour configurer l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} pour la réception de la demande d'authentification de votre fournisseur d'identités :
1. Connectez-vous à votre fournisseur d'identité, si ce n'est pas déjà le cas, et accédez à la page **Configuration SAML**. Notez les informations suivantes :
  * ID d'entité
  * Adresse URL de connexion unique
  * Certificat (les exigences concernant le certificat varient en fonction du fournisseur d'identité)
2. Connectez-vous à l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} en tant qu'utilisateur principal, avec les nom d'utilisateur et mot de passe utilisés pour créer votre compte SoftLayer.
3. Cliquez sur **Compte** > **Gérer** > **Authentification SAML**.
4. Entrez les métadonnées du **Fournisseur d'identité**.
5. Cliquez sur **Enregistrer**.
6. Cliquez sur **Compte** > **Gérer** > **Authentification SAML**.
7. Cliquez sur **Télécharger la configuration XML** pour télécharger les métadonnées du fournisseur de services ou notez ces informations.
8. Utilisez les métadonnées du **Fournisseur de service** pour configurer votre fournisseur d'identité en fonction des instructions de ce dernier.  

Vous pouvez vous connecter à l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} en utilisant votre ID fédéré. Pour plus d'informations sur les ID fédérés, voir [Inscription à {{site.data.keyword.Bluemix_notm}}](/docs/account/adminpublic.html) et [IBMid Enterprise Federation Adoption Guide ![Icône de lien externe](../icons/launch-glyph.svg)](https://ibm.box.com/v/IBMid-Federation-Guide){: new_window}.
