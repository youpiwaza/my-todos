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
2. ansible-install-web-server/ansible/tmp/
   1. Transformer le dossier tmp/ en generated/
3. ansible-install-web-server/ansible/tmp/tests/masamune/test-wordpress--masamune--fr/generated
   1. Transformer le dossier generated en var-files/
4. Générer tous les fichiers en local dans generated/
   1. core
   2. tutum
   3. tout en fait
5. Update hello tests
   1. ✅ New dashed notation
   2. ✅ Separate from role 4, in order to be easier to start new services, make a BP
   3. Hello php
      1. Passer en https
      2. Ajouter un exemple php
   4. Ajouter les variables sur les tests tutum + dash. C'ça qui fout la merde
      1. Voir remplacer le tutum par des nginx direct ?
   5. Créer / Maj un fichier ansible de template (volume, dash, etc.) avec .j2 lié afin de **générer la stack** ? Avec des GROSSES_VARS genre UI_OU_PUBLIER et IMAGE_DOCKER_LOL et PORTS_PUTAINS
   6. ^ doit être prêt a décliner pour nginx, caddy & autres : nouvelle techno sur un NDD : ~2min (image, dossier hôte, url publique)
6. Mise en place d'une admin SQL > [phpmyadmin](https://hub.docker.com/_/phpmyadmin)
   1. Objectif 1 : Go tutum/hello sur pma-test-wordpress.masamune.fr
      1. 🚀 .yml indépendant
      2. .yml de test-wordpress
   2. Objectif 2 : Go pma sur pma-test-wordpress.masamune.fr
7. BUG: Bitnami > Génération du wordpress : certaines variables font planter le lancement de mariaDB, voir pour trouver le mauvais caractère & l'exclure lors de la génération, cf. ansible-install-web-server/ansible/tmp/BUG VARIABLES client--picard--dev-champagne-pascal-picard-com--wordpress-stack--generated copy.yml > mariadb > environnement
8. Rôles création d'un site
   1. Génération des fichiers .yml usuels avec arbo clients/commandes ansible à cc/etc. !
   2. Mise en place & mise à jour
      1. most recent + daté (facilite mise en place, mise a jour & historique)
      2. Création d'un rôle pour relancer/maj tous les rôles clients
   3. Arrêt de la stack
   4. Prévoir dev & prod > 1 seul script mais url change, même users & pass
   5. Création d'un utilisateur ubuntu pour connexion ssh, qui remplace ftp (clé publique privée, etc.), & suppression si fin de contrat
9. Monitoring
   1. Mettre en place via ansible-install-web-server/ansible/4-setup-core-services.yml
   2. Alerte si CPU/RAM > 75%
   3. Checker ce qui prend de la place sur le disque ~80Go ? 13% de 450 > `docker system df -v` ; cf. backup des volumes
10. Gestion des mails propre
    1. [Conteneur postfix ?](https://hub.docker.com/_/postfixadmin)
11. Tester conteneurs de serveurs (facilité/stabilité/vitesse/http3)
    1. ✅ NDDs
    2. [Apache](https://hub.docker.com/_/httpd) / test-httpd.masamune.fr
    3. [Nginx](https://hub.docker.com/_/nginx) / test-nginx.masamune.fr
    4. [Caddy](https://hub.docker.com/_/caddy) / test-caddy.masamune.fr
    5. Litespeed : [open](https://hub.docker.com/r/litespeedtech/openlitespeed) / [payant ?](https://hub.docker.com/r/litespeedtech/litespeed)
       1. 2-3 trucs/plugins a regarder en plus pour WP : [doc](https://www.litespeedtech.com/open-source) & [site dédié](https://lscache.io/)
       2. test-litespeed.masamune.fr
12. Bitnami
    1. [Github issues](https://github.com/bitnami/bitnami-docker-mysql/issues/79#issuecomment-545477842) > Variable d'env afin d'augmenter le debug des conteneurs bitnami ! >> raisons explicites sur le problème de boot du conteneur
    2. MARIADB_ROOT_PASSWORD_FILE: 'secret.txt'
    3. Gestion notes dans ansible-install-web-server/ansible/203-setup-wordpress-lapie_secret.yml
    4. Lourder si serveurs web classique stabilité 100%, +1 speed
    5. Activer modules php
    6. Http 2/3
13. 🌱 Automatisation des backups (volumes)
    1. [Doc volumes](server-related-tutorials/01-docker/03-develop-with-docker/02-volumes/README.md) + notes dans .md à côté
    2. Ansible
       1. Création de l'arborescence, attention au répertoire année courante
       2. Role ponctuel
       3. Génération d'un rôle lors de la création d'un site
    3. Ajout au CRON
    4. Envoi vers serveur de backup + rotation/sauvegarde incrémentielle
14. ansible-install-web-server/README.md's 🌱
15. Cleaner / Relancer clients actuels
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
- ✅ Maj Docker desktop
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
