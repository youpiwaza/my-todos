# Done

Les tâches terminées des semaines précédentes :)

## 01/06/21

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
      - ✅ stack-web-nginx--run
      - ✅  stack-web-wordpress--generate
      - ✅  stack-web-wordpress--run
      - ✅ 10-forge-a-nginx-stack # generate & run > setup network & volumes & < config, generate, upload, start/updat- Avec un README ça passe
      - ✅ 20-forge-a-wordpress-stack

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
