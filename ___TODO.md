# Taf en cours

Légende :

- 🚀  En cours / **1 MAX A LA FOIS**
- ✅  Terminé
- ⏩  Suite
- 🚧  WIP / Work In Progress / Entamé, pas terminé
- 📌  A tester
- 🔍  Lecture/Vidéos
- 🌱  Plus tard, besoin dépendance ou flemme sur le coup
- ♻️  Récurrent
- 🚚  Contenus/notes dans les autres fichiers TODO
- 💩  KO
- ⏳ en attente
- 🤏 Petite partie

## 🧠⏫ Raccourcis & process à intégrer au flow

- Dactylo le midi > [typing study](https://www.typingstudy.com/fr/lesson/3/part/8)
- 🧠 Copier coller historique > Activer l'hitorique
  - *windows + V*
- Tétrachiée de nouveaux plugins VSCode
  - Better comments
  - Bookmarks
  - 🧠 changeCase
    - *Ctrl Shift X* > Choisir
    - *Ctrl Shift W* > Inverser
  - Code spell checker
  - TO DO Tree
  - 🧠 "Toggle quotes"
    - *Ctrl + ²*, curseur après la première de la paire de quotes à changer

## 🚀 Priorisation, simple ⏩

Indiquer ici les *tâches à effectuer en priorité*

- Si besoin de focus, mettre une ou 2 tâches ici.

Trucs **persos**

1. ⏳ Annuler [gorillaz](https://songkick.fnacspectacles.com/compteclient/detailTransaction.do?transactionId=4551758280325692730)
   1. Fnac songkick
   2. En attente de retour fnac songkick
   3. En attente retour paylogic
2. ⏳ vignette crit'air 1
   1. Commandée le 05/09/21, en attente de retour
3. ⏳ orga week end dralex
   1. Retour Angelike heberg
4. Compléments alimentaires avant le 9 septembre
   1. 💩 Manque 1 / [Solgar Phosphatidylcholine](https://www.amazon.com/your-orders/orders/ref=yo_oh_gp_to_ov?_encoding=UTF8&ref_=nav_orders_first&)
5. faire une liste too good to go > + & -
6. Mettre à jour CV !
7. Recette kir a la mûres > extraire sms guy
8. Musiques taf & portable
9. Rdv médecins
    1. Ophtalmo
    2. Cardiolog0ue
    3. Oreillologiste
10. CPF > Langage des signes / Amazon AWS
11. !site perso > cours particuliers code > 50€ heure

Trucs **taf**

1. 26 Digital
   1. ✅ Refaire au propre notes
   2. ✅ Boilerplate comptes rendus activité
      1. Envoyer au client & faire signer
      2. Envoyer à 26 Digital ~1 fois par semaine, avec % avancement mission totale
      3. Rappels/Emplois du temps
      4. 💥 28/09/2021 concert jinjer à REIMS, voir pour venir mercredi !
   3. ✅ Revoir bootstrap
   4. ✅ Faire sac
      1. ✅ Lunettes
      2. ✅ Tupperware
      3. ✅ Muffins
      4. ✅ Fringues
      5. 🌱 Douche
      6. ✅ Verre + Tasse café
      7. ✅ Masques covid
      8. ✅ Téléphone
      9. ✅ Chargeur téléphone
      10. ✅ Casque micro
   5. A voir avec tlm
      1. Questions
         1. Est-ce que le site doit être responsive ?
         2. [Échantillon de résolutions](https://supportdetails.com/) > envoi a masa
         3. Graphismes
            1. En interne ?
            2. Liberté d'adaptation ? De suggestions de compo bootstrap ?
      2. Kwaksé GIT
      3. Kwaksé environnement de dev
         1. Process de livraisons
            1. Contrôle
            2. Utilisateurs finaux : prévenir avant !
      4. can i use
   6. Dev
      1. Noter tous les contacts
      2. possibilité d'installer logiciels sur poste
      3. Mise en place du poste (vscode & autre joyeusetés)
         1. Mise à jour habituelles / cf. TODO
         2. ✅ VSCode > Settings sync ok pour github/youpiwaza
         3. ssd ?
      4. Gestion de projet > Jira/Trello ? Accès, tickets, etc.
      5. Concrètement le matos & bare metal qui fait tourner l'appli (windows server ?)
      6. Ca va tukoné ?
         1. Markdown
         2. Git
         3. Gitflow
         4. Bootstrap et toutes ses possibilités > [doc content](https://getbootstrap.com/docs/5.1/content/reboot/)
            1. Réfléchir avant chaque intégration ! Bonne pratiques + accéssibilité
            2. Annoter les maquettes afin d'homogénéiser le tout !
      7. Site dispatché sur 2 serveurs > répartition concrète des trucs
      8. Environnement de dev conteneur PHP5
         1. Voir si possibilité de migrer v8 "simplement" (test a la zob voir si bcp erreurs)
      9. Mettre en place git
      10. Mettre en place environnement de dev
          1. dev/preprod/prod
      11. Attention bootstrap officielement pas compatible avec IE (sinon voir bootstrap 4)
      12. Bonnes pratiques [html5 tags](https://getbootstrap.com/docs/5.1/content/reboot/)
          1. Si [tuto/doc](https://getbootstrap.com/docs/5.1/content/reboot/#user-input) `<kbd>`
   7. Si tout good > recommandation malt en fin de mission
2. slurp cours [3wa](https://e.3wa.fr/user/profile.php?id=2257)

Trucs pour la **migration du serveur**

1. 🚀 Bind volumes pour les fichiers /www des sites, sur les sftp créés
   1. A la mano voir si ça marche, sinon se pendre
   2. Automatiser
2. `/home/singed_the_docker_peon_9f3eqk4s9/configs/masamune/hello--masamune--fr` wtf is that
3. harmoniser builder guy > tout THE_BUiLDER_GUY, idem autres XXX_GUY
4. Tutum > remplacer par nginx
    1. Faire tourner déjà ca serait bien, go ctrl + f "curated"
    2. Utiliser vars d'environnement pour refaire un tutum mayzon: image + nom conteneur
    3. Serveur normal & serveur php basique pour les sites non wp
    4. Opti [Nginx](https://hub.docker.com/_/nginx) / test-nginx.masamune.fr
       1. 🔍 [Video configuration](https://www.youtube.com/watch?v=C5kMgshNc6g)
       2. Tune server for [nginx performance](https://www.nginx.com/blog/10-tips-for-10x-application-performance/)
       3. [+1](https://blog.monitis.com/blog/6-best-practices-for-optimizing-your-nginx-performance/)
5. Bitnami
    1. [Github issues](https://github.com/bitnami/bitnami-docker-mysql/issues/79#issuecomment-545477842) > Variable d'env afin d'augmenter le debug des conteneurs bitnami ! >> raisons explicites sur le problème de boot du conteneur
    2. Gestion notes dans ansible-install-web-server/ansible/203-setup-wordpress-lapie_secret.yml
    3. Testay avec surcharge de conf via config: voir si ca boot avec la bonne conf
    4. Lourder si serveurs web classique stabilité 100%, +1 speed
    5. Activer modules php
    6. Http 2/3
6. Gestion des mails propre
    1. Connexion au serveur SMPT du serveur ? cf. utils-emails
    2. [Conteneur postfix ?](https://hub.docker.com/_/postfixadmin)
    3. Ajout SPF/DKIM/DMARC
    4. Maj lapie & nonore
7. Maj conteneur bitnami/wordpress
8. Cleaner / Relancer clients actuels
    1. Lapie
       1. Cleaner au niveau du serveur dashed-uri > .com ou .fr
    2. Nonore
       1. (wp généré et lancement depuis ansible), Pour le moment c'est un yml lancé a l'arrache sur le serveur
    3. Backups volumes
       1. Maj ansible-install-web-server/commandes-backup-volumes-a-la-maing_secret.md (dashed notation)
       2. (normalement d'ici la les roles de backups seront générés auto :3)
       3. Backup
9. Migration serveur
   1. Lister
       1. Technos
       2. 📌📌📌📌📌📌📌 Fichiers
       3. BDD / Exports WordPress
       4. Basculer

Suite **Serveur** post migration

1. Gestion des backups
    1. Ajout au CRON
    2. Envoi vers serveur de backup + rotation/sauvegarde incrémentielle
2. Mise en place d'une admin SQL > [phpmyadmin](https://hub.docker.com/_/phpmyadmin)
    1. Objectif 1 : Go nginx sur pma-test-wordpress.masamune.fr
        1. 🚀 .yml indépendant
        2. .yml de test-wordpress
    2. Objectif 2 : Go pma sur pma-test-wordpress.masamune.fr
       1. ^ Check DNS
3. Monitoring > MOD: 4-setup-core-services.yml
    1. Alternative ? [traefik pilot](https://doc.traefik.io/traefik-pilot/)
    2. Alerte si CPU/RAM > 75%
    3. Alerte si space disque libre < 20%
    4. Checker ce qui prend de la place sur le disque ~80Go ? 13% de 450 > `docker system df -v` ; cf. backup des volumes
4. Prévoir dev & prod > 1 seul script mais url change, même users & pass
    1. Utiliser docker-compose.override.yml ? [Bonnes pratiques docker/compose](https://nickjanetakis.com/blog/best-practices-around-production-ready-web-apps-with-docker-compose)
       1. Variables d'environnement dans DC
    2. Check ansible > vars d'environnement afin de maj dev. ou prod
    3. Gestion dev/prod : 1 seul fichier
    4. ENV vars ++
    5. Volumes en fonction de l'environnement ¤_¤
5. Tester conteneurs de serveurs (facilité/stabilité/vitesse/http3)
    1. ✅ NDDs
       1. Need modules de cache php activés
       2. HTTP 2/3 serait un vrai plus
    2. [Apache](https://hub.docker.com/_/httpd) / test-httpd.masamune.fr
    3. [Caddy](https://hub.docker.com/_/caddy) / test-caddy.masamune.fr
    4. Litespeed : [open](https://hub.docker.com/r/litespeedtech/openlitespeed) / [payant ?](https://hub.docker.com/r/litespeedtech/litespeed)
       1. 2-3 trucs/plugins a regarder en plus pour WP : [doc](https://www.litespeedtech.com/open-source) & [site dédié](https://lscache.io/)
       2. test-litespeed.masamune.fr
    5. 🌱 Chaque serveur > Tester WP (install via wp-cli ?)

### Sinon, priorisation classique

1. Tâches récurrentes
2. Tâches en attente
3. Tâches critiques
4. Tâches WIP
5. Tâches rapides
6. Autres fichiers TODO

## ♻️ Tâches récurrentes ♻️

Tâches à *vérifier au moins une fois par semaine*, afin d'éviter un bordel plus tard/exponentiel

- ✅ Déplacer les terminés ✅ à chaque début de semaine dans done.md
- 💩 Déplacer les TODO 🌱 dans _TODO_shame.md
- ✅ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur ✅ mails, ✅ edt portable, ✅ favoris, ✅ bureau. Si possible description + lien.
- ✅ Nettoyer le fichier __TODO
  - ✅ Status
  - ✅ Ce fichier > ### Shame
    - ✅ Ranger dans fichiers TODO correspondant
    - ✅ Prioriser
- ✅ Virer ce qui traine
  - ✅ sur le bureau
  - 💩 dans le dossier _shame du bureau
  - 💩 Lel (local)/Mes documents/_dev/_shame
  - ✅ Vider corbeille
  - ✅ Vider téléchargements
  - ✅ Dans les mails
- ✅ Déplacer veille onglets dans TODO_veille
- 💩 Ranger DD boulot
- 💩 Lel Veille / Un truc par semaine, genre le vendredi aprem, a githuber
- ✅ Déclaration Auto entrepreneur
- ✅ Vérifier impôts sur espace / Dernière vérif 15/08/2021
  - ✅ Perso
  - ✅ Pro
- ✅ Maj locales / Environnement de dev / Dernière maj le 01/06/21
  - ✅ CHKDSK / Besoin de param `/f` ou [ne répare pas](https://docs.microsoft.com/fr-fr/windows-server/administration/windows-commands/chkdsk)
    1. Invite de commande ou Powershell **en admin**
    2. `chkdsk c: /f` (et en fonction de vos disques.. && `chkdsk d: /f`, etc.)
    3. `>Blah blah besoin de redémarrer O/n` >> `O`
    4. Redémarrer / Attendre 5 ans et demi sauf si t'as un SSD
  - ✅ Windaube update
    - ✅ [.net](https://dotnet.microsoft.com/download)
    - ✅ Panneau de conf > "Fichiers temporaires" > Supprimer
  - ✅ Drivers > [detection auto](https://www.touslesdrivers.com/index.php?v_page=29) > Lancer éxécutable, ça ouvre une page recap, et suivre liens dl
  - ✅ Firmware SSDs / Dépend du constructeur > Voir site officiel, avec un peu de chance logiciel auto alakon
    - [Sandisk ultra II](https://kb.sandisk.com/app/answers/detail/a_id/6053/~/ultra-3d-%7C-sandisk-ssd-plus-%28ssd%29-support-information)
    - Lancer (Sandisk) "Dashboard" / Firmware update automatique, et il préveitn avant. Nice
  - ✅ Docker desktop (tray > icône > RC > Check for updates) / Attention, besoin de redémarrer a la main pour installation
  - ✅ Logiciels alakon
    - ✅ Ouvrir VScode > Auto update plugins etc.
    - ✅ ~~Filezilla~~ WinSCP, OBS, VLC, ESET, [Xnview classic (Pas MP)](https://www.xnview.com/fr/xnview/#downloads)
    - ✅ Powershell [sans prise de tête](https://aka.ms/powershell-release?tag=stable) > ~`PowerShell-VERSION-win-x64.msi`.
    - ✅ Nvidia driver
      - ( [Doc](https://docs.microsoft.com/fr-fr/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-7.1) )
  - ✅ WSL
    - ✅ Version Ubuntu
      - ✅ Si majeure, ré-effectuer [install-dev-env](https://github.com/youpiwaza/install-dev-env)
    - ✅ Packages & terminal

```bash
omz update
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade
```

- ✅ Maj serveur, script maintenance
  - ✅ `98-maintenance.yml` & `sudo apt -y update && sudo apt --fix-broken install && sudo apt -y upgrade` & reboot si besoin
  - ✅ Maj Lapie HMAC
- ✅ Tout est Versionné, pas de WIP qui traîne

## ⏳ En attente

1. ⏳ Serveur > Maj WP 5.8 / Attente bitnami (5.7.2)
2. Trucs AE
   1. [hey](https://www.cominjob.com/candidat/)
   2. [hoy](https://www.ouiboss.com/)
   3. [prout](https://www.freelance-informatique.fr/)

### ⏳🌱 Vérifications sur la longueur

- Relancer Yoann Emile / Concretio-services.com pour [boulot](https://mail.google.com/mail/u/0/#inbox/FMfcgzGkbDbSHVlwFTBJKSstFTvVScJH)
- 🌱 Impôts > Pas d'avis de CFE ?
  - Réponse par mail le 26/11/20, CA non transmis pour le moment, avis et prélèvement courant 2021
  - Toujours rien au 01/01/21
  - Toujours rien au 10/02/21
  - Toujours rien au 12/05/21
  - Site KO au 15/05/21 (maintenance ?), toujours KO le 19/05/21
  - Toujours rien au 26/05/21
  - Toujours rien au 01/06/21
  - Toujours rien au 22/06/21
  - Toujours rien au 28/06/21
  - Toujours rien au 05/07/21
  - Toujours rien au 18/08/21
  - Toujours rien au 30/08/21
- 🌱 21/05/2021 > Heberg picard > Basculer sur nouveau serveur & annuler

## 💥 Tâches critiques

Bug clients majeurs, interruptions de service, etc.

## 🚧 WIP 🚧

Si travail en cours, indiquer *les notes* ici

## ⚡️ Tâches rapides ✨

Indiquer ici les *tâches en dehors du flux général* (urgences, corrections process, trucs qui perturbent et doivent être fait, tâches ultra rapides, etc.)

1. Serveur
   1. Lint done : ansible-install-web-server > README.MD
   2. Ansible convenience
       1. Clean templating, variable [deprecated ansible_managed](https://docs.ansible.com/ansible/2.4/intro_configuration.html#ansible-managed)
           1. [?](https://docs.ansible.com/ansible/latest/reference_appendices/config.html#default-managed-str)
       2. [ansible prompt](https://docs.ansible.com/ansible/latest/user_guide/playbooks_prompts.html)
   3. Opti script maintenance
      1. Ajouter maj OMZ ZSH
2. install-dev-env > docker-compose pour les principales technos : js & phpay
3. __TODO_shame.md > serveur
4. 🔍 [tmux](https://nickjanetakis.com/blog/who-else-wants-to-boost-their-productivity-with-tmux)
5. 🔍 [keys remap](https://nickjanetakis.com/blog/remap-and-set-global-hotkeys-on-windows-10-with-auto-hotkey)
6. Lapie > Traitement des tâches en souffrance
   1. Cleaner github dedié > client/url-site/
   2. Lapie > Ranger chartes graphiques & lapie-web
   3. Charte graphique > Faire les TODOs
   4. 🚚(shame) > Lapie kek.php (Crédit agricole > génération d'un fichier kek.php à la racine lors de l'insertion de clé HMAC > détruit au reboot du conteneur)
   5. Lapie, retours SEO
   6. Lapie > 🚚([Statut](https://docs.google.com/spreadsheets/d/1zZUT0F4XMQyVAFbP7ihACnRz10pmog5KoYlcaiXOGIk/edit#gid=0))
   7. ~Lapie > Maj traefik pour redirection www. > faire des tests alakon sur NDD masa avant, cf. critique
       1. Maj Ansible
   8. 🚚(shame) Accès fichiers bloqués conteneur bitnamiwp, modules php, passer en http2/3
7. Relancer impôts pro pour CFE
8. Renvoi doc AE décla 0€ années passées [hey](https://mail.google.com/mail/u/0/#inbox/FMfcgxmXKmkCGqSQkpPRbBrSKWcsbCpr)

## 💩 Shame

Parfois, l'entropie.

Emplois du temps stockés sur mail, portable, favoris, bureau.

Extraire ici puis ranger & prioriser. Doit rester vide.

---

---

Tout est extrait :)

---

### Priorisation

Ordonner puis ranger dans le flux. Doit rester vide.

---

---

Tout est priorisé :)

---
