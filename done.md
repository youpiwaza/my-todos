# Done

Les tâches terminées des semaines précédentes :)

## 05/07/21

Perso

- ✅ Inscription piscine
- ✅ Appeler damien pour aout
  - ✅ Inviter guillaume wawrhammers

AE

Server

1. forge playbookS
   1. ✅ Manual > Restore backup
      1. ✅ manual > host
      2. ✅ manual > local
      3. ✅ nginx > host
      4. ✅ nginx > local
      5. ✅ wordpress > host
      6. ✅ wordpress > local
      7. ✅ Rajouter commande en dur pour vérifier contenu du volume, dans les playbooks de restauration de sauvegarde
      8. ✅ nginx > add commands to readme
      9. ✅ wordpress > add commands to readme
   2. ✅ Optimisation > Passer les playbooks locaux en delegate 127.0.0.1 pour éviter les connexions inutiles

## 28/06/21

Perso

- ✅ Virement remb emprunt juillet
- ✅ Gérer déménagement box sfr, voir avec Pierre
- ✅ Réservation Black sheep 3 juillet 8 personnes

AE

- ✅ Nouveau NDD masa > demo.masamune.fr afin de pouvoir montrer le déploiement
- ✅ Clean noms de domaines masa
- ✅ Décla AE juin

Serveur

1. ✅ FIX: Ajouter la réaparation auto des dépendances
   1. [state: fixed](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/apt_module.html#parameter-state)
   2. ✅ system-update > update-packages
   3. ✅ package-installation
2. forge playbookS
    1. playbooks supplémentaires
       1. ✅ stop stack / ansible-install-web-server\ansible\51-stop-traefik-service.yml
          1. ✅ Créer une rôle quand même, sinon la tâche ne sera dispo qu'après génération (pas de possibilité de ponctuel, etc.)
       2. Generated doc
          1. ✅ prefix 100-
          2. ✅ à la racine également
       3. ✅ Utiliser const_prefix pour les playbooks générés (vu qu'il va y en avoir 4+ pour chaque projet, cela permet l'alpha-order)
          1. 100---hello--masamune--fr---nginx-stack--start--generated
          2. la^
       4. ✅ uninstall stack (stop + rm volumes)
          1. ✅ Création du rôle *stack-web-nginx--uninstall* / se baser sur deploy)
          2. ✅ Génération playbook par site `roles/stack-web-nginx--generate-playbooks/templates/original---nginx-playbook-start.yml`
          3. ✅ rôle wordpress
          4. ✅ playbook wordpress
       5. ✅ save volumes
          1. ✅ Création de l'arborescence, attention au répertoire année courante, cf. nomenclature-and-folder-tree.md
          2. ✅ Ponctuel pour un volume souhaité, `cf. commandes-backup-volumes-a-la-maing_secret.md`
             1. ✅ Variables : nom du volume & dossier de destination a l'intérieur
             2. ✅ Automatiser arbo, nom & date de l'archive
             3. ✅ Sauvegarde en ligne
                1. ✅ Extraire en rôle
             4. ✅ Create a "latest" backup, to simplify the gathering
             5. ✅ Rapatriement en local
          3. ⛔🌱 Refacto création de volume
             1. Créer un rôle avec variables nom de volume & dossier
             2. Non, il y a également les labels, le type de volume, et les opérations particulières, pour le moment je préfère tout laisser groupé
          4. ✅ volumes nginx
             1. ✅ Générer playbookS sauvegarde
             2. ✅ Ajouter sauvegarde avant uninstall
          5. ✅ volumes wordpress
             1. ✅✅ Générer playbookS sauvegarde
             2. ✅ Ajouter sauvegarde avant uninstall
          6. ✅ Revoir arbo des backups > Ajouter client & dashed-uri, avec des défauts dans les playbook 95-96

## 21/06/21

Perso

- ✅ Mairie reims déménagement 10 07 21 > bloquer parking devant
  - Fait le 23/06/2021
- ✅ Je dois 30€ a sofia

AE

- ✅ Deprecated all old react projects
- ✅ Facture passerelle juin 2021

Serveur

1. forge playbookS
    1. playbooks supplémentaires
       1. ✅ stop stack / ansible-install-web-server\ansible\51-stop-traefik-service.yml
       2. ✅ Utiliser const_prefix pour la generation de starts
          1. 100---hello--masamune--fr---nginx-stack--start--generated
          2. la^

## 07/06/221

✅ Github bot dependalerts > Fix

Serveur

1. ✅ Fusionner config dans generate
2. ✅ Plus de dossier /configs, directement dans le dossier client/etc/habituel/
3. ✅ Lint nginx folder & filenames > Renommer '/home/{{ users.3.name }}/configs/webserver/nginx/tutum--customUser-p8080-php--nginx.conf'
   1. ansible-install-web-server\ansible\roles\stack-web-nginx--config\tasks\main.yml
   2. ^ Attention à changer les chemins d'injection dans les .yml également
   3. ansible-install-web-server\nomenclature-and-folder-tree.md
