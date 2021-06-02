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

Trucs sur le **Serveur**

1. ✅ Tâches > Ajout de la commande d'éxécution correspondante dans chaque fichier (et pas uniquement dans README.md)
2. ✅ ansible-install-web-server/ansible/tmp/ > Transformer le dossier tmp/ en generated/
3. ✅ Maj **locales** putaing
   1. ✅ WSL
   2. ✅ Terminal
   3. ✅ Docker Desktop
   4. Maj tuto environnement de dev
      1. ✅ Terminal
      2. ✅ [Video du gars](https://www.youtube.com/watch?v=idW-an99TAM)
      3. ✅ Docker
      4. ✅ Autres
4. ✅ Connexion au serveur optimisée
5. ⏳ Date bière élèves
6. ✅ Libérer espace disque C
7. ✅ ansible-install-web-server/ansible/tmp/tests/masamune/test-wordpress--masamune--fr/generated > Transformer le dossier generated en var-files/
8. Uniformiser install/generate/init/setup
   1. core
   2. tutum/nginx
   3. wordpress
   4. Choix des mots :
      1. Etape 1 : Fichiers générés en local, puis copiés en ligne
      2. Etape 2 : Network & volumes, lancement/Mise à jour des stacks
      3. Besoin de prefixes, ex:
         1. core--reverse-proxy--traefik---step1-generate-and-upload
         2. core--reverse-proxy--traefik---step2-setup-then-start-or-update
         3. stack--wordpress--step1-generate-and-upload
         4. stack--wordpress--step2-setup-then-start-or-update
         5. stack--nginx--step1-generate-and-upload
         6. stack--wordpress--step2-setup-then-start-or-update
         7. 10-forge-a-nginx-stack # Create or modify
         8. 20-forge-a-wordpress-stack
9.  Générer tous les fichiers en local dans generated/
   5. core
      1. Maj traefik ?
   6. tutum/nginx
   7. tout en fait
10. Dupliquer les générations : 1 avec le nom de base (qui tourne), 1 avec le timestamp (historique)
11. `TASK [tests-init-hello : Edit 'test---hello--masamune--fr---tutum-hello---logs' volume content : create files & docker_peon chown 1003:1003] ***********************************************************
[DEPRECATION WARNING]: The container_default_behavior option will change its default value from "compatibility" to "no_defaults" in community.docker 2.0.0. To remove this warning, please specify an
explicit value for it now. This feature will be removed from community.docker in version 2.0.0. Deprecation warnings can be disabled by setting deprecation_warnings=False in ansible.cfg.`
11. tests-install << Renommer nginx-generate & nginx-setup
12. Clean noms containers (noms services fichiers yml :
    1. OK / test---test-wordpress--masamune--fr_mariadb.1.6u0pzz5paqai596um2b22eu1c
    2. NOK / test---hello-php--masamune--fr---tutum-hello-php_hello-php.1.
    3. .                                             ^ retarded
13. Tutum
   1. Remplacer les hardcoded par des VARIABLES, cf. wp-generate
   2. Remplacer les tutum par des nginx (afficher nom container ? :3)
      1. basique
      2. php avec un vrai exemple
14. Créer / Maj un fichier ansible de template (volume, dash, etc.) avec .j2 lié afin de **générer la stack**
   3. Avec des GROSSES_VARS genre UI_OU_PUBLIER et IMAGE_DOCKER_LOL et PORTS_PUTAINS
   4. ^ doit être prêt a décliner pour nginx, caddy & autres : nouvelle techno sur un NDD : ~2min (image, dossier hôte, url publique)
15. Mise en place d'une admin SQL > [phpmyadmin](https://hub.docker.com/_/phpmyadmin)
   5. Objectif 1 : Go tutum/hello sur pma-test-wordpress.masamune.fr
      1. 🚀 .yml indépendant
      2. .yml de test-wordpress
   6. Objectif 2 : Go pma sur pma-test-wordpress.masamune.fr
16. Rôles création d'un site
    1. Génération des fichiers .yml usuels avec arbo clients/commandes ansible à cc/etc. !
    2. Mise en place & mise à jour
       1. most recent + daté (facilite mise en place, mise a jour & historique)
       2. Création d'un rôle pour relancer/maj tous les rôles clients
    3. Arrêt de la stack
    4. Prévoir dev & prod > 1 seul script mais url change, même users & pass
    5. Création d'un utilisateur ubuntu pour connexion ssh, qui remplace ftp (clé publique privée, etc.), & suppression si fin de contrat
17. Monitoring
    1. Maj : ansible-install-web-server/ansible/3-utils-security-docker-setup.yml
    2. Mettre en place via ansible-install-web-server/ansible/4-setup-core-services.yml
    3. Alerte si CPU/RAM > 75%
    4. Checker ce qui prend de la place sur le disque ~80Go ? 13% de 450 > `docker system df -v` ; cf. backup des volumes
18. Gestion des mails propre
    1. [Conteneur postfix ?](https://hub.docker.com/_/postfixadmin)
19. Tester conteneurs de serveurs (facilité/stabilité/vitesse/http3)
    1. ✅ NDDs
    2. [Apache](https://hub.docker.com/_/httpd) / test-httpd.masamune.fr
    3. [Nginx](https://hub.docker.com/_/nginx) / test-nginx.masamune.fr
       1. Tune server for [nginx performance](https://www.nginx.com/blog/10-tips-for-10x-application-performance/)
    4. [Caddy](https://hub.docker.com/_/caddy) / test-caddy.masamune.fr
    5. Litespeed : [open](https://hub.docker.com/r/litespeedtech/openlitespeed) / [payant ?](https://hub.docker.com/r/litespeedtech/litespeed)
       1. 2-3 trucs/plugins a regarder en plus pour WP : [doc](https://www.litespeedtech.com/open-source) & [site dédié](https://lscache.io/)
       2. test-litespeed.masamune.fr
20. Bitnami
    1. [Github issues](https://github.com/bitnami/bitnami-docker-mysql/issues/79#issuecomment-545477842) > Variable d'env afin d'augmenter le debug des conteneurs bitnami ! >> raisons explicites sur le problème de boot du conteneur
    2. MARIADB_ROOT_PASSWORD_FILE: 'secret.txt'
    3. Gestion notes dans ansible-install-web-server/ansible/203-setup-wordpress-lapie_secret.yml
    4. Lourder si serveurs web classique stabilité 100%, +1 speed
    5. Activer modules php
    6. Http 2/3
21. 🌱 Automatisation des backups (volumes)
    1. [Doc volumes](server-related-tutorials/01-docker/03-develop-with-docker/02-volumes/README.md) + notes dans .md à côté
    2. Ansible
       1. Création de l'arborescence, attention au répertoire année courante
       2. Role ponctuel
       3. Génération d'un rôle lors de la création d'un site
    3. Ajout au CRON
    4. Envoi vers serveur de backup + rotation/sauvegarde incrémentielle
22. ansible-install-web-server/README.md's 🌱
23. Cleaner / Relancer clients actuels
    1. Lapie
       1. Cleaner au niveau du serveur dashed-uri > .com ou .fr
    2. Nonore
       1. (wp généré et lancement depuis ansible), Pour le moment c'est un yml lancé a l'arrache sur le serveur
    3. Backups volumes
       1. Maj ansible-install-web-server/commandes-backup-volumes-a-la-maing_secret.md (dashed notation)
       2. Backup

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
- ✅ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur mails, edt portable, favoris, bureau. Si possible description + lien.
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
- ✅ Vérifier impôts sur espace / Dernière vérif 01/06/2021
  - ✅ Perso
  - ✅ Pro
- 🚀 Maj locales / Environnement de dev / Dernière maj le 01/06/21
  - ✅ Windaube update
  - ✅ WSL
    - ✅ Version Ubuntu
      - 🚀 Si majeure, ré-effectuer [install-dev-env](https://github.com/youpiwaza/install-dev-env)
    - ✅ `sudo apt update && sudo apt upgrade`
  - ✅ Docker desktop
- ✅ Maj serveur, script maintenance
  - ✅ `98-maintenance.yml & sudo apt-get update & sudo apt upgrade & reboot si besoin`
  - ✅ Maj Lapie HMAC
- ✅ Tout est Versionné, pas de WIP qui traîne

## ⏳ En attente

- Perso > Vérifier résilation red sfr une fois repassé chez soshs
- Serveur > Corriger 98-maintenance > faire vraiment les upgrades
   1. ansible-install-web-server/ansible/roles/system-update/tasks/update-packages.yml, l. 8
   2. Besoin d'un maj de plugin pour constater le bug

### ⏳🌱 Vérifications sur la longueur

- 🌱 Impôts > Pas d'avis de CFE ?
  - Réponse par mail le 26/11/20, CA non transmis pour le moment, avis et prélèvement courant 2021
  - Toujours rien au 01/01/21
  - Toujours rien au 10/02/21
  - Toujours rien au 12/05/21
  - Site KO au 15/05/21 (maintenance ?), toujours KO le 19/05/21
  - Toujours rien au 26/05/21
  - Toujours rien au 01/06/21
- 🌱 21/05/2021 > Commande d'un hébergement ovh dédié aux picards (ovh manager > bare metal ? kimsufi) > rebasculer sur le nouveau serveur quand il sera terminé

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
      2. Basculer
2. Lapie > Traitement des tâches en souffrance
   1. Cleaner github dedié > client/url-site/
   2. Lapie > Ranger chartes graphiques & lapie-web
   3. Charte graphique > Faire les TODOs
   4. 🚚(shame) > Lapie kek.php (Crédit agricole > génération d'un fichier kek.php à la racine lors de l'insertion de clé HMAC > détruit au reboot du conteneur)
   5. Lapie, retours SEO
   6. Lapie > 🚚([Statut](https://docs.google.com/spreadsheets/d/1zZUT0F4XMQyVAFbP7ihACnRz10pmog5KoYlcaiXOGIk/edit#gid=0))
   7. ~Lapie > Maj traefik pour redirection www. > faire des tests alakon sur NDD masa avant, cf. critique
       1. Maj Ansible
   8. 🚚(shame) Accès fichiers bloqués conteneur bitnamiwp, modules php, passer en http2/3
3. Relancer impôts pro pour CFE
4. Renvoi doc AE décla 0€ années passées [hey](https://mail.google.com/mail/u/0/#inbox/FMfcgxmXKmkCGqSQkpPRbBrSKWcsbCpr)
5. CPF > Langage des signes / Amazon AWS
6. Cleaner zone DNS masamune.fr

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

Tout est priorisé :)

---
