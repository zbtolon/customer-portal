---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-06"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Création de rapports système
{: #cp_compuschrootkit}

Vous pouvez utiliser l'outil Chrootkit pour analyser, créer et envoyer par e-mail des rapports système.
{:shortdesc}

Pour utiliser l'outil Chrootkit, utilisez d'abord SSH en tant qu'administrateur sur votre serveur. Ne vous servez pas de telnet, qui devrait déjà être désactivé. Utilisez ensuite la procédure suivante :

1. Accédez au répertoire racine (root) :  

  ```
  su -
  ```
  {: pre}

2. Exécutez la commande suivante :

  ```
  wget ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.tar.gz
  ```
  {: pre}

3. Recherchez la somme MD5 SUM du téléchargement pour la sécurité<br/

  ```
  ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.md5
  md5sum chkrootkit.tar.gz
  ```
  {: pre}

4. Décompressez le fichier compressé en utilisant la commande suivante :<br/>

  ```
  tar xvzf chkrootkit.tar.gz
  ```
  {: pre}

5. Accédez au répertoire qui vient d'être créé :

  ```
  cd chkrootkit*
  ```
  {: pre}

6. Compilez les résultats en exécutant la commande suivante :

  ```
  make sense
  ```
  {: pre}

7. Pour utiliser chkrootkit, entrez la commande suivante :

  ```
  ./chkrootkit
  ```
  {: pre}

La sortie de l'outil chkrootkit doit indiquer `not found` (introuvable) ou `not infected` (non infecté).

Si vous voyez *Checking `bindshell`... INFECTED (PORTS: 465)* et que vous exécutez PortSentry, klaxon, ou un autre programme qui s'associe aux ports inutilisés, chkrootkit risque de produire un faux positif sur le test bindshell (ports 114/tcp, 465/tcp, 511/tcp, 1008/tcp, 1524/tcp, 1999/tcp, 3879/tcp, 4369/tcp, 5665/tcp, 10008/tcp, 12321/tcp, 23132/tcp, 27374/tcp, 29364/tcp, 31336/tcp, 31337/tcp, 45454/tcp, 47017/tcp, 47889/tcp, 60001/tcp).
{: tip}

8. Changez de répertoire (`cd ..`) et retirez le fichier .gz :  

  ```
  rm chkrootkit.tar.gz
  ```
  {: pre}

## Envoi d'analyses quotidiennes automatisées
{: #cp_chrootkitdaiautscan}

Pour configurer une analyse automatisée quotidienne du système vous envoyant un rapport par e-mail, procédez comme suit :

1. En mode SSH, exécutez la commande suivante : 

  ```
  pico /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

2. Ajoutez la ligne suivante au nouveau fichier :

  ```
  #!/bin/bash<br/>
  cd /yourinstallpath/chkrootkit-0.42b/<br/>
  ./chkrootkit | mail -s "Daily chkrootkit from Servername" admin@youremail.com
  ```
  {: pre}

3. Remplacez `yourinstallpath` par le chemin réel où vous avez décomprimé Chkrootkit.
4. Remplacez `Servername` par le serveur que vous exécutez afin de savoir d'où il provient.
5. Remplacez `admin@youremail.com` par votre adresse e-mail réelle où vous souhaitez que le script vous soit envoyé.
6. Utilisez la commande suivante pour sauvegarder le fichier dans SSH :

  ```
  Ctrl+X then type Y
  ```
  {: pre}

7. Changez les droit d'accès au fichier pour pouvoir l'exécuter :

  ```
  chmod 755 /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

8.  Facultatif : vous pouvez exécuter manuellement un rapport de test dans SSH pour avoir une idée de son aspect : 

  ```
  cd /etc/cron.daily/
  ./chkrootkit.sh
  ```
  {: pre}

Vous êtes fin prêt à recevoir le rapport dans un e-mail quotidien et n'avez donc pas besoin de l'exécuter manuellement.
