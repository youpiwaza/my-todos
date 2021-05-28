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

1. Tâches serveur > Passe de 'done.md' au 'serveur > README.md'
2. 🚀 Backup nouveau serveur (volumes containers)
   1. ✅ Lapie > All in one WP Migration
   2. ✅ Tests backup volume > .tar
      1. [Doc volumes](server-related-tutorials/01-docker/03-develop-with-docker/02-volumes/README.md)
   3. 💩 Tests [archivage incrémentiel](https://doc.ubuntu-fr.org/tar#utilisation_en_archivage_incrementiel)
      1. Test sur fichier alakon
      2. Test sur fichier alakon dans volume
      3. KO / --listed-incremential not found dans `tar`
   4. 🚀 Cleaner backup
      1. ✅ Mettre nom, date & heure dans le nom de fichier de la sauvegarde
         1. `nom-volume---backup---$(date +%Y-%m-%d--%H.%M.%S).tar`
      2. ✅ Contenu de l'archive propre : 1 seul dossier bien nommé
      3. ✅ Bien le ranger sur l'hôte (emplacement à choisir + maj ansible-install-web-server/nomenclature-and-folder-tree.md)
         1. Les volumes sont liés aux conteneurs, mais contenu sensible (!DOCKER_PEON) > dans le dossier de DOCKER_GUY/
         2. Arbo logique ek details `DOCKER_GUY/backups/volumes/clients/LE_CLIENT/SITE_COM/ANNEE/nom-volume---backup---$(date +%Y-%m-%d--%H.%M.%S).tar`
         3. Mais, les noms de volumes ont de l'info, ex : `client---dev--masamune-fr---wordpress--db`, mais les sauvegardes seront récurrentes (vite le bordel si beaucoup de fichiers)
         4. `DOCKER_GUY/backups/volumes/ANNEE/TYPE/LE_CLIENT/SITE_COM/nom-volume---backup---$(date +%Y-%m-%d--%Hh%Mm%Ss).tar`
         5. Eg. `DOCKER_GUY/backups/volumes/2021/clients/masamune/dev--masamune--fr/client---dev--masamune--fr---wordpress--db---backup---2021-05-27--11h23m57s.tar`
      4. 🚀 Documenter
         1. ✅ Fichier de commandes usuelles, pour sauvegarde manuelle
         2. 🚀 Maj de l'arborescence du serveur
   5. Faire les backups des volumes en prod
      1. SSH > récupérer les archives en local/github
   6. Ajouter note/faire ansible

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
- x Déplacer les TODO 🌱 dans _TODO_shame.md

- ✅ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur mails, edt portable, favoris, bureau. Si possible description + lien.
- ✅ Nettoyer le fichier __TODO
  - ✅ Status
  - ✅ Ce fichier > ### Shame
    - ✅ Ranger dans fichiers TODO correspondant
    - ✅ Prioriser
- ✅ Virer ce qui traine
  - ⏳ sur le bureau
  - 💩 dans le dossier _shame du bureau
  - 💩 Lel (local)/Mes documents/_dev/_shame
  - ✅ Vider corbeille
  - ✅ Vider téléchargements
  - ✅ Dans les mails
- ✅ Déplacer veille onglets dans TODO_veille
- 💩 Ranger DD boulot
- 💩 Lel Veille / Un truc par semaine, genre le vendredi aprem, a githuber
- ✅ Déclaration Auto entrepreneur
- ✅ Vérifier impôts sur espace / Dernière vérif 19/05/2021
  - ✅ Perso
  - ✅ Pro
- ✅ Maj serveur, script maintenance
  - ✅ `98-maintenance.yml & sudo apt-get update & sudo apt upgrade & reboot si besoin`
  - ✅ Maj Lapie HMAC
- ⏳ Tout est Versionné, pas de WIP qui traîne

## ⏳ En attente

Rieng

### ⏳🌱 Vérifications sur la longueur

- 🌱 Impôts > Pas d'avis de CFE ?
  - Réponse par mail le 26/11/20, CA non transmis pour le moment, avis et prélèvement courant 2021
  - Toujours rien au 01/01/21
  - Toujours rien au 10/02/21
  - Toujours rien au 12/05/21
  - Site KO au 15/05/21 (maintenance ?), toujours KO le 19/05/21
  - Toujours rien au 26/05/21
- 🌱 21/05/2021 > Commande d'un hébergement ovh dédié aux picards (ovh manager > bare metal ? kimsufi) > rebasculer sur le nouveau serveur quand il sera terminé

## 💥 Tâches critiques

Bug clients majeurs, interruptions de service, etc.

## 🚧 WIP 🚧

Si travail en cours, indiquer *les notes* ici

## ⚡️ Tâches rapides ✨

Indiquer ici les *tâches en dehors du flux général* (urgences, corrections process, trucs qui perturbent et doivent être fait, tâches ultra rapides, etc.)

1. Migrer ancien serveur
   1. Tester conteneurs de serveurs (facilité/stabilité/vitesse/http3)
      1. Apache
      2. Nginx
      3. Caddy
      4. Lightspeed
   2. Migrer sites une fois serveur choisi
      1. Lister
         1. Technos
         2. 📌📌📌📌📌📌📌 Fichiers
         3. BDD / Exports WordPress
      2. Basculer
2. github > secrets > Rajouter tous les identifients du boulot
3. Faire photos nouvel apart
4. drive > clients > passer sur github
5. Serveur
   1. Création d'un site > création d'un utilisateur pour connexion ssh, qui remplace ftp (clé publique privée, etc.)
   2. Maj de la nomenclature des sites clients : sub-domain--da-domain--ext
      1. Nom des dossiers
      2. Noms des fichiers
      3. noms des volumes
   3. Git > virer/sauv ce qui n'est pas versionné
   4. Backup volumes automatiques
      1. Attention, volumes avec bind limités au répertoire de DOCKER_PEON, sinon *permission denied*
   5. Supprimer les conteneurs & volumes inutiles (bruno, devs)
   6. [Github issues](https://github.com/bitnami/bitnami-docker-mysql/issues/79#issuecomment-545477842) > Variable d'env afin d'augmenter le debug des conteneurs bitnami ! >> raisons explicites sur le problème de boot du conteneur
   7. Corriger 98-maintenance > faire vraiment les upgrades
   8. BUG: Génération du wordpress : certaines variables font planter le lancement de mariaDB, voir pour trouver le mauvais caractère & l'exclure lors de la génération
      1. cf. ansible-install-web-server\ansible\tmp\BUG VARIABLES client--picard--dev-champagne-pascal-picard-com--wordpress-stack--generated copy.yml > mariadb > environnement
   9. Checker ce qui prend de la place sur le disque ~80Go ? 13% de 450 > `docker system df -v`
   10. Fixer ansible-install-web-server\ansible\roles\wordpress-generate\templates\ "original", doublons
   11. Terminer ansible > wordpress generate > /tmp > donner des dossiers aux clients
   12. Virer sites de tests et doublons
   13. Cleaner génération d'un wordpress
   14. Migrer sites > Liste ?
   15. Régénérer sites déjà présents
      - Passer nonore en cliente (wp généré et lancement depuis ansible), Pour le moment c'est un yml lancé a l'arrache sur le serveur
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
7. Truc baptiste guerechi
8. Relancer impôts pro pour CFE
9. Renvoi doc AE décla 0€ années passées [hey](https://mail.google.com/mail/u/0/#inbox/FMfcgxmXKmkCGqSQkpPRbBrSKWcsbCpr)
10. CPF > Langage des signes / Amazon AWS

## 💩 Shame

Parfois, l'entropie.

Emplois du temps stockés sur mail, portable, favoris, bureau.

Extraire ici puis ranger & prioriser. Doit rester vide.

---

Tout est extrait :)

---

### Priorisation

Ordonner puis ranger dans le flux. Doit rester vide.

---

Tout est priorisé :)

---