4. ✅ WordPress forge stack > WordPress forge role
   1. ✅ Playbook to generate .yml files: playbook & role 20X-forge---DASHED-URI---wordpress-stack-generated.yml
   2. ✅ Ajuster stack-web-wordpress--generate-stack
5. ✅ Nginx forge stack > WordPress forge role
   1. ✅ Créer fichier de variables de projet
   2. ✅ Adapter generate stack
6. ✅👥 stack-web-nginx--generate > vars comme wordpress
7. ✅ Sur les fichiers générés
   1. ✅ En-tête avec commentaire: "Généré avec ansible + timestamp + ref au fichier original + ref playbook original"
   2. ✅ suffixe extension > ex "README.j2" devient "README.md.j2"
8. ✅ ansible > \n KO
9. ✅ Deprecated docker_container explicit default behavior stuff [container_default_behavior: compatibility](https://docs.ansible.com/ansible/latest/collections/community/docker/docker_container_module.html#parameter-container_default_behavior)
   1. ✅ ansible-install-web-server\ansible\roles\core-reverse-proxy-traefik--run\tasks\main.yml
   2. ✅ ansible-install-web-server\ansible\roles\stack-web-nginx--generate
   3. ✅ ansible-install-web-server\ansible\roles\stack-web-nginx--deploy
10. ✅ BUG: stack-web-nginx--deploy > can't update due to timestamp in .conf file
11. ✅ Forge playbookS > At the end add a message to start the generated playbook
12. ✅ Maj traefik ?
13. ✅ Clean noms containers (noms services fichiers yml :
    1. OK / test---test-wordpress--masamune--fr_mariadb.1.6u0pzz5paqai596um2b22eu1c
    2. NOK / test---hello-php--masamune--fr---tutum-hello-php_hello-php.1.
14. ✅ Add docker images credits.docs
15. ✅✅✅ Clean cette TODO, enlever les doublons👥

---

1. forge playbookS
    1. ✅ Tout dans dossier /generated
    2. ✅ History dans un sous dossier /history (sinon on va pas s'en sortir)
    3. ✅ Playbooks générés > Ne pas interpréter certaines variables (crrentDateTime & users)
       1. ✅ Update timestamps, cf. ansible-install-web-server\ansible\10-forge-a-nginx.yml
       2. ✅ Preserve vars string REMOVE-ME-TO-PRESERVE-VARS > ansible-install-web-server\ansible\roles\stack-web-nginx--generate-playbooks\templates\nginx-playbook-start.yml.j2
       3. ✅ Remove string > ansible-install-web-server\ansible\roles\stack-web-nginx--generate-playbooks\tasks\main.yml
    4. playbooks communs ? injectés depuis forge spécifiques dans 100 & 200 ?
    5. Générer des README.md
       1. ✅ Warning généré & Timestamp
       2. ✅ Intro 1 liner
       3. ✅ Principales commandes
          1. ✅ Recos lancement depuis ansible
       4. ✅ Kwaksé & technos
       5. ✅ Repo github & script principal
       6. ✅ Majs
       7. ✅ ! template vars file > add techno & go common (afin de différencier les noms des scripts et des commandes, etc.)
       8. ✅ ! folder path
       9. ✅ README sur serveur également, à la racine du projet

## 01/06/21

✅ Maj VLC

Serveur

- ✅ Update hello tests
  - ✅ New dashed notation
  - ✅ Separate from role 4, in order to be easier to start new services, make a BP
  - Hello php
    - ✅ Passer en https
- ✅ Tâches > Ajout de la commande d'éxécution correspondante dans chaque fichier (et pas uniquement dans README.md)
- ✅ ansible-install-web-server/ansible/tmp/ > Transformer le dossier tmp/ en generated/
- ✅ Maj **locales** putaing
  - ✅ WSL
  - ✅ Terminal
  - ✅ Docker Desktop
  - Maj tuto environnement de dev
    - ✅ Terminal
    - ✅ [Video du gars](https://ww-youtub-com/watch?v=idW-an99TAM)
    - ✅ Docker
    - ✅ Autres
- ✅ Connexion au serveur optimisée
- ✅ Libérer espace disque C
- ✅ ansible-install-web-server/ansible/tmp/tests/masamune/test-wordpress--masamune--fr/generated > Transformer le dossier generated en var-files/
- ✅ Uniformiser install/generate/init/setup
  - ✅ core
  - ✅ tutum/nginx
  - ✅ wordpress
  - Choix des mots :
    - Etape 1 : Fichiers générés en local, puis copiés en ligne > generate
    - Etape 2 : Network & volumes, lancement/Mise à jour des stacks > run
    - Besoin de prefixes, ex:
      - ✅ core-reverse-proxy-traefik--generate
      - ✅ core-reverse-proxy-traefik--run
      - core-monitoring-grafana-generate
      - core-monitoring-grafana-run
      - ✅ stack-web-nginx--configs
      - ✅ stack-web-nginx--generate
      - ✅ stack-web-nginx--deploy
      - ✅  stack-web-wordpress--generate
      - ✅  stack-web-wordpress--deploy
      - ✅ 10-forge-a-nginx-stack # generate & run > setup network & volumes & < config, generate, upload, start/updat- Avec un README ça passe
      - ✅ 20-forge-a-wordpress-stack
- ✅ Séparer nginx & nginx php
- ✅ Optimiser local/server, la seule diff c'est le début du chemin
- Ajouter local & history partout, ref : ansible/roles/core-reverse-proxy-traefik--generate/tasks/main.yml
  - ✅ stack-web-nginx--generate
    - ✅ local
    - ✅ history
  - 💩 stack-web-nginx-php--generate
    -💩 Refaire a partir de nginx, garder que la conf
    - 🔥 Non, en fait ce sont les mêmes, les deux ont besoin de php
  - ✅ stack-web-wordpress--generate
    - ✅ generate id > local > history
    - ✅ stack > history
- ✅ nginx conf worker_connections  127; check diff entre normal et php << max perf : 1024
- ✅ Générer tous les fichiers en local dans generated/
  - ✅ core / reverse proxy
  - ✅ tutum/nginx / test-hello & hello-php
  - ✅  ansible-install-web-server\ansible\4-setup-core-services.yml
  - ✅  Extract config wtf l. ~75 📌📌📌 normalement c'est fait + generated mais tjr besoin de split nginx & nginx phpay
  - ✅  tout en fait
- ✅ Serveur > Corriger 98-maintenance > faire vraiment les upgrades
  - ansible-install-web-server/ansible/roles/system-update/tasks/update-packages.yml, l. 8
  - 📌✅ Besoin d'un maj de plugin pour constater le bug > corrigé
- ✅ Changer message d'accueil KO

## 24/05/21

1. Taf
   1. ✅ Réparer baptiste guereschi
   2. ✅ Picard avec https
      1. ✅ DNS corrects pour dev
      2. ✅ Url wp corrects pour dev
      3. ✅ Checkup complet
      4. ✅ Confirmation des picard que tout est good
      5. ✅ Passer en prod
         1. ✅ Url du wordpress changées dans les réglages
         2. ✅ DNS changés
            1. [Doc OVH](https://docs.ovh.com/fr/hosting/erreur-site-non-installe/)
            2. Attendre ~15-20min > 17h20
         3. ✅ HTTPS régénérés
         4. ✅ Vérif fin de soirée
         5. ✅ Vérif lendemain
      6. ✅ .fr KOs > forcer redirection vers .com
   3. Serveurh
      1. ✅ Cleaner ansible-install-web-server/ansible/roles/wordpress-generate/templates > original stack ?
      2. ✅ Backup nouveau serveur (volumes containers)
      3. ✅ Lapie > All in one WP Migration
      4. ✅ Tests backup volume > .tar
         1. [Doc volumes](server-related-tutorials/01-docker/03-develop-with-docker/02-volumes/README.md)
      5. 💩 Tests [archivage incrémentiel](https://doc.ubuntu-fr.org/tar#utilisation_en_archivage_incrementiel)
         1. Test sur fichier alakon
         2. Test sur fichier alakon dans volume
         3. KO / --listed-incremential not found dans `tar`
      6. ✅ Cleaner backup
         1. ✅ Mettre nom, date & heure dans le nom de fichier de la sauvegarde
            1. `nom-volume---backup---$(date +%Y-%m-%d--%H.%M.%S).tar`
         2. ✅ Contenu de l'archive propre : 1 seul dossier bien nommé
         3. ✅ Bien le ranger sur l'hôte (emplacement à choisir + maj ansible-install-web-server/nomenclature-and-folder-tree.md)
            1. Les volumes sont liés aux conteneurs, mais contenu sensible (!DOCKER_PEON) > dans le dossier de DOCKER_GUY/
            2. Arbo logique ek details `DOCKER_GUY/backups/volumes/clients/LE_CLIENT/SITE_COM/ANNEE/nom-volume---backup---$(date +%Y-%m-%d--%H.%M.%S).tar`
            3. Mais, les noms de volumes ont de l'info, ex : `client---dev--masamune-fr---wordpress--db`, mais les sauvegardes seront récurrentes (vite le bordel si beaucoup de fichiers)
            4. `DOCKER_GUY/backups/volumes/ANNEE/TYPE/LE_CLIENT/SITE_COM/nom-volume---backup---$(date +%Y-%m-%d--%Hh%Mm%Ss).tar`
            5. Eg. `DOCKER_GUY/backups/volumes/2021/clients/masamune/dev--masamune--fr/client---dev--masamune--fr---wordpress--db---backup---2021-05-27--11h23m57s.tar`
         4. ✅ Documenter
            1. ✅ Fichier de commandes usuelles, pour sauvegarde manuelle
            2. ✅ Arborescence du serveur
               1. ✅ Maj de la notation dash
               2. ✅ Ajout des backups
      7. ✅ Faire les backups des volumes en prod
         1. ✅ Virer les stacks inutiles
         2. ✅ Faire les backups sur le serveur
         3. ✅ SSH > récupérer les archives en local/github
            1. ✅ Récupérer également les .yml temporaires (de nonore, etc.)
      8. ✅ Mettre à jour la dashed notation partout (folders, files, containers, volumes, networks)
         1. ✅ Update ~wp-generate & wp-setup
         2. ✅ 20-setup-a-wordpress.yml
      9. ✅ /tmp/ un dossier par client et par site
         1. ex: `'/home/{{ users.3.name }}/{{ project.type }}s/{{ project.client_name }}/{{ project.dashed_domain }}/wordpress-stack--generated.yml'`
         2. cf. ansible-install-web-server/ansible/roles/wordpress-generate/vars/template.yml
         3. ansible-install-web-server\ansible\roles\wordpress-generate\tasks\generate-ids-readme.yml
         4. ansible-install-web-server\ansible\roles\wordpress-generate\tasks\generate-wordpress-stack-file.yml
         5. & template files *.j2
      10. ✅📌 Tester les rôles sur un [wp masa](https://test-wordpress.masamune.fr/)
   4. ✅ Devis Nico 14 au 18/06/21 (5 jours)
   5. ✅ Git > virer/sauv ce qui n'est pas versionné
   6. ✅ Cleaner/prioriser tâches serveur + OLD
   7. Local
      1. ✅ docs _secret > need versionné quand même sur github en repo privé
         1. ✅ Virer les tests/non clients
         2. ✅ Github privé en respectant arbo
2. Perso
   1. ✅ Dématérialiser carte SNCF
   2. ✅ Commander / Livraison
       1. 20/05
          1. Han Hepa
   3. ✅ Faire photos nouvel apart
   4. ✅ Extraire, ✅dédoublonner, ✅retailler & ✅ ranger photos portable
   5. ✅ Backup wallpapers

## 17/05/21

1. ✅ Labo Prise de sang
   1. Lundi 17/05 à 10h
   2. Merci de vous présenter au laboratoire avec votre ordonnance, votre carte vitale et votre carte de mutuelle.
   3. Il est préférable de venir à jeun
   4. RDV doc > carnet de santé : rappel vaccin &
2. ✅ Rdv doc résultats analyses sang et autre
   1. ✅ Rdv pris
3. ✅ docteur en récurrent 1 x an
4. ✅ Commander / Livraison
    1. Vendredi 14/05
       1. Huile de foie de morue
       2. Gelée royale
       3. Guarana
    2. Samedi 15/05
        1. Ginseng
    3. 17/05/2021
        1. Cable chaine stéréo
    4. 19/05
       1. Truc foie
       2. Choline
5. ✅ Confirmer Maj adresse siret
6. ✅ Assurance > Mercer / ou changer ? >> Alan FTW
   - FNAE [otherwise](https://www.federation-auto-entrepreneur.fr/sites/default/files/otherwise_-_guide_des_assurances_pour_les_auto-entrepreneurs_de_la_fnae_0.pdf)
   - [alan](https://alan.com/tns)
   - [malt + axa](https://messolutionsplus.fr/msp/S/S/S/web-insure-quote/new-quote/productId/MALT_PREV?_ga=2.257990786.968299628.1601458302-2117978627.1601458301)
   - mercer cf. mails
7. ✅ ovh manager > Modifier adresse client
8. Picard avec https
   1. Backup site existant
      1. ✅ All in one WP Migration
   2. 💩 Problèmes de stabilité sur nouveau serveur > Commande hébergement kimsufi le temps de les régler
   3. ✅ Attente mise en place de la commande
   4. 💩📌 Mise en place du DNS dev. vers le nouveau serveur
      1. Ok pour krépautak mais ko pour dev.champ -.-
   5. ✅ Https
   6. ✅ Import & maj de l'ancien site
      1. [admin temp](http://krpauax.cluster029.hosting.ovh.net/wp-admin/)
      2. ✅ BDD
      3. ✅ Themes
      4. ✅ Plugins
      5. ✅ Mises a jour
      6. ✅ Médias
      7. ✅ Backups
