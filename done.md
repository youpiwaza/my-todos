# Done

Les tâches terminées des semaines précédentes :)

## 24/05/21

1. Taf
   1. ✅ Picard avec https
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
   2. Serveurh
      1. ✅ Backup nouveau serveur (volumes containers)
      2. ✅ Lapie > All in one WP Migration
      3. ✅ Tests backup volume > .tar
         1. [Doc volumes](server-related-tutorials/01-docker/03-develop-with-docker/02-volumes/README.md)
      4. 💩 Tests [archivage incrémentiel](https://doc.ubuntu-fr.org/tar#utilisation_en_archivage_incrementiel)
         1. Test sur fichier alakon
         2. Test sur fichier alakon dans volume
         3. KO / --listed-incremential not found dans `tar`
      5. ✅ Cleaner backup
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
      6. ✅ Faire les backups des volumes en prod
         1. ✅ Virer les stacks inutiles
         2. ✅ Faire les backups sur le serveur
         3. ✅ SSH > récupérer les archives en local/github
            1. ✅ Récupérer également les .yml temporaires (de nonore, etc.)
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
