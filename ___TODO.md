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

## 🚀 Priorisation, simple ⏩

Indiquer ici les *tâches à effectuer en priorité*

- Si besoin de focus, mettre une ou 2 tâches ici.

PRESSE PAPIER WINDOWS > Activer l'hitorique > (windows + V)

1. Régime hyper prot
2. facture NDD [picards](https://mail.google.com/mail/u/0/#inbox/FMfcgzGkZZwLntCGLnPgcLNCzSlJVKlg)
3. Musiques taf & portable
4. amazon ["herbs pro"](https://www.amazon.com/s?me=A19497B1AUMQOH&marketplaceID=ATVPDKIKX0DER) voir pour trouver un meilleur vendeur
5. Rdv médecins
6. WP picard
   1. Facture NDD
   2. spam > virer commentaires
7. CPF
8. !site perso > cours particuliers code > 50€ heure

Trucs sur le **Serveur**

1. Activer github copilot
2. forge playbookS
   1. Optimiser script maintenance ?
   2. 🚀 Création d'un utilisateur ubuntu pour connexion ssh, qui remplace ftp (clé publique privée, etc.)
      1. ✅🔍 Docs n' tests
         1. Doc officielle
            1. [ubuntu 20 adduser/addgroup](https://manpages.ubuntu.com/manpages/focal/fr/man8/adduser.8.html)
            2. [Ubuntu 20 sshd_config](https://manpages.ubuntu.com/manpages/focal/man5/sshd_config.5.html)
            3. [ansible users](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/user_module.html)
         2. Tutos
            1. [chroot jail](https://www.tecmint.com/restrict-ssh-user-to-directory-using-chrooted-jail/)
            2. [User sftp restrict](https://www.tecmint.com/restrict-sftp-user-home-directories-using-chroot/) > #Restrict Users to a Specific Directory
            3. [Only sftp](https://geraldonit.com/2018/05/02/enabling-sftp-only-access-on-linux/)
      2. Tests
         1. 💩 Tester tutos > Besoin de clés ssh privées/publiques pour connexion avec mon setup
         2. ✅ Annuler toutes les commandes de test sur le serveur
         3. ✅ Cleaner & prioriser tâches
         4. Adapter rôle users (tester surcharger vars afin de créer un seul user)
            1. ✅ Tester sshd configuration (avant reboot sshd)
               1. `sudo sshd -t` > Si cela ne renvoit rien, c'est ok
               2. Exemple de service sshd restart : ansible\roles\security-custom-ssh-port\tasks\main.yml
               3. Mettre a jour partout, il y a ~verify pour ansible
            2. 🌱 Cleaner ansible\roles\users\tasks\restrict-user.yml
               1. Passer shell en nologin pour le peon
               2. ✅ Cleaner les commentaires
            3. 🚀 Création d'utlisateurs : ansible\roles\users\tasks\main.yml
               1. 🔍 Utilisation de loop
               2. ✅🔍 Surcharger la variable user qui alimente la boucle ?
                  1. ansible\2-generate-users-and-change-ssh-port.yml
                  2. Not in our favor [doc ansible variable precedence](https://docs.ansible.com/ansible/latest/user_guide/playbooks_variables.html#variable-precedence-where-should-i-put-a-variable)
                  3. [cheat](https://stackoverflow.com/questions/31310688/conditionally-define-variable-in-ansible#comment86310852_43403229)
               3. ✅ User default shell zsh if present
                  1. Si package zsh est la > shell zsh
               4. 🌱 User > condtionnal home folder creation
                  1. ~OK (création de l'utilisateur AVANT tâche complète + suppression de la home crée quand même..)
                  2. Besoin de faire le tuto chroot prison à la maing afin de savoir si les répertoires pourront être situés dans /docker_peon/
               5. 🚀 Faire le tuto a la maing
                  1. Afin de voir si cela fonctionne dans le répertoire /home
                  2. Afin de voir si cela fonctionne dans le répertoire /home/docker_peon
               6. Créer une nouvelle tâche conditionnelle pour les sftp
                  1. Créer un fichier `sshd_config.d/*.conf` par utilisateur fichier par utilisateur
                     1. `/etc/ssh/sshd_config.d/*.conf` files are included at the start of the configuration file, so options set there will override those in /etc/ssh/sshd_config.
                  2. Attention
                     - For file transfer sessions using SFTP no additional
                     - configuration of the environment is necessary if the in-process sftp-server is used,
                     - though sessions which use logging may require /dev/log inside the chroot directory
                     - on some operating systems (see sftp-server(8) for details).
               7. Retirer la clé ssh de bob du serveur
               8. Génération des identifiants utilisateurs
                  1. Possibilité de se baser sur
                     1. ansible\roles\users\tasks\generate-users-manual-commands.yml
                     2. ansible\roles\users\templates\ssh-users-manual-commands.md.j2
      3. Rôle ajout utilisateur sftp
      4. Rôle suppression utilisateur sftp
   3. Bind volumes pour les fichiers /www des sites
   4. Prévoir dev & prod > 1 seul script mais url change, même users & pass
       1. Utiliser docker-compose.override.yml ? [Bonnes pratiques docker/compose](https://nickjanetakis.com/blog/best-practices-around-production-ready-web-apps-with-docker-compose)
          1. Variables d'environnement dans DC
       2. Check ansible > vars d'environnement afin de maj dev. ou prod
       3. Gestion dev/prod : 1 seul fichier
       4. ENV vars ++
       5. Volumes en fonction de l'environnement ¤_¤
3. harmoniser builder guy > tout THE_BUiLDER_GUY, idem autres XXX_GUY
4. Tutum > remplacer par nginx
    1. Faire tourner déjà ca serait bien, go ctrl + f "curated"
    2. Utiliser vars d'environnement pour refaire un tutum mayzon: image + nom conteneur
5. Bitnami
    1. [Github issues](https://github.com/bitnami/bitnami-docker-mysql/issues/79#issuecomment-545477842) > Variable d'env afin d'augmenter le debug des conteneurs bitnami ! >> raisons explicites sur le problème de boot du conteneur
    2. Gestion notes dans ansible-install-web-server/ansible/203-setup-wordpress-lapie_secret.yml
    3. Lourder si serveurs web classique stabilité 100%, +1 speed
    4. Activer modules php
    5. Http 2/3
6. Mise en place d'une admin SQL > [phpmyadmin](https://hub.docker.com/_/phpmyadmin)
    1. Objectif 1 : Go nginx sur pma-test-wordpress.masamune.fr
        1. 🚀 .yml indépendant
        2. .yml de test-wordpress
    2. Objectif 2 : Go pma sur pma-test-wordpress.masamune.fr
       1. ^ Check DNS
7. Monitoring > MOD: 4-setup-core-services.yml
    1. Alternative ? [traefik pilot](https://doc.traefik.io/traefik-pilot/)
    2. Alerte si CPU/RAM > 75%
    3. Alerte si space disque libre < 20%
    4. Checker ce qui prend de la place sur le disque ~80Go ? 13% de 450 > `docker system df -v` ; cf. backup des volumes
8. Gestion des mails propre
    1. Connexion au serveur SMPT du serveur ? cf. utils-emails
    2. [Conteneur postfix ?](https://hub.docker.com/_/postfixadmin)
    3. Ajout SPF/DKIM/DMARC
    4. Maj lapie & nonore
9. Tester conteneurs de serveurs (facilité/stabilité/vitesse/http3)
    1. ✅ NDDs
       1. Need modules de cache php activés
       2. HTTP 2/3 serait un vrai plus
    2. [Apache](https://hub.docker.com/_/httpd) / test-httpd.masamune.fr
    3. [Nginx](https://hub.docker.com/_/nginx) / test-nginx.masamune.fr
       1. 🔍 [Video configuration](https://www.youtube.com/watch?v=C5kMgshNc6g)
       2. Tune server for [nginx performance](https://www.nginx.com/blog/10-tips-for-10x-application-performance/)
       3. [+1](https://blog.monitis.com/blog/6-best-practices-for-optimizing-your-nginx-performance/)
    4. [Caddy](https://hub.docker.com/_/caddy) / test-caddy.masamune.fr
    5. Litespeed : [open](https://hub.docker.com/r/litespeedtech/openlitespeed) / [payant ?](https://hub.docker.com/r/litespeedtech/litespeed)
       1. 2-3 trucs/plugins a regarder en plus pour WP : [doc](https://www.litespeedtech.com/open-source) & [site dédié](https://lscache.io/)
       2. test-litespeed.masamune.fr
    6. 🌱 Chaque serveur > Tester WP (install via wp-cli ?)
10. Cleaner / Relancer clients actuels
    1. Lapie
       1. Cleaner au niveau du serveur dashed-uri > .com ou .fr
    2. Nonore
       1. (wp généré et lancement depuis ansible), Pour le moment c'est un yml lancé a l'arrache sur le serveur
    3. Backups volumes
       1. Maj ansible-install-web-server/commandes-backup-volumes-a-la-maing_secret.md (dashed notation)
       2. (normalement d'ici la les roles de backups seront générés auto :3)
       3. Backup
11. Gestion des backups
    1. Ajout au CRON
    2. Envoi vers serveur de backup + rotation/sauvegarde incrémentielle
12. Lint done : ansible-install-web-server > README.MD
13. Ansible convenience
    1. Clean templating, variable [deprecated ansible_managed](https://docs.ansible.com/ansible/2.4/intro_configuration.html#ansible-managed)
        1. [?](https://docs.ansible.com/ansible/latest/reference_appendices/config.html#default-managed-str)
    2. [ansible prompt](https://docs.ansible.com/ansible/latest/user_guide/playbooks_prompts.html)
14. install-dev-env > docker-compose pour les principales technos : js & phpay
15. Mettre en place pour docker_peon [chroot jail](https://www.tecmint.com/restrict-ssh-user-to-directory-using-chrooted-jail/) et virer toutes les commandes

### Sinon, priorisation classique

1. Tâches récurrentes
2. Tâches en attente
3. Tâches critiques
4. Tâches WIP
5. Tâches rapides
6. Autres fichiers TODO

## ♻️ Tâches récurrentes ♻️

Tâches à *vérifier au moins une fois par semaine*, afin d'éviter un bordel plus tard/exponentiel

- ⏳ Déplacer les terminés ✅ à chaque début de semaine dans done.md
- 💩 Déplacer les TODO 🌱 dans _TODO_shame.md
- ⏳ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur ⏳ mails, ⏳ edt portable, ⏳ favoris, ⏳ bureau. Si possible description + lien.
- ⏳ Nettoyer le fichier __TODO
  - ⏳ Status
  - ⏳ Ce fichier > ### Shame
    - ⏳ Ranger dans fichiers TODO correspondant
    - ⏳ Prioriser
- ⏳ Virer ce qui traine
  - ⏳ sur le bureau
  - 💩 dans le dossier _shame du bureau
  - 💩 Lel (local)/Mes documents/_dev/_shame
  - ⏳ Vider corbeille
  - ⏳ Vider téléchargements
  - ⏳ Dans les mails
- ⏳ Déplacer veille onglets dans TODO_veille
- 💩 Ranger DD boulot
- 💩 Lel Veille / Un truc par semaine, genre le vendredi aprem, a githuber
- ⏳ Déclaration Auto entrepreneur
- ⏳ Vérifier impôts sur espace / Dernière vérif 05/07/2021
  - ⏳ Perso
  - ⏳ Pro
- ⏳ Maj locales / Environnement de dev / Dernière maj le 01/06/21
  - 🔍 CHKDSK ? -f ?
  - ⏳ Windaube update
    - ⏳ Panneau de conf > "Fichiers temporaires" > Supprimer
  - Drivers > [detection auto](https://www.touslesdrivers.com/index.php?v_page=29)
  - Firmware SSDs
  - ⏳ Nvidia driver
  - ⏳ Docker desktop (tray > icône > RC > Check for updates) / Attention, besoin de redémarrer a la main pour installation
  - ⏳ WSL
    - ⏳ Version Ubuntu
      - ⏳ Si majeure, ré-effectuer [install-dev-env](https://github.com/youpiwaza/install-dev-env)
      - ⏳ Packages & terminal, `omz update && git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade`
- ⏳ Maj serveur, script maintenance
  - ⏳ `98-maintenance.yml` & `sudo apt -y update && sudo apt --fix-broken install && sudo apt -y upgrade` & reboot si besoin
  - ⏳ Maj Lapie HMAC
- ⏳ Tout est Versionné, pas de WIP qui traîne

## ⏳ En attente

1. ⏳ Serveur > Maj WP 5.8 / Attente bitnami (5.7.2)

### ⏳🌱 Vérifications sur la longueur

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
- 🌱 21/05/2021 > Heberg picard > Basculer sur nouveau serveur & annuler

## 💥 Tâches critiques

Bug clients majeurs, interruptions de service, etc.

## 🚧 WIP 🚧

Si travail en cours, indiquer *les notes* ici

## ⚡️ Tâches rapides ✨

Indiquer ici les *tâches en dehors du flux général* (urgences, corrections process, trucs qui perturbent et doivent être fait, tâches ultra rapides, etc.)

1. Migrer ancien serveur
   1. Migrer sites une fois serveur choisi
      1. Lister
         1. Technos
         2. 📌📌📌📌📌📌📌 Fichiers
         3. BDD / Exports WordPress
         4. Basculer
2. Ranger liste de lien > première page + intro
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
9. CPF > Langage des signes / Amazon AWS

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
