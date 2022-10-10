# Done

Les tâches terminées des semaines précédentes :)

## 09/10/2022

AE

1. ✅ Cleaner déclarations 3 derniers mois

Perso

1. ✅ Payer tout le monde
   1. ✅ Payer impots AE ~1k€
   2. ✅ Payer Avis de taxe d'habitation-CAP 2022 / 295,00 € par 2 = 148€ / Date limite de paiement : 15/11/2022
      1. Pougnoutte la prend en intégralité
   3. ✅ Payer syndic
2. ✅ Decathlon > Acheter poids plus lourd
3. ✅ Mail anouk
4. ✅ Vigi agenda spectacle
5. ✅ Nettoyer tireuse bière
6. ✅ Prévoir menus sadi soir & brunch gromanche
7. ✅ Cadeau anniv pougnoutte
    1. ✅ Arnaud tsamère

PB Modelisme

1. ✅ Réponses mails du 30/09/2022 et mise à jour de la TODO
2. ✅📧 Rapport de la semaine
3. 🚀 Import l'ensemble des catégories
   1. ♻️💥 Retour clients prioritaires
      1. ✅ 20/09/2022
         1. ✅ Ajouter un champ "Notices, fiches de sécurité & documents" de type `répéteur > document`, commun à tous les champs
            1. ✅ Mettre a jour le doc des champs personnalisés & secrets
            2. ✅ Rajouter un champ personnalisé commun à l'ensemble des produits
         2. ✅ Tous les produits > Par défaut "autoriser les commande en réappro"
            1. ✅ Supprimer l'ensemble des produits importés
            2. ✅ accessoires
               1. ✅ Mise à jour craft
               2. ✅ Mise à jour requête finale
               3. ✅ Réimporter les produits
            3. ✅ acctx
               1. ✅ Mise à jour craft
               2. ✅ Mise à jour requête finale
               3. ✅ Réimporter les produits
            4. ✅ avion
               1. ✅ Mise à jour craft
               2. ✅ Mise à jour requête finale
               3. ✅ Réimporter les produits
            5. ✅ bateaux
               1. ✅ Mise à jour craft
               2. ✅ Mise à jour requête finale
            6. ✅ batterie
               1. ✅ Mise à jour craft
               2. ✅ Mise à jour requête finale
               3. ✅ Réimporter les produits
            7. ✅ bougie
               1. ✅ Mise à jour craft
               2. ✅ Mise à jour requête finale
            8. ✅ carburant
               1. ✅ Mise à jour craft
               2. ✅ Mise à jour requête finale
            9. ✅ chargeur
               1. ✅ Mise à jour craft
               2. ✅ Mise à jour requête finale
               3. ✅ Réimporter les produits
            10. ✅ controleur
                1. ✅ Mise à jour craft
                2. ✅ Mise à jour requête finale
                3. ✅ Réimporter les produits
            11. ✅ heliceavion
                1. ✅ Mise à jour craft
                2. ✅ Mise à jour requête finale
                3. ✅ Réimporter les produits
            12. ✅ voitures
                1. ✅ Mise à jour craft
                2. ✅ Mise à jour requête finale
                3. ✅ Réimporter les produits
            13. ✅ boilerplate
                1. ✅ Mise à jour requête
      2. ⏳📧 30/09/2022
         1. ✅ Carburants > Composition `COMPOFUEL` > à rajouter en fin de description
            1. ✅ Mise à jour craft
            2. ✅ Réimporter les produits
            3. ✅📌 Vérification sur [Tornado Competition offroad](https://dev.pb-modelisme.com/wp-admin/post.php?post=4198&action=edit)
            4. ✅ Mise à jour requête finale
         2. ✅ Chargeurs > Renommer le champ "Charge type" en "Coupure fin de charge"
         3. ✅ Bougies > Nombre de temps > Il faut multiplier la valeur par 2 avant import
            1. ✅ Mise à jour craft
            2. ✅ Réimporter les produits
            3. ✅📌 Vérification sur [LC3](https://dev.pb-modelisme.com/wp-admin/post.php?post=4235&action=edit)
            4. ✅ Mise à jour requête finale
         4. ⏳📧 Bateaux > La catégorie "statique pouvant être rendu naviguant" est transféré dans "bateau naviguant"
            1. Pas compris, en attente de retour
      3. ✅📧 Mail Cédric confirmation traitement des retours & réimportations produits pour 20/09 & 30/09
      4. ✅♻️ Vérifier qu'il n'y a pas de champs à crafter/refacto sur les précédents imports
         1. ✅ Ajout au boilerplates
         2. ✅ accessoires
            1. ✅ `GOODESCACC` à ajouter en fin de description
            2. ✅📌💩 Pas de réimport, les 30+ produits plus récents ont ce champ NULL
            3. ✅ Maj requête finale
         3. ✅ bateaux
            1. ✅ `NBELEBAT`, "Nombre d'éléments sur les accus" > Dans la description
               1. en dur php ? 6 = "Electrique - 6 éléments NiMh" ou 7 = (tous les bateaux KO sur site). 🚨 Peut être NULL
               2. ✅ Analyse de l'ancien site ~> "`NBELEBAT` éléments NiMh"
               3. ✅ Ajout à la description
               4. ✅📌💩 Pas de réimport, les 30+ produits plus récents ont ce champ NULL
               5. ✅ Maj requête finale
         4. ✅ batterie
            1. ✅ `Pas de champ` Catégorie piles (alkaline (cdtypebat == 6) > dans description > pas rechargeable
               1. ✅ Déjà rajouté à la description
            2. ✅ `CDUTILBAT` > Utilisation de la batterie
               1. ✅ Déjà rajouté dans un champ personnalisé
            3. ✅ `KEYWRDBAT` > Mots clés
               1. ✅ Déjà rajouté aux étiquettes (tags)
         5. ✅🖐 bougie
            1. ✅ `4TPSGLOW` Nombre de temps
               1. ✅ Déjà rajouté dans un champ personnalisé
            2. ✅ Liens avec tables `allume` lien entre `bougie` et `moteur_thermique`, `type_moteur`, utilisé sur les moteurs pour bougies conseillés
               1. 🤏 40 bougies, on fera à la main
               2. ✅ Rajouté en note dans la doc
         6. ✅🖐 carburant
            1. ✅ Table "consomme" lien entre carburant et moteur_thermique > déterminer la compatibilité avec le type de véhicules
               1. 🤏 10 carburants affichés sur le site, on fera à la main
               2. ✅ Rajouté en note dans la doc
            2. ✅ `COMPOFUEL`
               1. ✅ Déjà rajouté à la description
         7. ✅ controleur
            1. ✅ `CDUTILCONTRO` > Compatibilité contrôleur
               1. ✅ Déjà rajouté dans un champ personnalisé
   2. ✅ accessoires
   3. ✅ acctx
   4. ✅📧 avion
      1. 🌱🌱🌱🚨 Peut contenir des vidéos (.mpg)
   5. ✅ bateaux
   6. ✅ batterie
      1. ✅ Créer la requête
          1. 🌱🌱🌱🚨 type_prise_accus > 🔗 Lien avec la table "accessoires". Produit recommandé > Prise avec lien
   7. ✅ bougie
   8. ✅ carburant
   9. ✅ chargeur
   10. ✅ controleur
   11. ✅ heliceavion
   12. ✅ helico
       1. ✅ Remplir ~~complètement~~ champs persos dédié un produit sur le nouveau site + cat _test_export
       2. ✅ Exporter le produit
       3. ✅ Linter le CSV
       4. ✅ Créer la requête
           1. ✅ Correspondance catégories ancien PB >< WC > Tout est différent, `CASE`
           2. ✅🧠 PAs de champ pour le nombre de moteurs, 1 par défaut, 4 si il s'agit de drones
           3. ✅♻️ Vérifier qu'il n'y a pas de champs à crafter/refacto
              1. ✅ `WARNTYPEHELI`, table `helicat`, mention légale danger d'utilisation > Déplacer dans description
       5. ✅ Export ancien site & import vers le nouveau site
       6. ✅📌 Tester
       7. ✅ Création de la requête finale
       8. ✅📧 Faire valider
   13. ✅ maquette
       1. ✅ Remplir ~~complètement~~ champs persos dédié un produit sur le nouveau site + cat _test_export
       2. ✅ Exporter le produit
       3. ✅ Linter le CSV
       4. ✅ Créer la requête
           1. ✅ Correspondance catégories ancien PB >< WC
           2. ✅♻️ Vérifier qu'il n'y a pas de champs à crafter/refacto
       5. ✅ Export ancien site & import vers le nouveau site
       6. ✅📌 Tester
       7. ✅ Création de la requête finale
       8. ✅📧 Faire valider
   14. ✅ matprem
       1. ✅ Remplir ~~complètement~~ champs persos dédié un produit sur le nouveau site + cat _test_export
       2. ✅ Exporter le produit
       3. ✅ Linter le CSV
       4. ✅ Créer la requête
           1. ✅ Correspondance catégories ancien PB >< WC > Ca a pris une plombe
           2. ♻️ Vérifier qu'il n'y a pas de champs à crafter/refacto
       5. ✅ Export ancien site & import vers le nouveau site
       6. ✅📌 Tester
       7. ✅ Création de la requête finale
       8. ✅📧 Faire valider
   15. ✅ moteur_electrique
       1. ✅ Remplir ~~complètement~~ champs persos dédié un produit sur le nouveau site + cat _test_export
       2. ✅ Exporter le produit
       3. ✅ Linter le CSV
       4. ✅ Créer la requête
           1. ✅ Correspondance catégories ancien PB >< WC
              1. ✅ Création de nouvelles catégories sur le site, afin d'assigner les compatibilités
                 1. Une seule compatibilité par catégorie
                 2. Possibilité d'avoir plusieurs catégories pour un produit
                 3. Homogénéisation des noms
              2. ✅ Réimport & lint produit test
           2. ✅ Pas oublier qu'il s'agit d'un accessoire (champs persos) > Champs NA
           3. ✅♻️ Vérifier qu'il n'y a pas de champs à crafter/refacto
       5. ✅ Export ancien site & import vers le nouveau site
       6. ✅📌 [Tester](https://dev.pb-modelisme.com/wp-admin/post.php?post=4588&action=edit)
       7. ✅ Création de la requête finale
       8. ✅📧 Faire valider
   16. 🚀 moteur_thermique
       1. ✅ Remplir ~~complètement~~ champs persos dédié un produit sur le nouveau site + cat _test_export
       2. ✅ Exporter le produit
       3. ✅ Linter le CSV
       4. Créer la requête
           1. Correspondance catégories ancien PB >< WC
           2. ♻️ Vérifier qu'il n'y a pas de champs à crafter/refacto
       5. Export ancien site & import vers le nouveau site
       6. 📌 Tester
       7. Création de la requête finale
       8. 📧 Faire valider

## 30/09/2022

Perso

1. ⏳ Payer tout le monde
   1. ✅ Payer nonore
   2. ✅ Payer remboursement emprunt
   3. ✅ Payer taxe foncière /  1 270,00 € par 2 = 635€
2. ✅ Répondre mails darons
3. ✅ Week end 1 er octobre concert x2
   1. ✅ Hebergement
   2. ✅ Theatre le dimanche
   3. ✅ Mail sites sorties
   4. ✅ Réserver parking, attente horaire po en fonction oncle/théatre
   5. ✅ Mail remboursement Po
4. Cadeau anniv pougnoutte
   1. ✅ Surprise dredi 07/09/2022
5. 🚀 Réserver concerts
   1. 💩 GuiV > The Hu, casino de paris, le 25/11 > Complet
   2. ✅ Igorrr, [hey](https://www.seetickets.com/fr/ap/event/igorrr/salle-pleyel/32806)
      1. ✅ Agenda
   3. ✅ Avatar
      1. ✅ Agenda

Lapie

1. ✅🐛 Les clients ne peuvent pas se connecter à leurs comptes
   1. ✅ L'option était désactivée dans WordPress et dans WooCommerce
      1. ✅ WP > Réglages > Général > Autoriser les gens à s'inscrire + role de base "client"
      2. ✅ WC > Réglages > Comptes > Afficher connexion/inscription sur mon compte & pendant la commande
      3. ✅📌 Vérifications
2. ✅ Mails changements de mot de passe > Il s'agit des comptes utilisateurs, pas des comptes admin

Ophé

1. ✅ Formation admin

PB Modelisme

1. 🌱🔍 Réductions de prix réduit en cas de commande de multiples éléments
   1. 🌱 Plus tard et/ou à la main, ça me soule
2. 🚀 Import l'ensemble des catégories
   1. ✅♻️💥 Retour clients prioritaires
      1. ✅ 20/09/2022
         1. ✅ Champ visibilité `AFF* / AFFVOITURE`, si valeur 4 "sur commande"
            1. ✅ Mettre a jour le doc drive
            2. ✅ Mettre a jour le doc des champs personnalisés & secrets
            3. ✅ Rajouter un champ personnalisé commun à l'ensemble des produits
            4. ✅ Maj boilerplate
         2. ✅ Champs dimensions & poids à retirer des champs expédition (il s'agit des colis)
            1. ✅ Mettre a jour le doc drive
            2. ✅ Mettre a jour le doc des champs personnalisés & secrets
            3. ✅ Rajouter les champs personnalisés communs à l'ensemble des produits
            4. ✅ Maj boilerplate
         3. ✅ Stock par defaut pas de commande en reaprovisionnement, voir CASE cf mail cedric 20/09/2022
            1. ✅ Ajout de l'autorisation de commande en réapprovisionnement avec notif client
            2. ✅👷 Modification du champ perso, instructions pour administrateurs
         4. ✅ Répercuter les changements
            1. ✅ voitures
               1. ✅ dimensions & poids > `POIDSVOITURE` x 4
               2. ✅ sur commande > "Gestion des `"sur commande uniquement"` " x 2
               3. ✅ maj requête craft
               4. ✅ csv de test
               5. ✅ maj requête finale
            2. ✅ Maj boilerplate requête
            3. ✅ accessoires
               1. ✅ dimensions & poids > `POIDSVOITURE` x 4
               2. ✅ sur commande > "Gestion des `"sur commande uniquement"` " x 2
               3. ✅ maj requête craft
               4. ✅ csv de test
               5. ✅ maj requête finale
         5. ⏳ Ajouter un champ "Fiches de sécurité" de type document, commun à tous les champs
            1. ⏳ En attente de savoir si on rajoute un champ ou un répéteur
            2. Mettre a jour le doc des champs personnalisés & secrets
            3. Rajouter un champ personnalisé commun à l'ensemble des produits
         6. ✅ Mail confirmation & recettage
      2. ✅ 27/09/2022
         1. ✅ Import Accessoires > VALEURTRI = capacite_en_cc > Faux
            1. ✅ Ajouter un nouveau champ legacy
               1. ✅ Maj doc BDD
               2. ✅ Maj doc champs persos
               3. ✅ Maj requête accessoires
               4. ✅ Maj requête accessoires finale
               5. ✅ Maj boilerplate
               6. ✅📌 [Produit de test](https://dev.pb-modelisme.com/wp-admin/post.php?post=3655&action=edit)
            2. ✅  Populer les champs "Communs > Divers > diamètre" (hélices) et "Accesoires > capacité" (réservoirs)
               1. ✅ Maj doc BDD
               2. ✅ Maj doc champs persos
               3. ✅ Maj requête accessoires
               4. ✅ Maj requête accessoires finale
               5. ✅ Maj boilerplate
            3. ✅📧 Faire valider
   2. ♻️ Global craft
   3. ✅ accessoires
      1. ✅ Maj suite aux retours de Cédric 20/09/2022
      2. ✅ Export ancien site & import vers le nouveau site
      3. ✅📌 Tester
      4. ✅📧 Faire valider
   4. ✅ acctx
      1. ✅ Remplir complètement un produit sur le nouveau site, ajouter une catégorie pour export de cette catégorie
      2. ✅ Exporter le produit
      3. ✅ Linter le CSV
      4. ✅ Ajouter le masque des champs deprecated
      5. ✅ Créer la requête
          1. ✅⬆️ Catégories à migrer dans `accessoires > Accessoires radios`
      6. ✅ Export ancien site & import vers le nouveau site
      7. ✅📌 Tester
      8. ✅ Faire valider
   5. ✅📧 avion
      1. ✅ Remplir complètement un produit sur le nouveau site, ajouter une catégorie pour export de cette catégorie
      2. ✅ Exporter le produit
      3. ✅ Linter le CSV
      4. ✅ Ajouter le masque des champs deprecated
      5. ✅ Créer la requête
          1. ✅ Correspondance catégories ancien PB >< WC
             1. ✅ Catégorie 3D ?
                1. ✅🐛 Il s'agit d'un type d'avion, et non d'une catégorie. fixé
             2. ✅📧 CDCATAVION -1, CDAVION 957 ?
                1. ✅ Corrigé par Cédric dans l'ancienne BDD, rien à changer de mon côté.
          2. ✅🐛 `materiau_aile` `materiau_fuselage` > "Elapor &amp; EPP" après l'import dans wordpress
          3. ✅ Onglet servos conseillés > possibilité d'affecter plusieurs catégories
             1. ✅ Mise à jour des champs personnalisés afin de changer le choix unique en choix multiples
                1. 💩 Pas de valeurs dans l'export ? Champ de type taxonomie
                2. ✅👴 Création d'un champ legacy (texte) avec la concaténation des catégories
                   1. ✅ Création du champ personnalisé
                   2. ✅ Récupération d'un export WC
             2. ✅ Adapter la requête > table depend & cat servo
      6. ✅ Export ancien site & import vers le nouveau site
      7. ✅📌 Tester
      8. ✅ Création de la requête finale
      9. 🌱🌱🌱🚨 Peut contenir des vidéos (.mpg)
      10. ✅📧 Faire valider
   6. ✅ bateaux
      1. ✅ Remplir complètement un produit sur le nouveau site, ajouter une catégorie pour export de cette catégorie
      2. ✅ Exporter le produit
      3. ✅ Linter le CSV
      4. ✅ Ajouter le masque des champs deprecated
      5. ✅ Créer la requête
          1. ✅ Correspondance catégories ancien PB >< WC
          2. ✅📧 Menu ancien site > bateaux > Type > PLastique & statiques > Renvoie vers une catégorie de maquettes
             1. On ne s'en occupe pas ?
             2. Je met une note pour leur rajouter la catégorie bateaux en plus lorsque je traiterai les maquettes ?
             3. > On touche à rien, on laisse comme ça
      6. ✅ Export ancien site & import vers le nouveau site
      7. ✅📌 Tester
      8. ✅ Création de la requête finale
      9. ✅📧 Faire valider
   7. ✅ batterie
      1. ✅ Remplir ~~complètement~~ champs persos dédié un produit sur le nouveau site + cat _test_export
      2. ✅ Exporter le produit
      3. ✅ Linter le CSV
      4. ✅ Créer la requête
          1. ✅ Correspondance catégories ancien PB >< WC
          2. 🌱🌱🌱🚨 type_prise_accus > 🔗 Lien avec la table "accessoires". Produit recommandé > Prise avec lien
      5. ✅ Export ancien site & import vers le nouveau site
      6. ✅📌 Tester
      7. ✅ Création de la requête finale
      8. ✅📧 Faire valider
   8. ✅ bougie
      1. ✅ Remplir ~~complètement~~ champs persos dédié un produit sur le nouveau site + cat _test_export
      2. ✅ Exporter le produit
      3. ✅ Linter le CSV
      4. ✅ Créer la requête
          1. ✨ Correspondance catégories ancien PB >< WC. En dur
      5. ✅ Export ancien site & import vers le nouveau site
      6. ✅📌 Tester
      7. ✅ Création de la requête finale
      8. ✅📧 Faire valider
   9. ✅ carburant
      1. ✅ Remplir ~~complètement~~ champs persos dédié un produit sur le nouveau site + cat _test_export
      2. ✅ Exporter le produit
      3. ✅ Linter le CSV
      4. ✅ Créer la requête
          1. ✅ Correspondance catégories ancien PB >< WC. en dur
      5. ✅ Export ancien site & import vers le nouveau site
      6. ✅📌 Tester
      7. ✅ Création de la requête finale
      8. ✅📧 Faire valider
   10. ✅ chargeur
       1. ✅ Remplir ~~complètement~~ champs persos dédié un produit sur le nouveau site + cat _test_export
       2. ✅ Exporter le produit
       3. ✅ Linter le CSV
       4. ✅ Créer la requête
           1. ✅ Correspondance catégories ancien PB >< WC. En dur
           2. ✅🐛 Un caractère spécial dans l'une des `descriptions longue` bloque l'import
              1. CD `183` Nom "KN-PROX2" [le coupable](https://pb-modelisme.com/Chargeur/showprod.php?prod=183)
                 1. Le caractère est KO à la fois dans phpmyadmin et à l'affichage du site
                 2. On vire avec un `REPLACE`
       5. ✅ Export ancien site & import vers le nouveau site
       6. ✅📌 Tester
       7. ✅ Création de la requête finale
       8. ✅📧 Faire valider
   11. ✅ controleur
       1. ✅ Remplir ~~complètement~~ champs persos dédié un produit sur le nouveau site + cat _test_export
       2. ✅ Exporter le produit
       3. ✅ Linter le CSV
       4. ✅ Créer la requête
           1. ✅ Correspondance catégories ancien PB >< WC. En dur.
              1. ✅ Cas particulier, nouvelles catégories pour "utilisation"
       5. ✅ Export ancien site & import vers le nouveau site
       6. ✅ 📌 Tester
       7. ✅ Création de la requête finale
       8. ✅📧 Faire valider
   12. ✅ heliceavion
       1. ✅ Remplir ~~complètement~~ champs persos dédié un produit sur le nouveau site + cat _test_export
       2. ✅ Exporter le produit
       3. ✅ Linter le CSV
       4. ✅ Créer la requête
           1. ✅ Correspondance catégories ancien PB >< WC
       5. ✅ Export ancien site & import vers le nouveau site
       6. ✅ 📌 Tester
       7. ✅ Création de la requête finale
       8. ✅📧 Faire valider
   13. ✅ voitures
       1. ✅ Maj suite aux retours de Cédric 20/09/2022
       2. ✅📧 Faire valider

## 23/09/2022

Perso

1. ✅ Go Fnac acheter cadeaux Po & Mo
2. ✅ Demande dépannage parents
3. Mortier pour MSG maison
   1. ✅ Achat mortier

PB Modelisme

1. 🚀 Import l'ensemble des catégories
   1. 🚀♻️💥 Retour clients prioritaires
      1. ✅ Champ visibilité `AFF* / AFFVOITURE`, si valeur 4 "sur commande"
         1. ✅ Mettre a jour le doc drive
         2. ✅ Mettre a jour le doc des champs personnalisés & secrets
         3. ✅ Rajouter un champ personnalisé commun à l'ensemble des produits
         4. ✅ Maj boilerplate
      2. ✅ Champs dimensions & poids à retirer des champs expédition (il s'agit des colis)
         1. ✅ Mettre a jour le doc drive
         2. ✅ Mettre a jour le doc des champs personnalisés & secrets
         3. ✅ Rajouter les champs personnalisés communs à l'ensemble des produits
         4. ✅ Maj boilerplate
      3. ✅ Stock par defaut pas de commande en reaprovisionnement, voir CASE cf mail cedric 20/09/2022
         1. ✅ Ajout de l'autorisation de commande en réapprovisionnement avec notif client
         2. ✅👷 Modification du champ perso, instructions pour administrateurs
      4. ✅ Vérifier l'import correcte des marques, peut être une correspondance à faire
         1. ✅📧 Il s'agissait simplement des liens sur le menu principal qui sont KO (placeholders)
      5. ✅📧 Faire valider par Cédric les 5 premières modifications
         1. "Sur commande"
            1. champ rajouté dans champs communs > divers
            2. Modification du champ WC "Données produit" > "Inventaire" > "Autoriser les commandes en réapprovisionnement ?"
               1. Si le produit est sur commande uniquement, autoriser avec notification client
               2. Par défaut elles ne sont pas autorisées
         2. Champs dimensions & poids à retirer des champs expédition (il s'agit des colis)
            1. Création de champs particuliers dédiés & modification de l'import
   2. ♻️ Global craft
      1. ✅ Correspondances catégories ancien PB & WC
         1. ✅ Récupération de l'intégralité des libellés de catégorie & sous catégorie de WC au format CSV (8 plombes)
         2. ✅ Lint
            1. Réorganisation alphabétique
               1. ✅ Catégories
               2. ✅ Sous cat
               3. ✅ sous sous cat
               4. ✅ sous sous sous cat -_-
         3. ✅ Ajout tâche Diff & correspondance avec WC à chaque import de catégorie
         4. ✅ Maj boilerplate
         5. ✅ Maj voitures
         6. ✅🧽 Harmoniser les catégories
            1. ✅ 'pr' > 'pour'
            2. ✅ pluriels
            3. ✅ préfixes
            4. ✅ Maj accessoires
         7. ✅📝 Procédure pour les imports des catégories restantes
   3. accessoires
      1. ✅ Remplir complètement un produit sur le nouveau site, ajouter une catégorie pour export de cette catégorie
      2. ✅ Exporter le produit
      3. ✅ Linter le CSV
      4. ✅ Créer la requête
         1. ✅ Premiers champs basiques
         2. ✅ Catégories & sous catégories
            1. ✅ Sous requête à créer
            2. ✅ CONCAT pour hiérarchisation
            3. ✅🐛 Libellés doivent correspondre avec WC (ajoutés a la main & corrigés par max)
            4. ✅ Gestion des `'`, `"`, `\` et autres joyeusetés
            5. ✅🐛 sous catégories homonymes
            6. ✅📌 Tester import
            7. ✅ Sauvegarder CSV de test
            8. ✅ Maj boilerplate
            9. ✅ Maj voitures
         3. ✅🧽 Clean décalage sur export linté
         4. ✅ Suite et fing
         5. Maj suite aux retours de Cédric 20/09/2022
      5. Export ancien site & import vers le nouveau site
      6. 📌 Tester
      7. 📧 Faire valider
   4. ✅ voitures
       1. Maj suite aux retours de Cédric 20/09/2022

## 16/09/2022

PB Modelisme

1. 🌱🔍 Réductions de prix réduit en cas de commande de multiples éléments
   1. 🌱 Plus tard et/ou à la main, ça me soule
2. ✅ Importer l'ensemble d'une catégorie de produits
    1. ✅ Requête SQL afin de créer le CSV correspondant, s'aider de 🧠 `_docs/craft-and-tests/16-XXX/04-XXX/01-annote-champs-a-virer.txt`
       1. ✅ Images voitures > `/_docs/craft-and-tests/17-craft-de-requete-sql-pour-export-csv_secret/README.md`
          1. ✅ boucler (sous requête ?)
             1. ✅ préfixer
          2. ✅ concaténer wo trailing ,
          3. ✅📌 Tester
             1. 🐛 Bug lors de l'import > `Impossible d’utiliser l’image « NULL »`
             2. ✅ Remplacer `NULL` par chaîne de caractères vides `''`
       2. ✅ Marques
          1. ✅📌 Vérifier si problème casse différente > Non
       3. ✅ Code barre & version
       4. ✅ Champs plugins
       5. ✅ Champs personnalisés
          1. ✅ Communs
          2. ✅ Véhicules
          3. ✅ Voitures
    2. ✅📌 Tester
       1. ✅ Import des 20 dernières voitures (les plus récentes) afin d'avoir du stock
       2. ✅🐛 Problème au niveau de l'import des images
    3. ✅🖐 Noter à faire à la main
    4. ✅ Sauvegarder dans secrets !
    5. ✅⬆️ Besoin de récupérer les dernières images uploadées afin de récupérer les derniers produits
       1. ✅ Récupérer sur ancien serveur
       2. ✅ Envoyer sur nouveau serveur
       3. ✅📌 Relancer import
    6. ✅📧 Faire valider
3. 🚀 Import l'ensemble des catégories
   1. ♻️ Global craft
      1. ✅ Template vertical pour champs deprecated 🔥
      2. 🚀 Récupération de l'intégralité des libellés de catégorie & sous catégorie de WC au format CSV
         1. Lint
            1. ✅ Virgules
            2. Réorganisation alphabétique
               1. ✅ Catégories
               2. 🚀 Sous cat
               3. sous sous cat
               4. sous sous sous cat -_-
               5. Diff & correspondance avec WC
   2. 🚀 accessoires
      1. ✅ Remplir complètement un produit sur le nouveau site, ajouter une catégorie pour export de cette catégorie
      2. ✅ Exporter le produit
      3. ✅ Linter le CSV
      4. 🚀 Créer la requête

Perso

1. ✅ Chateau sedan pour quand vigi reviendra [hey](https://www.chateau-fort-sedan.fr/evenements)

## 09/09/2022

PB Modelisme

1. ✅👪 RDV client jeudi 01/09/22
    1. ✅ RDV
    2. ✅ Cleaner compte rendu
       1. ✅📧 Envoi
    3. ✅ Mail Cédric, intégrer retours, [hey](https://mail.google.com/mail/u/0/#inbox/FMfcgzGqQJrPndBccNvXhJNvglQJpdvg)
2. 🚀📌 Finaliser les tests d'import : importer un produit avec l'ensemble des champs
    1. ✅📝 Détails `secrets > /_docs/craft-and-tests/16-tests-imports-finaux_secret/`
    2. ✅ Nettoyage final des champs problématiques
       1. ✨ Ci-dessous, à corriger dans 💾 doc structure, 🙎‍♂️ doc champs persos, ⚙️ champ perso, 📌 tests imports
       2. ✅ Rétablir champs legacy
          1. ✅💾✅🙎‍♂️✅⚙️✅📌 date dernier achat
       3. ✨ Legacy > Rajouter champs qui tapent dans les onglets
       4. ✅ Maquettes > Liste peintures
          1. ✨ Conserver le nouveau champ de type relation
          2. ✅💾✅🙎‍♂️✅⚙️✅📌 Ajouter le champ legacy original "PAINTLIST"
          3. Ajouter les 2 'nouveaux' champs légacy créés par Cédric
             1. ✅💾✅🙎‍♂️✅⚙️✅📌 RefPaintList / Références des peintures présentes dans la table accessoires. Poss multiples, séparateur `;`
             2. ✅💾✅🙎‍♂️✅⚙️✅📌 IDPaintList / Identifiant des peintures présentes dans la table accessoires. Poss multiples, séparateur `;`
       5. ✅📌 Tester import avec nouveaux champs remplis
    3. ✅ Prix importé en HT
        1. 📝 Site actuel PB, les prix sont TTC, mais doivent être importés en HT sur le nouveau site
        2. 💩 ~Import KO, les prix sont importés en TTC et casés tels quels en HT, malgré `taxable`
           1. ✅ Admin > WC > Réglages > TVA > Taux standards > Créer règles > `Pour tous, 20%`
           2. ~📌 Affichage OK mais 20% rajoutés au tarif déjà en TTC, il faut les retirer avant l'import
        3. ✅📌 Calcul TTC vers HT
           1. [Doc](https://www.clicfacture.com/calculette-tva-convertir-montant-ht-ttc/)
           2. `HT = TTC ÷ [1 + (taux de TVA / 100)]`
           3. 🚨 Arrondi
           4. 🚨 Convertir tarif promotionnel également
           5. 🚨 Séparateur de virgule est un point `.`
           6. ✅📌 Import & affichage sur site
           7. 🐛 Dans le menu, widget panier, le prix est affiché en HT
    4. 🌱🔍 Réductions de prix réduit en cas de commande de multiples éléments
       1. 💩✌️ Check quantité voir si à la maing > Accessoires + de 500
       2. 📝 Plugin original : Tarification dynamique avancée pour WooCommerce
       3. 📝 Dans l'admin > WC > Règles de tarification
       4. ✅ Création d'une règle à la mano
       5. 💩 Test export voir si on récupère
          1. 📝 Possibilité d'importer des règles via Admin > WC > Règles de tarification > Outils > Import rules
          2. 💩 Pas de récupération dans l'export classique + la réduction n'est pas sur la fiche produit
       6. 🔍 Recherche autre plugin
          1. 💩💩💩 [Conditional Discounts for WooCommerce](https://fr.wordpress.org/plugins/woo-advanced-discounts/)
             1. Indiqué comme payant sur le site ?
             2. D'après les screenshots, inclus à l'onglet WC sur la page produit
             3. 💩📌 Complètement payant
          2. 💩 [Discount Rules and Dynamic Pricing for WooCommerce](https://fr.wordpress.org/plugins/easy-woocommerce-discounts/)
             1. A priori freemium avec ce qu'on veut
             2. 💩 Mwé, mais déconne à balle pour le calcul des prix
          3. 💩 [Booster for WooCommerce](https://fr.wordpress.org/plugins/woocommerce-jetpack/)
             1. Freemium, ca a vraiment l'air d'un piege a con a l'instinct
             2. 100k trucs, imbitable
          4. 🌱 Plus tard et/ou à la main, ça me soule
    5. ✅💥 [Guidelines](https://woocommerce.com/document/product-csv-importer-exporter/#general-guidelines)
       1. Attention pour les **nombres décimaux** : remplacer séparateur "." par virgule ","
          1. ✅📌 A vérifier, lors de l'export de contrôle les décimaux (pour les **champs classiques de woocommerce**) `"Longueur (mm)"` utilise un point `46.6`
             1. Non, utiliser des points
       2. Use 1 or 0 in your CSV, if importing a Boolean value (true or false)
       3. Multiple values in a field get separated with commas.
       4. Wrapping values in quotes allows you to insert a comma.
       5. Prefix the id with id: if referencing an existing product ID. No prefix is needed if referencing an SKU. For example: id:100, SKU101
       6. It is not possible to assign a specific post ID to product on import. Products will always use the next available ID, regardless of the ID included in the imported CSV.
       7. Pas de serialisation dans les données
    6. ✅ Import des images produits
        1. [Doc](https://woocommerce.com/document/product-csv-importer-exporter/#images)
        2. Tester avec images sur le même serveur
           1. ✅ Uploader les images
           2. ✅ Modifier le csv d'import
           3. ✅📌 Tester
              1. 💩 Images avec chemin relatif ?
              2. ✅ Chemins absolus
    7. ✅🙊 Sauvegarder tests dans repo secret

Effy art tattoo

1. ✅ Installation WordPress & configuration basique
2. ✅ Admin > Réglages
   1. ✅ Utilisateurs
3. ✅ Installer theme divi + license
4. ✅ 🔍 Inspiration
   1. [sktchd](https://www.divilayouts.com/wp-content/uploads/2017/05/sktchd-4-page-tatoo-layout.jpg)
   2. [tattooz](https://divireadythemes.com/tattooz/)
   3. [tattoo](https://www.divione.com/tattoo/)
5. ✅ 🔍 Theme de base
   1. [Restaurant](https://www.elegantthemes.com/layouts/business/restaurant-home-page)
   2. [Butcher](https://www.elegantthemes.com/layouts/business/butcher-landing-page)
   3. [~~Bar~~](https://www.elegantthemes.com/layouts/food-drink/bar-landing-page)
6. ✅ Page d'accueil : Blocs
   1. ✅ Métier & localisation
      1. Butcher > home 1
   2. ✅ Profil
      1. Butcher > home 2
   3. ✅ Derniers encrages
      1. Farmers market [landing page](https://www.elegantthemes.com/layouts/business/farmers-market-landing-page)
   4. ✅ Projets préférés / mis en avant / Différents styles
      1. Restaurant > home > grille
   5. ✅ Nombre de réalisations qui défilent
      1. Cooking school > [home](https://www.elegantthemes.com/layouts/food-drink/cooking-school-home-page/live-demo)
   6. ✅ Galerie
      1. Restaurant > Gallery
      2. Lien vers page dédiée
   7. ✅ Témoignages
      1. Restaurant > home
   8. ✅ Disponibilité
   9. ✅ Horaires / Contact / Réserver
       1. Restaurant > Contact en bas
   10. ✅ Expérience, ~trucs santé sécurité hygiène, normes encres, etc.
7. ✅ Logo ~~scarabay~~ + Favicon
   1. ✅ Rapport avec tattoo > encre
8. ✅ Couleurs
   1. ✅ Site ~Noir / foncé
   2. ✅ Dominante Noble red **#92181d**
9. ✅ Polices
   1. Titres [Kaushan Script](https://fonts.google.com/specimen/Kaushan+Script?slant=7)
   2. Textes [Cairo](https://fonts.google.com/specimen/Cairo?query=cairo)
10. ✅ Contenus
    1. ✅ Photos
    2. ✅ Textes
    3. ✅ Relire à tête reposée
11. ✅ Photos fonds intro & contact
12. ✅ Virer images inutiles
13. ~~Page galerie~~ > Liens vers insta
    1. ✅ Lien sur page accueil
14. ✅ Plugin calendrier
15. ✅ [Réseaux](https://effy-art-tattoo.com/wp-admin/admin.php?page=et_divi_options)
16. ✅ Pages profondes
    1. [Mentions légales & crédits](https://effy-art-tattoo.com/mentions-legales/)
    2. [RGPD blah](https://effy-art-tattoo.com/rgpd-politique-confidentialite/)
17. ✅ Footer + liens pages profondes
18. ✅ Contact lien vers salon tattoo
19. ✅ Passer en https Admin > Réglages > Général
20. ✅ Ajuster horaires
21. ✅💾 Backups
    1. ✅ BDD
    2. ✅ AI1WPM
22. ✅ Images dans drive
23. ✅📱 Cleaner responsive
    1. Tel
       1. ✅ Global
          1. ✅ Revoir marges verticales
          2. ✅ Séparateurs des différentes parties à revoir > bordure basse rouge 2px
       2. ✅ Partie 1 / intro
          1. ✅ Hauteur minimale
          2. ✅ Rétrécir bouton
       3. ✅ Partie 2 / A propos
          1. ✅ Titre 2 lignes max, réduire
       4. ✅ Chiffres défilent
          1. ✅ Passer chacun en horizontal
       5. ✅ Prestations
          1. ✅ Revoir ordre
          2. ✅ Bouton insta mal placé
       6. ✅ Témoignages
       7. ✅ Contact
          1. ✅ Réduire marges ext. horizontales
          2. ✅ Réduire taille police, Pas de passages à la ligne
       8. ✅ Footer
          1. ✅ Marges aussi
          2. ✅ Garder une marge en bas pour ne pas gener le clic sur les RS
    2. ✅ Tablette
       1. ✅ Audit après correction tel
       2. ✅ Repasser sur l'ensemble des points ci-dessus
    3. ✅ Vérifier que rien n'a sauté sur Desktop
    4. ✅ Re-test sur tel
    5. Check viteuf en paysage
       1. Tel
       2. Tablette
24. ✅ Redirection autre [nom de domaine plus court :)](http://effy-tattoo.art/)
25. Optimisations
    1. [Pagespeed insight](https://pagespeed.web.dev/report?url=https%3A%2F%2Feffy-art-tattoo.com%2F&hl=fr&form_factor=mobile)
       1. ✅ Mobile, avant **score de 78, FCP 2.8s, TTI 5.2s**
          1. ✅ Convertir les images (plugin wp ?) > test nouveau "Converter for media"
          2. Temps de réponse du serveur :/
          3. Charger/écrémer les polices google web fonts
          4. ✅ `.htaccess` définir des règles de cache
          5. ✅ Plugin de cache > test nouveau "WP Fastest Cache"
          6. Optimisation à la mano de 3 images lourdes
          7. Pas de diff de score de ouf, FCP à baissé un peu, à cause du temps de réponse serveur et de subitilités du cache (fichiers >) mais pour l'utilisateur ça pulse
    2. ✅ [Pingdom](https://tools.pingdom.com/#60c6a6687e400000)
       1. avant **score de B 83, Load 1.13s, Page size 1.6mb**
       2. ⚡️ après **score de A 91, Load 393ms, Page size 848.5kb**
    3. ✅ [gtmetrix](https://gtmetrix.com/reports/effy-art-tattoo.com/4i2hzVkT/)
       1. avant **C, Perf 68%, Structure 92%, LCP 2.8s, TBT 47ms**
       2. ⚡️ après **A, Perf 95%, Structure 97%, LCP 1.2s, TBT 0ms**
26. ✅ Référencement naturel
    1. ✅ Partages RS [open graph](https://www.elegantthemes.com/blog/tips-tricks/how-to-add-open-graph-tags-to-wordpress)
    2. ✅ sitemap.xml
    3. ✅⏳ robots.txt
    4. ✅ activation google search console
    5. ✅ Associer à google analytics
       1. ✅⏳ Tayste
       2. ✅ Maj Politique de confidentialité
27. ✅ Formulaire de contact qui fonctionne
    1. ✅ Configurer envoi de mail
    2. ✅📌 Tayste
    3. ~✅ Configurer envoi de [mail++](https://docs.ovh.com/fr/dedicated/optimiser-envoi-emails/)
       1. ✅✨ SPF / Déjà en place sur OVH
       2. 💩 [DKIM](https://dkimcore.org/tools/keys.html)
          1. ✅ Sauvegarde des clés dans les secrets
          2. ✅ Publique dans DNS
          3. 💩 Privée en sortie de mails / Pas possible sur mutualisé
       3. 💩🌱 [DMARC](https://support.google.com/a/answer/2466563?hl=fr)
          1. 💩 Dépendant de DKIM
28. ⏳📌 Après avoir montré le site à Ophé
    1. ✅ Changer mail
       1. ✅ Utilisateur ophélie
       2. ✅ Formulaire de contact
          1. ⏳📌 Tayste > Envoi à ophélie, en attente de confirmation
    2. ✅ Envoyer les identifiants de connexion
29. ⏳ Check google search console
    1. ✅ Ajouter Ophélie aux stats
    2. ✅ Configurer
    3. ⏳📌 Check [mise en place](https://search.google.com/search-console?resource_id=sc-domain%3Aeffy-art-tattoo.com&hl=fr)
    4. Appliquer recommandations
30. ⏳ Analytics
    1. ✅ Configurer
    2. ⏳📌 Check [mise en place](https://analytics.google.com/analytics/web/#/a241007713p331735161/admin/streams/table/4060071527)
    3. ⏳📌 robots.txt

## 02/09/2022

PB Modelisme

1. ✅ Retours nouvelles pages > Rajouté à la réunion du jeudi 01/09
2. ✅🔍 Retours RDV clients : Fonctionnalités++ a mettre en place
   1. ✅ Vente a l'étranger
      1. ✅📧 Retour client
   2. ✅ Sauvegarde automatique du panier
      1. ✨ Déjà en place dans WC par défaut (~besoin d'accepter les cookies)
      2. ✅ Fonctionnalité avancée > suggestion de 2 plugins
         1. [WPC Save For Later for WooCommerce](https://fr.wordpress.org/plugins/wc-save-for-later/)
            1. [Démo](https://demo.wpclever.net/woosl/)
            2. Possibilité de séparer des produits du panier pour les "acheter plus tard"
         2. [WPC Smart Wishlist for WooCommerce](https://fr.wordpress.org/plugins/woo-smart-wishlist/)
            1. [Démo](https://demo.wpclever.net/woosw/)
            2. Possibilité de mettre en ~favoris / liste de souhaits, ce qui met en place une page similaire au panier
            3. Note : certains sites l'utilisent afin d'offrir des cadeaux lors de grosses commandes
      3. ✅📧 Retour client
   3. ✅ Devis à transformer en commande
      1. ✨ Voir si possibilité commerçant qui remplit panier du client (quand le client appelle)
         1. Possibilité de créer une commande depuis l'administration
      2. ✅👌 Plus propre : installation du plugin [Ni WooCommerce Custom Order Status](https://fr.wordpress.org/plugins/ni-woocommerce-custom-order-status/)
         1. Ajout d'un statut propre aux devis
         2. Propose également des [statistiques](https://dev.pb-modelisme.com/wp-admin/admin.php?page=ni-custom-order-status-report)
      3. ✅📌 test devis
      4. ✅📧 Retour client
   4. ✅ Ajouter un état produit : "Produit plus fabriqué" ~possibilité d'avoir en stocks mais ne sera pas renouvelé
      1. 🔍 [Trad "discontinued"](https://barn2.com/woocommerce-product-discontinued-status-plugin/)
      2. ✅ Gestion propre via plugin [Discontinued Product Stock Status for WooCommerce](https://fr.wordpress.org/plugins/discontinued-product-stock-status-woocommerce/)
         1. Possibilité d'afficher ou non ces produits
         2. Message global ou personnalisé par produit (suggestion nouveau produit !)
      3. ✅📌 test produit discontinued
      4. ✅📧 Retour client
3. ✅🔍 Checker rapidement le nouvel [ACF 6.0 RC](https://www.advancedcustomfields.com/blog/acf-pro-6-0-rc-1/)
   1. Retro compatible > installer
      1. ✅💾 Sauvegarder cazou
      2. ✅⬆️ Migrer
4. ✅🔍 Veille [suggestions de plugins](https://dev.pb-modelisme.com/wp-admin/admin.php?page=pwb_suggestions)
   1. ✅📝 Notes + versionner
   2. ✅📧 CR client
5. ✅ Menu principal > tester plugins & cleaner
   1. ✅🔍📌 3 choix, tester
      1. ✅ meh ~~[Max mega menu](https://wordpress.org/plugins/megamenu/)~~
         1. Pas über intuitif, un poil vieux
         2. Responsive impecab'
      2. ✅ ~~[theme um  > WP Mega Menu](https://www.themeum.com/product/wp-megamenu/)~~ > Maj 10 mois :/
         1. Littéralement le même que celui d'avant avec du drag & drop côté administration
         2. Possibilité de bien customiser en admin wp
         3. 💩 Responsive KO ~~à priori~~
      3. 💩 [QuadMenu – Divi Mega Menu](https://quadmenu.com/divi/) / Pas maj depuis > 1 an
         1. KO à l'installation
      4. ✅🎉 [WordPress Mega Menu – QuadMenu](https://quadmenu.com/) / Maj récentes mais trop de trucs en premium ?
         1. Page d'options sympa, beaucoup de custom dispo
         2. Possibilité d'ajouter du css dans l'admin
         3. 🚨 Attention
            1. Items pour menu principal
            2. Widgets pour Mega > Columns (s'affiche uniquement quand colonne sélectionnée !)
            3. Pas mal d'options dans Mega (autres que colonnes)
   2. ✅ Création du menu principal au mieux
      1. ✅ Fil de l'eau
         1. ✅ 📱 Vérification responsive
      2. ✅ Contenus
         1. ✅ Avions
         2. ✅ Hélico & Drones
         3. ✅ Voitures
         4. ✅ Bateaux
         5. ✅ Maquettes
         6. ✅ Accessoires
         7. ✅ Matériaux
      3. 🌱💩💩💩💩💩💩💩💩💩💩💩💩 Ajouter blocs usuels
         1. ✅ Panier
         2. ✅ Recherche
         3. 💥💥💥🤑💩 Connexion > Premium
      4. ✅ Visuels
         1. ✅ Eclater menu de base pour éviter les bugs graphiques
            1. ✅ Apparence > perso
            2. 💩 Divi > tout > options à moitié KO
            3. ✅ CSS kustom FTW
         2. ✅ Changer logo > Garder logo divi & virer logo menu
         3. ✅ Changer polices > Laisser divi gérer
            1. 🚨 Taille & épaisseur dans quandmenu obligatoirement :/
         4. ✅ Changer couleurs
         5. ✅ Changer espacement vertical 🚨 desktop uniquement
         6. ✅📱 Idem responsive
            1. 🐛 Virer burger menu en trop
         7. ✅ Desktop > revoir taille logo
         8. 🤏🌱 Bandeau sup (panier tel mail) > CSS kustom FTW
            1. ✅ Desktop > virer panier
            2. 🤏🌱📱 Revoir Mobile
         9. ✅ Logo PB sur menu quand et non menu normal c'juste pas possible
         10. ✅📱 Check [tablette](https://dev.pb-modelisme.com/wp-admin/customize.php?return=%2Fwp-admin%2Fadmin.php%3Fpage%3Dwc-settings%26tab%3Dadvanced%26section%3Dfeatures)
         11. 🌱 Check desktop faible ~ entre 980px et 1280px
      5. ✅💬 Notes pour clients
         1. [Prestations dans accessoires ??](https://pb-modelisme.com/Accessoires/listeprod.php?cat=35)
         2. Menu > accessoires > redondance avion bateaux voitures helico
         3. Partie dédiées outillage, aerographe, pièces détachées, partie dédiée destockage
            1. Reco max : effets spéciaux décors (still water, boues, pigments, etc.)
         4. "Grosses" catégorie (centre d'inérêt++) avec image illustration
6. ✅ Repasse catégories
   1. ✅ Tout passer en pluriel
   2. ✅ Plus d'homonymes
   3. ✅ Véhicules > slugs préfixés de la catégorie parente
   4. ✅💬 Notes pour clients
      1. Il y a énormément de catégorie redondantes / inutiles, ex matériaux > plaques
         1. Ptet voir pour faire une grosse repasse et faire des catégorie générales, avec des taxonomies
            1. Ex: plutôt que "plaque lisse blanche" "plaque lisse noire" "plaque pavage" > plaque avec attributs couleur & texture...
            2. "Tube carré" "Tube rond" >> Tubes > forme
            3. "Décor - " y'en a plein x)
            4. Idem pour les matières "XXX en métal"
      2. Eclater les catégories actuelles > simplifier avec un sujet et des compatibilités (ex: roues + compat. voiture)
      3. dans menu pourquoi cat. générales & cat. marques ? ex: Matériaux > "Outillages" & "Outillages Proxon"
7. ✅💬 Compiler notes clients puis mail
8. ✅⬆️ Maj WordPress 6.0.2
   1. ✅🔍 Changelog
9. ✅🔥 Lien mort dans menu Drones "Suivez notre guide (tout en bas)." > retour de Cédric, à supprimer
10. ✅👪 Prévoir RDV client jeudi 01/09/22
11. ✅🔍 Veille
    1. [Autocomplete WC orders](https://fr.wordpress.org/plugins/autocomplete-woocommerce-orders/)
12. ✅ Footer > ajouter logo paypal
13. ✅💩 Installer plugin [wishlist](https://fr.wordpress.org/plugins/woo-smart-wishlist/)
    1. 📌 Tester que ça pète pas tout & que ça fonctionne
       1. 💩 Gros bouton texte moche ?
       2. [Traductions](https://dev.pb-modelisme.com/wp-admin/admin.php?page=wpclever-woosw&tab=localization)
       3. 💩 Comportement KO (erreurs Ajax)
14. 🚀📌 Finaliser les tests d'import : importer un produit avec l'ensemble des champs
    1. ✅📝 Détails `secrets > /_docs/craft-and-tests/16-tests-imports-finaux_secret/`
    2. 🚀 (Re)mise en place
       1. ✅🔍 Relire les notes sur les anciens tests d'imports
       2. ✅ Ancienne BDD : Export basique produit récent + test CSV sur requête SQL particulière
       3. ✅ Nouveau site : Export d'un produit afin de voir la structure liée à l'ensemble des nouveaux champs personnalisés
          1. ✅ Remplir & noter les données du produit afin de référencer l'ensemble des champs..
             1. ✅ WordPress
             2. ✅ WooCommerce
             3. ✅ Champs personnalisés (ACF)
             4. ✅ Ajouter une catégorie "_Test export"
          2. ✅🔍 Relire les ressources associées
          3. ✅ Admin > WC > Export
             1. ✅ Catégorie "_Test export" uniquement
             2. ✅ Export Custom Meta
       4. ✅🔍 Analyse de la structure du fichier CSV d'export, 🧮 ~190 champs dont ~40 WP/WC ~150 persos
          1. ✅ Vérifications, différences, notes, problèmes
          2. ✅ Annoter simplement, cf. `secrets > /_docs/craft-and-tests/16-tests-imports-finaux_secret/02-nouveau-site-export-un-produit/export-avec-champs-personnalisés---identifiants-et-valeurs-d-exemples.txt`
          3. ✅📌 Vérifier valeurs entre admin & csv
             1. ✅🐛 Champ voitures > dimensions avancées > valeurs différentes ?
                1. 🧠 Lié à la mise à jour des champs personnalisés : passage de cm à mm > nouveaux champs & résidus invisibles dans l'admin ACF, mais conservés en BDD. Rien à corriger, juste 🧽⚰️ cleaner export de base pour retirer le deprecated
             2. ✅👥 Manquants ?
                1. ✅ WordPress
                   1. url si personnalisée
                   2. Pas de date de publication
                2. ✅ WC > OK
                3. ✅🐛 Champs ACF > 🧠 Instinct ok > champs avec **passage produits en référence** (pos. multiples)
       5. ✅📌 Virer id, changer nom & sku, tester réimport oké
          1. ~🐛 Is ok en dehors des champs relation
       6. ✅🧽⚰️ Cleaner des champs deprecated ou inutilisés
          1. Doc export > champs classiques
          2. Nouveau produit > export > diff
             1. ACF deprecated / pas de possibilité de virer l'historique :'(
             2. les champs divis, status wp, etc.
       7. 🚀 Rétablir champs legacy dernier achat date & prix pour éviter conversion complexe en répéteur ? avec nouveaux champs dispos pour nouveau site
       8. Idem champs requêtes onglets, si besoin de taper dedans (affichage conditionnel > onglet vieux contenu ou onglet données nouveau site)
       9. 🌱 Liste peintures des maquettes > Faire à la main via requête sql `SELECT * FROM maquette WHERE QUANTITEM > 0 AND PAINTLIST IS NOT NULL ORDER BY PAINTLIST DESC` pour savoir lesquelles faires
          1. ET SURTOUT demander a cédric de convertir en références/CDACCESSOIRES ! sinon galères
       10. Rajouter tout ça a l'import
    3. Prix importé en HT
        1. Import OK
        2. Affichage sur site ?
        3. Calcul TTC ok ? arrondi machin mes couilles
    4. ✅ Catégories : si plusieures elles sont séparées par des virgules, si hiérarchie `>`
    5. ✅ Marques : si plusieures, séparées par des virgules
    6. ✅ Codes barres : plugin | ACF > un champ pour chaque code barre, ça reste du texte
    7. 🔍 Réductions en cas de prix réduit pour commande de multiples éléments
       1. Check quantité voir si à la maing ✌️ > Accessoires + de 500
    8. ✅ Produits associés

## 26/08/2022

Perso

1. ✅ Virement loyer/emprunt

PB Modelisme

1. ✅ WP > Création des champs personnalisés
    1. ✅ Repasse sur doc BDD drive, suite aux retours de cédric
       1. ✅ Batterie
          1. ✅ CDACC > Type de prise sur accus. Un produit dans table accessoire
             1. ✅ Maj doc champs persos
             2. ✅ Maj WP champs persos
          2. ✅ Serie & Para > Pas legacy
             1. ✅ Maj doc champs persos
             2. ✅ Maj WP champs persos
          3. ✅ Helico > cylidrée min & max > Uniquement helico thermique
             1. ✅ Maj doc champs persos
             2. ✅ Maj WP champs persos
          4. ✅ radio > BRAIN & RXEM
             1. ✅ Maj doc champs persos
             2. ✅ Maj WP champs persos
    2. ✅🧽 Revoir gestion de l'utilisation du moteur (pour le moment catégorie "Moteurs" avec les véhicules compatibles)
        1. ✅ Et deux catégories vides "Moteurs thermiques" et "Moteurs électriques"
           1. ✅ On conserve
        2. ✅♻️ Refacto ? sur un champ "compatibilité" ? pour affecter aux autres catégories qui pourraient en avoir besoin
           1. 📝 Actuellement
              1. Moteurs
                 1. Bateau
                 2. Hélico
                 3. Moteurs avions
                 4. Planeur
                 5. Turbine
                 6. Voiture
              2. Moteurs électriques
              3. Moteurs thermiques
           2. ✅ Refacto / Compatible / moteurs-compatibles-
              1. ✅ Compatibilité moteurs
                 1. ✅ Compatible avions
                 2. ✅ Compatible bateaux
                 3. ✅ Compatible hélicos
                 4. ✅ Compatible planeurs
                 5. ✅ Compatible turbines
                 6. ✅ Compatible voitures
    3. ✅💾 Backup de fin
2. ✅ Gestion retours Cédric [dernier mail](https://mail.google.com/mail/u/0/#inbox/FMfcgzGqPzFxzJdDMktFtKZHsRmrhLrL)
   1. 📝 Pour les liens à rajouter : "Avez vous pensez à ..." où "Avez vous besoin de ..."
   2. ✅ Avions > Ajouter un onglet produits associés
      1. ✅ Maj doc BDD
      2. ✨👪 Maj WP > champs persos
   3. ✅ Moteur électrique
      1. ✅ Notice > C'est juste un lien, on garde
         1. ✅ Maj doc BDD
         2. ✨👪 Maj WP > champs persos
      2. ✅ Produit compatible > On garde pas, on mettra des produits associés
         1. ✅ Maj doc BDD
         2. ✨👪Maj WP > champs persos
      3. ✅ Autres onglets > Affichage en dur d'une catégorie
         1. ✅ Maj doc BDD
   4. ✅ Moteur thermique > Onglet indispensable > On remplace par plusieurs liens * vers les catégories suivantes : durites, filtre, réservoir, clef à bougie, Glow starter
      1. ✅ Maj doc BDD
   5. ✅ Voiture
      1. ✅ Accessoires Camion > On remplace par un lien* vers tous les accessoires camion
         1. ✅ Maj doc BDD
      2. ✅ Indispensables > On remplace par des liens * vers les rubriques suivantes : Huile diff & Amorto / Pignon moteur / Clip carrosserie / Filtre à air
         1. ✅ Maj doc BDD
   6. ✅ Tout passer en mm, en non en cm
      1. ✅ Maj doc BDD
      2. ✅ Maj doc champs persos
      3. ✅ Maj WP > WC > Réglages
      4. ✅ Maj WP > champs persos
3. ✅ Importer les marques
    1. ✅ Elimination des doublons, chaque marque n'a qu'une entrée
    2. ✅ Plus de marquées dédiées à certaines catégories, que des marques générales
    3. ✅ Hiérarchie / familles de marques
4. ✅ Tâches prioritaires suite au RDV client
    1. ✅ Créer les pages statiques & pré-remplir le contenu
       1. ✅ à propos (theme bike)
          1. [originale](https://www.pb-modelisme.com/presentation.php)
          2. [base](https://dev.pb-modelisme.com/brs-a-propos/)
          3. [nouvelle](https://dev.pb-modelisme.com/a-propos/)
       2. ✅ services (theme bike)
          1. [base](https://dev.pb-modelisme.com/brs-services/)
          2. [nouvelle](https://dev.pb-modelisme.com/services/)
       3. ✅ Un service
          1. [base](https://dev.pb-modelisme.com/brs-service/)
          2. [nouvelle](https://dev.pb-modelisme.com/services/reparations/)
       4. ✅ Actualités / blogs (theme hardware store)
          1. [base](https://dev.pb-modelisme.com/hs-blog/)
          2. [nouvelle](https://dev.pb-modelisme.com/actualites-blog/)
       5. ✅ contact, fusionner avec "nous situer"
          1. Originale [nous situer](https://www.pb-modelisme.com/acces.php) [nous contacter](https://www.pb-modelisme.com/contact.php)
          2. [Nouvelle](https://dev.pb-modelisme.com/contact/)
          3. ✅ Adresse
          4. ✅ Gmaps
             1. ✅ clé API > besoin infos paiement même si c'est gratuit > 3 mois max
             2. ✅ Alternative > ~~Leaflet maps~~ > WP GO Maps (plus d'installations)
                1. ✅ Installation
                2. ✅ Config
                3. ✅ Vérification responsive ok
          5. ✅ Horaires
          6. ✅ Formulaire de contact
          7. ✅ Venir au magasin > Récupérer trucs Champagne Lapie > gmaps & ways instant
       6. ✅ page des marques
          1. ✅ [Originale](https://www.pb-modelisme.com/liens.php)
          2. ✅ [Nouvelle](https://dev.pb-modelisme.com/marques-partenaires/)
             1. ✅🔍 [Doc plugin](https://quadlayers.com/documentation/perfect-woocommerce-brands/?utm_source=pwb_admin)
             2. 🌱 Traduction "Brands" dans le fil d'arianne sur une page "marque"
       7. ✅ Mentions légales
          1. ✅ Originale > [popup dans footer](https://pb-modelisme.com/)
          2. ✅ [Nouvelle](https://dev.pb-modelisme.com/mentions-legales/)
          3. ⏳ Retours PB
             1. "le site pb-modelisme.com est déclaré à la CNIL sous le numéro **123456789**" < **SUSPICION**
             2. Textes et photos non contractuels
       8. ✅ Conditions générales de vente
          1. ✅ Originale > [popup dans footer](https://pb-modelisme.com/)
          2. ✅ [Nouvelle](https://dev.pb-modelisme.com/conditions-generales-vente/)
             1. Corrections typos
             2. ⏳ Retours PB
                1. Uniformiser nom de la société sur l'ensemble des pages mentions "PB-MODELISME" "PB MODÉLISME" "PB Modélisme" "PB MODELISME"
                2. 3 Commandes > 3.2 > Re-phraser ? Un poil familier
                3. ⏳ Faire une grosse relecture avant que j'arrange la disposition des textes
       9. ✅ RGPD Politique de confidentialité & Cookies
          1. Générée auto : [Nouvelle](https://dev.pb-modelisme.com/rgpd-cookie-politique-confidentialite-eu/)
    2. ✅ Footer / Pied de page
       1. ✅ Note : ~~Apparence > perso > widgets~~ Divi > theme builder
       2. ✅ Design > faire un mix de BRS et HS
          1. BRS plus sympa mais pas d'adresse ni de newsletter
       3. ✅ Faire une proposition de menu (trier les anciens liens)
          1. Contact
          2. A propos
          3. Services
          4. Marques
          5. Actualités
          6. Mentions
          7. CGV
          8. Cookies
          9. Plan du site
       4. ✅ Reprendre les images bancaires du pied de page de l'ancien site
       5. ✅ Copyright, avec année automatique
       6. ✅ Cleaner logo gouvernement plan relance
       7. ✅ Tester footer full page
          1. ✅ Enregistrer templates full & pas full (pour switch)
          2. ✅ Check responsive
          3. ✅ Screeshots propositions clients
    3. ✅ Cleaner contenus menus
    4. ✅ Repasse sur le carousel de la page d'accueil
    5. ✅ Correction à la volée de certaines catégories avec noms similiares (sous catégories..)
    6. ✅ Créer un compte admin pour PB Modelisme
       1. ✅ Créer le compte
       2. ✅ Noter identifiants dans doc secret
       3. ✅ 📧 Envoyer identifiants avec liste des pages admin à recetter
       4. ✅ Même chose pour nonore
    7. ✅ Mail PB & ALD liste des pages à recetter

## 19/08/2022

PB Modelisme

1. ✅⬆️ Mise à jour plugins, thèmes, traductions WP
2. ✅ Améliorations WP classiques
   1. ✅🔒️ Attente https
   2. ✅ WP admin > Santé du site
      1. ✅ Retirer extensions inactives > attente fin du développement
      2. ✅ Evènement planifié en retard > Rien trouvé dans l'onglet correspondant
      3. ✅ Maj d'arrière plan POURRAIENT être KO > Il a juste détecté le git
      4. ✅ HTTPS dans la config
         1. ✅ Revoir BDD
         2. ✅ Revoir wp-config & réglages > général
         3. ✅ Régénérer permaliens
   3. 💩 Vérifier Erreurs console ? Ressources dans wp-include/ en 404 > Besoin https
      1. ✅💾 Backup BDD avant
      2. 💩 Changer toutes les urls des fichiers médias
         1. 💩 Ca merde, soit l'import est HS, soit fait sauter la config divi
      3. 🌱 Voir plus tard > éclater tout avant import
   4. ✅ Mise en place de l'extension pour les marques > WPC Brand
      1. ✅ 💩 Rajoute du contenu sur la page d'accueil + KO + erreurs consoles
      2. ✅ 🔍 Autre plugin
         1. ✅ [Perfect Brands pour WooCommerce](https://fr.wordpress.org/plugins/perfect-woocommerce-brands/)
            1. Is ok mais éclate le tableau dans la page des produits
               1. `/plugins/perfect-woocommerce-brands/assets/css/styles-admin.min.css` > virer `width: 11% !important`
      3. ✅ Récupérer les images ~`https://pb-modelisme.com/Logo_Marque/XXX.jpg`
      4. ✅ Optimiser les images pour un meilleur référencement
         1. ✅ Renommer
            1. ✅ Tout en minuscule
            2. ✅ Remplacer " " & "_" par "-"
            3. ✅ Ajouter les textes sur les images, ex "BMF.pjg" > "bmf-bare-metal-foil-co.jpg"
            4. ✅ Virer les ids
         2. ✅ Virer les doublons
         3. ✅ Remplacement des mauvaises images (logo PB sur d'autres marques !?)
         4. ✅ Discriminer ceux utilisés sur le site ~100/400
            1. ✅ Pour les autres on récupère les images de l'ancien site
         5. ✅ Aller voir sur le net pour maj les logos
         6. ✅ Mise à jour des liens également
         7. ✅ Passer en png
         8. ✅ Recadrage propre
         9. Création image carrée / Bannière
         10. ✅ Suffixer "logo-brand"
      5. ✅ Injecter les marques dans le nouveau site `total de 409` yay
3. WP > Création des champs personnalisés
    1. ✅🙍‍♂️ Propre au produit / 📝✨ Ajout d'un produit pour tester les champs personnalisés
       1. ✅ pcedetthermik      > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/culasse-moteur-alpha-28-3-transfert-rtr/)
           1. ✅ OPTPCETH a virer
           2. ✅ COEFFPCETH a virer
       2. ✅ piece_heli         > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/accu-3-7v-500mah-sky-watcher-drone/)
       3. ✅ piece_voiture      > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/cale-triangles-arrieres-r-f-alu-oas/)
           1. ✅ OPTPCECAR > choix unique
       4. ✅ quartz             > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/quartz-hsb-fm27-075/)
       5. ✅ radio              > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/cr4s-avec-2-recepteurs/)
       6. ✅ recepteur          > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/recepteur-3-voies-pour-racer-3s/)
           1. ✅ SBUSRECEP a virer
       7. ✅ servo              > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/go-02servo-digital/)
    2. ✅🧽 Tous les champs booléens, remplacer "Ne sais pas" par "Non défini"
    3. ✅🧽 Tous les ensembles de champs > ordre 100
    4. 🧽 Revoir gestion de l'utilisation du moteur (pour le moment catégorie "Moteurs" avec les véhicules compatibles)
        1. Et deux catégories vides "Moteurs thermiques" et "Moteurs électriques"
        2. Refacto ? sur un champ "compatibilité" ? pour affecter aux autres catégories qui pourraient en avoir besoin
    5. 💾 Backup de fin

Perso

1. ✅ Croquettes chien
   1. ✅ Commandé
   2. ✅ Aller chercher
2. ✅ Jeu alakonn unlock 1st dragon
   1. Need pasture level 26 ? [hey](https://pillarofgaming.com/evony-the-kings-return/dragons-guide-and-how-to-obtain-dragons/)
      1. Need donjon & entrepot
   2. 300k gems [gems guide mais en gros c'la merde](https://pillarofgaming.com/evony-the-kings-return/gems-obtaining-guide/)
3. ✅ [Orga we warhammer](https://docs.google.com/spreadsheets/d/1VPE3STTiAxp2QXXSfQ36fRdWbYpTJ5odioZmtBJRTDQ/edit#gid=0)

## 14/08/2022

PB Modelisme

1. ✅ Inventaire champs personnalisés
   1. cf. `pb-modelisme--com/_docs/craft-and-tests/10-inventaire-champs-personnalisés_secret`
2. ✅👪 Questions à sylvie & cédric
   1. ✅📧 Mail envoyé
3. ✅🔍 Vérifier gestion des..
   1. ⏳ codes barres (= "EAN") : x2, fournisseur & pb
      1. cf. `pb-modelisme--com/_docs/craft-and-tests/09-codes-barres-barcode-ean`
      2. Impression : Passer par extension payante ou utiliser une librarie et coder un truc maison
      3. Politique concernant les x2, voir avec Cédric
   2. ✅ Notations, étoiles de 1 à 5 > Note PB Modélisme > Champ perso commun
      1. cf. `pb-modelisme--com/_docs/craft-and-tests/08-import-product-reviews-and-notes`
   3. ✅ Favoris > Pas utilisé sur le site, 1 seul champ par produit ? wat > is Produit affiché sur accueil, boolean
   4. ✅ Eco-taxe
      1. Voir avec Cédric comment c'est géré avant de partir trop loing
      2. Soit stocké en champ particulier, soir [plugin payant 39€](https://solutions.fluenx.com/produit/eco-participation-pour-woocommerce/)
         1. Si plugin payant voir comment importer
      3. Valeur simplement affichée sur facture finale > Champs personnalisés global
   5. ✅ Prix de vente club
      1. [Plugin gratuit bien caché](https://fr.wordpress.org/plugins/elex-woocommerce-role-based-pricing-plugin-basic/)
      2. `cf. pb-modelisme--com/_docs/craft-and-tests/12-prix-club`
      3. 🧠 Pas mal d'autres fonctionnalités proposées, notemment pour la gestion des rôles
   6. ✅ Vente multiples > prix réduits
      1. "Products bundle discount" / "bulk discount"
      2. [Tuto avec plugin gratuit (?)](https://quadlayers.com/product-bundles-in-woocommerce/)
         1. Plus pour des réductions sur ventes groupées
      3. Go [check](https://www.commercegurus.com/bulk-discount-plugins-woocommerce/)
         1. Tous gratuits à partir de #6
         2. ✅Plugin [Advanced Dynamic Pricing for WooCommerce](https://wordpress.org/plugins/advanced-dynamic-pricing-for-woocommerce/), d'après la description c'est good
            1. ✅📌 Tayste
               1. WC > Règles de tarification
               2. [Impecab' sur altitude 2000](https://dev.pb-modelisme.com/produit/altitude-2000/)
4. ✅🔍 Veille plugins existants croisés lors des recherches
   1. ✅ [Check plugins "wpc*" sur WordPress](https://dev.pb-modelisme.com/wp-admin/plugin-install.php?s=wpc&tab=search&type=term)
      1. Freemium mais le côté payant n'apporte pas grand chose, tout est déjà bien dispo
      2. cf. `pb-modelisme--com/_docs/craft-and-tests/13-veille-plugins-wpclever`
      3. ✅📌 [WPC Force Sells for WooCommerce](https://fr.wordpress.org/plugins/wpc-force-sells/)
         1. Création de packs de produits ! Avec possibilité d'ajouter des réductions, etc.
         2. [Impecab'](https://dev.pb-modelisme.com/produit/pack-avion-shirt-bonnet/)
      4. ~✅🔒️📌 [WPC Brands for WooCommerce](https://fr.wordpress.org/plugins/wpc-brands/)
         1. Gestion simplifiée des marques de produit & affichage des logos, etc.
         2. A l'air correct mais est KO et pète la page d'accueil à cause de l'absence de HTTPS
      5. ~💩📌 [WPC Composite Products for WooCommerce](https://fr.wordpress.org/plugins/wpc-composite-products/)
         1. Création de pack may mieux, à l'air vraiment rpévu pour ça (pas de greffon sur un produit, contrairement à force sells)
         2. Cela correspond mieux, mais une fois sur la page de apiement les prix sont chelous, a retester
         3. [Demo](https://demo.wpclever.net/wooco/product/composite-02/)
         4. La démo fonctionne correctement
      6. ✅📌 [WPC AJAX Add to Cart for WooCommerce](https://fr.wordpress.org/plugins/wpc-ajax-add-to-cart/)
         1. Ajouter au panier sans recharger la page, pas de config
      7. ✅ [WPC Grouped Product for WooCommerce](https://fr.wordpress.org/plugins/wpc-grouped-product/)
         1. Flemme de tester, ressemble aux deux autres pour les groupes de produits
         2. [demo](https://demo.wpclever.net/woosg/?utm_source=content&utm_medium=woosg&utm_campaign=wporg)
   2. ✅📌 [Moteur de recherche avancé freemium](https://fr.wordpress.org/plugins/ajax-search-for-woocommerce/)
      1. C'canon mais ça éclate le visuel de la barre de menu
5. ✅📝 Ajout des champs supplémentaires WooCommerce requis (avec défauts), non présents en BDD PB, permettra d'uniformiser
   1. 🌱 Quartz > 🚨💥 Nom a générer
6. ✅📝 Repasse sur les onglets > Infos manquantes, stocker comment ?
   1. ✅🧠 Possibilité d'aller voir les fichiers PHP du site
      1. Oh god nope, besoin de linter + très complexe : 🐢 trop grosse perte de temps je pense
      2. AFFCC utilisé pour la gestion de l'affichage de produits ?
         1. cf. `_dev/site actuel pb modelisme/Accessoires/_lint_max___prodassoc.php`
   2. ✅ accessoires
      1. Onglet **Produits Similaires**
      2. Mains dans le code > `/_docs/craft-and-tests/14-retro-engineering-onglets-fiches-produits`
      3. ✅👪📧 Bref, c'est la compliqué. 2 solutions :
         1. Voir avec Cédric pour récupérer l'intégralité des requêtes
         2. Beaucoup plus simple, demander la logique de la requête SQL pour chaque onglet & recoder !
7. ✅ Gestion des retours à mes questions, réponses de Cédric > Maj ce fichier & doc BDD
   1. ✅ Champs avec interogations sur accessoires
   2. ✅ Choix des unités de mesure
      1. ✅ cm & grammes
      2. ✅ [Maj de WC](https://dev.pb-modelisme.com/wp-admin/admin.php?page=wc-settings&tab=products)
      3. ✅ Maj Champs persos `/_docs/craft-and-tests/10-inventaire-champs-personnalisés_secret`
      4. ✅ Doc BDD
   3. ✅ Prix par défaut en HT, affiché en TTC
      1. ✅ [Maj de WC](https://dev.pb-modelisme.com/wp-admin/admin.php?page=wc-settings&tab=tax)
      2. ✅ Doc BDD
      3. ✅ Maj Champs persos `/_docs/craft-and-tests/10-inventaire-champs-personnalisés_secret`
      4. ✅ Prévoir tests & validation
   4. ✅⚰️ Prix club > deprecated
      1. ✅ Maj Champs persos `/_docs/craft-and-tests/10-inventaire-champs-personnalisés_secret`
      2. ✅ Doc BDD
   5. ✅⚰️ Champ commun FAV___ > Produits affichés sur le bandeau d'accueil du site > deprecated
      1. ✅ Maj Champs persos `/_docs/craft-and-tests/10-inventaire-champs-personnalisés_secret`
      2. ✅ Doc BDD
   6. ✅⚰️ Champ commun AFF___ > Produits affichés sur le bandeau d'accueil du site > deprecated
      1. ✅ Maj Champs persos `/_docs/craft-and-tests/10-inventaire-champs-personnalisés_secret`
      2. ✅ Doc BDD > Remplacé par doubles status > 🛒 status && catalog_visibility
   7. ✅ Eco-taxe > Affiché sur facture finale (& produit maintenant -_-) > Champ perso global
      1. ✅ Maj Champs persos `/_docs/craft-and-tests/10-inventaire-champs-personnalisés_secret`
      2. ✅ Doc BDD > Remplacé par doubles status > 🛒 status && catalog_visibility
   8. ✅ NBSTAR___ > Note PB Modélisme > Champ perso commun
      1. 📝 Sera différent des notes relatives aux avis clients
      2. ✅ Maj Champs persos `/_docs/craft-and-tests/10-inventaire-champs-personnalisés_secret`
      3. ✅ Doc BDD > Remplacé par doubles status > 🛒 status && catalog_visibility
8. ✅📝 Repasse sur les choix uniques > populer + ajouter champ "ne sais pas"
   1. ✅ accessoires
   2. ✅ acctx
   3. ✅ avion
   4. ✅ bateaux
   5. ✅ batterie
   6. ✅ bougie
   7. ✅ carburant
   8. ✅ chargeur
   9. ✅ controleur
   10. ✅ heliceavion
   11. ✅ helico
   12. ✅ maquette
   13. ✅ matprem
   14. ✅ moteur_electrique
   15. ✅ moteur_thermique
   16. ✅ pcedetthermik
   17. ✅ piece_heli
   18. ✅ piece_voiture
   19. ✅ quartz
   20. ✅ radio
   21. ✅ recepteur
   22. ✅ servo
   23. ✅ voitures
   24. ✅ Revoir majuscule première lettre de l'ensemble des libellés
9. ✅ Doc champs perso > Rajouter les champs en attente de reponse > format `legacy_XXX`
    1. ✅ accessoires
    2. ✅ acctx
    3. ✅ avion
    4. ✅ bateaux
    5. ✅ batterie
    6. ✅ bougie
    7. ✅ carburant
    8. ✅ chargeur
    9. ✅ controleur
    10. ✅ heliceavion
    11. ✅ helico
    12. ✅ maquette
    13. ✅ matprem
    14. ✅ moteur_electrique
    15. ✅ moteur_thermique
    16. ✅ pcedetthermik
    17. ✅ piece_heli
    18. ✅ piece_voiture
    19. ✅ quartz
    20. ✅ radio
    21. ✅ recepteur
    22. ✅ servo
    23. ✅ voitures
10. ✅ WP > Création des ~~catégories~~ attributs table "versboite" ARTF, etc.
    1. ✅🧽 Correction des fautes :3
    2. ✅🧽 Suppression de caractères invisibles chelous dans les textes
11. 🚀 WP > Création des nouvelles catégories (faire une repasse sur l'ensemble des tables)
    1. ✅📝📌 Faire la différence entre catégories & [attributs !](https://dev.pb-modelisme.com/wp-admin/edit.php?post_type=product&page=product_attributes)
       1. Notes : Les attributs...
          1. **peuvent** être rajoutés aux produits depuis la fiche produit > données produits > attributs
          2. sont communs à l'ensemble des produits
          3. sont affichés **automatiquement** dans l'onglet "Informations complémentaires", [ex](https://dev.pb-modelisme.com/produit/easyglider-electric-rr/).
             1. 🚨👀 Visibilité publique
          4. sont considérés comme des catégories (affichage dans admin) + [page dédiée](https://dev.pb-modelisme.com/product-category/version-boite/kit-artr/)
             1. Doivent effectivement être définis comme catégorie et pas seulement dans attribut WC si produit veut être considéré comme tel
             2. La catégorie peut prendre le pas dans le fil d'ariane (ex: version boite > Avions)
       2. ✅📌 Tester champs particuliers ACF, différences avec atrtibuts WC ?
          1. Non affiché par défaut
    2. ✅📝🚨 Privilégier choix uniques (select/radio/etc.) lorsque c'est possible
    3. ✅🧠📏 **Comment choisir le type de champ particulier**
       1. Rien en catégorie, c'est fait pour les ... catégories
       2. Commun à tous les produits
          1. Visibilité publique
             1. Attribut
          2. Visibilité interne
             1. ACF
       3. Spécifique à un produit ou un groupe de produit
          1. ACF
    4. ✅🧽 Cleaner les catégories créées prématurément
       1. ✅♻️ ~Avion > Niveau
       2. ✅♻️ ~Avion > Type
       3. ✅♻️ ~Bateaux > Type
       4. ✅♻️ ~Helico > Niveau
       5. ✅♻️ ~Voiture > type moteur
       6. ✅ Maj structure BDD
       7. ✅ Maj doc champs personnalisés
12. 🚀 WP > Création des champs personnalisés
    1. ✅💾 Backups afin de pouvoir ré-importer la structure en cas de problème
    2. ✅👪 Globaux
    3. ✅🏎️ Véhicules & maquettes uniquement
    4. 💥 Corrections liées au RDV client : Mettre à jour doc champs particuliers ET WP
       1. ✅ Champs commun
          1. ✅ Fournisseurs
             1. ✅ Passer en champ répéteur
             2. ✅ contenant lui-même un répéteur (passer prix d'achat + date) PAR fournisseur
             3. ✅ Virer divers > prix d'achat
          2. ✅✨🛒 Ajouter date dernière vente
             1. Existe déjà dans WC, en automatique : Admin > Statistiques > Produit
          3. ✅ (Onglet) Produits associés
             1. Ajouter une liste de produits, qui seront ajoutés a la main, très spécifique au produit
          4. 🌱 (Onglet) Produits similaires
             1. Requête qui essaie pour rapatrier de manière automatique
       2. ✅ Véhicules
          1. ✅ Matériel à prévoir
             1. ✅ Passer en champ commun
             2. ✅ Remplacer par une liste de produits
          2. ✅ Liste de peintures
             1. ✅ Ajouter une liste de produits
          3. ✅ Pièces détachées
             1. ✅ Ajouter une liste de produits
          4. ~~Articles conseillés~~ Il y a déjà Produits associés
             1. ~~Ajouter une liste de produits~~
       3. ✅ Avion
          1. ✅ (Onglet) Servos conseillés
             1. ✅ Possibilité d'en choisir a la maing OU d'afficher l'ensemble des servos d'une catégorie de servos
       4. ✅ Chargeur
          1. ✅ Produits compatibles
             1. ✅ Ajouter une liste de produits
    5. 🚀🙍‍♂️ Propre au produit / 📝✨ Ajout d'un produit pour tester les champs personnalisés
       1. ✅ accessoires         > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/pompe-eau-moteur-gazoline/)
       2. ✅ acctx               > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/potentiometre-pilot-6t/)
       3. ✅ avion               > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/twin-astir-ii/)
          1. ✅ DIAMINI maxi > Taille des hélices > permet d'éviter que l'hélice touche par terre, etc.
       4. ✅ bateaux             > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/peniche-le-picardie/)
          1. ✅⚰️ NBELEBAT a virer
       5. ✅ batterie            > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/batterie-lipo-37v-tx-mhd3s/)
       6. ✅ bougie              > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/bougie-5-turbo/)
          1. ✅ 4TPSGLOW > description du champ
          2. ✅⚰️WANKELGLOW a virer
       7. ✅ carburant           > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/rocket-fuel-flight/)
       8. ✅ chargeur            > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/pro-x4-4-sorties-4x100w/)
       9. ✅ controleur          > ✅✨ [exemple](https://www.pb-modelisme.com/Controvaria/detailCont.php?prod=197)
       10. ✅ heliceavion        > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/tri-pales-propulsive/)
       11. ✅ helico             > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/drone-sky-watcher/)
       12. ✅ maquette           > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/tank-m3a3-pak40-yugoslav/)
       13. ✅ matprem            > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/planchette-balsa-prestige-7-10/)
       14. ✅ moteur_electrique  > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/quicrun-10-5t-g2-noir-sensored/)
       15. ✅ moteur_thermique   > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/moteur-delta-18s-lisse-tirette/)
       16. 🚀 pcedetthermik      > ✨ exemple
           1. OPTPCETH a virer
           2. COEFFPCETH a virer
       17. piece_heli         > ✨ exemple
       18. piece_voiture      > ✨ exemple
           1. OPTPCECAR
       19. quartz             > ✨ exemple
       20. radio              > ✨ exemple
       21. recepteur          > ✨ exemple
           1. SBUSRECEP a virer
       22. servo              > ✨ exemple
       23. ✅ voitures       > ✅✨ [exemple](https://dev.pb-modelisme.com/produit/fighter-buggy-rx-dt01/)
       24. 🧽 Tous les champs booléens, remplacer "Ne sais pas" par "Non défini"
       25. 🧽 Revoir gestion de l'utilisation du moteur (pour le moment catégorie "Moteurs" avec les véhicules compatibles)
           1. Et deux catégories vides "Moteurs thermiques" et "Moteurs électriques"
           2. Refacto ? sur un champ "compatibilité" ? pour affecter aux autres catégories qui pourraient en avoir besoin
13. ✅👪 RDV client du 12/08/22
    1. ✅ Retours sur le début de front
    2. ✅ Présentation administration champs particuliers
    3. ✅ [Tech] Réponse aux questions
    4. ✅ Repasser sur champs persos doc BDD
    5. ✅🧽 Cleaner compte rendu
    6. ✅ Ajouter nouvelles tâches à la TODO & Maj doc BDD
    7. ✅ 📧 Envoyer compte rendu
14. ✅ Compte rendu de fin de semaine

## 07/08/2022

PB Modelisme

1. ✅📧 Récap semaine envoyé
2. ✅ Analyse BDD > Excel > 1 feuille par table, contenant les champs, les descriptions & les correspondances
   1. ✅ Correspondances avec WC
      1. ✅ accessoires
      2. ✅ acctx
      3. ✅ avion
      4. ✅ bateaux
      5. ✅ batterie
      6. ✅ bougie
      7. ✅ carburant
      8. ✅ chargeur
      9. ✅ controleur
      10. ✅ heliceavion
      11. ✅ helico
      12. ✅ maquette
      13. ✅ matprem
      14. ✅ moteur_electrique
      15. ✅ moteur_thermique
      16. ✅ pcedetthermik
      17. ✅ piece_heli
      18. ✅ piece_voiture
      19. ✅ quartz
      20. ✅ radio
      21. ✅ recepteur
      22. ✅ servo
      23. ✅ voitures
   2. ✅ Inventaire champs personnalisés
      1. cf. `pb-modelisme--com/_docs/craft-and-tests/10-inventaire-champs-personnalisés_secret`
3. ⏳👪 Questions à sylvie & cédric
   1. ✅📧 Mail envoyé
4. 🚀🔍 Vérifier gestion des..
   1. ✅ codes barres (= "EAN") : x2, fournisseur & pb
      1. cf. `pb-modelisme--com/_docs/craft-and-tests/09-codes-barres-barcode-ean`
      2. Ajout de la gestion dans WC via plugin
      3. Impression : Passer par extension payante ou utiliser une librarie et coder un truc maison
      4. ⏳ Politique concernant les x2, voir avec Cédric
   2. ⏳✅ Notations, étoiles de 1 à 5
      1. ✅ Natif, besoin plugin pour import
      2. cf. `pb-modelisme--com/_docs/craft-and-tests/08-import-product-reviews-and-notes`
   3. ⏳ Favoris > Pas utilisé sur le site, 1 seul champ par produit ? wat
   4. ⏳ Eco-taxe
      1. Voir avec Cédric comment c'est géré avant de partir trop loing
      2. Soit stocké en champ particulier, soir [plugin payant 39€](https://solutions.fluenx.com/produit/eco-participation-pour-woocommerce/)
         1. Si plugin payant voir comment importer
   5. ✅ Prix de vente club
      1. [Plugin gratuit bien caché](https://fr.wordpress.org/plugins/elex-woocommerce-role-based-pricing-plugin-basic/)
      2. `cf. pb-modelisme--com/_docs/craft-and-tests/12-prix-club`
      3. 🧠 Pas mal d'autres fonctionnalités proposées, notemment pour la gestion des rôles
5. ✅📝 Ajout des champs supplémentaires WooCommerce requis (avec défauts), non présents en BDD PB, permettra d'uniformiser
   1. ✅ Seulement [SKU & name de requis](https://github.com/woocommerce/woocommerce/wiki/Product-CSV-Import-Schema#csv-columns-and-formatting)
   2. 🌱 Quartz > 🚨💥 Nom a générer
6. 🚀 Repasse sur champs problématiques
   1. ✅ Codes barres (PB & fournisseur)
      1. En attendant retour Cédric, on stocke les deux dans des champs personnalisés
         1. `code_barre_fournisseur`
         2. `code_barre_pbmodelisme`
      2. Champ WC (EAN) prendra celui du fournisseur ?
   2. ✅ Notations 5/5 étoiles
      1. En attendant retour Cédric, on stocke dans un champ legacy `legacy___note_sur_5`
      2. A voir si ça passe en avis clients ?
   3. ✅ Favoris
      1. En attendant retour Cédric, on stocke dans un champ legacy `legacy___favoris`
   4. ✅ Eco taxe
      1. En attendant retour Cédric, on stocke dans un champ personnalisé `taxe_eco_participation`
      2. Sinon reco [plugin payant](https://solutions.fluenx.com/produit/eco-participation-pour-woocommerce/)
   5. ✅ Prix de vente club
      1. 🚨 Voir comment le plugin stocke les infos
      2. De mémoire petite quantité sur une seule table (voiture), ptet faire à la main 👋
         1. ✨🧠💥 Tous les prix clubs ont été retirés de la bdd !?? ~05/08/22
   6. ✅ "AFF" > `legacy___aff`
   7. 🌱👪 Champs spécifiques aux tables > ajoutés aux questions cédric
   8. ✅ Typage des champs
7. 📝 Gestion de l'import des images produits
    1. ✅📌 Voir quand pas d'image, champ à importer peut être vide ?
       1. Oui, seuls les champs SKU & noms sont requis pour l'import en CSV
       2. Voir dans WC il y a un réglage pour fixer l'image par défaut du produit, si il n'en a pas
    2. ⏳ Récupération des fichiers images, afin de les balancer sur le nouveau serveur

## 29/07/22

PB Modelisme

1. 🚀 Analyse BDD > Excel > 1 feuille par table, contenant les champs, les descriptions & les correspondances
   1. ✅ Inventaire global des champs
      1. ✅ Sur l'ensemble des tables
         1. ✅ Compter 🧮 le nombre d'entrées dans chaque table
         2. ✅ Compter 📊 le nombre d'entrées affichées sur le site
         3. ✅ Inventaire des champs en BDD 💾
         4. ✅ Description des champs en BDD 💬
         5. ✅ Inventaire caractéristiques techniques 🔧
         6. ✅ Inventaire tout ce qui est affiché 👀
         7. ✅ Discriminer les champs
            1. 👤 vides
            2. 🤏 Faible quantité de données fabriqués à partir d'autres tables
            3. ♻️ à refactoriser
            4. 🔗 fabriqués à partir d'autres tables
            5. 👪 communs
            6. 🏎️ communs à tous les véhicules
            7. 🙍‍♂️ propre à cette table
            8. ❓ Infos non retrouvées en BDD
         8. ✅ Lister tables liées 🔗
      2. ✅ Avancement par table
         1. ✅ accessoires
         2. ✅ acctx
         3. ✅ avion ❓ Produits compatibles, Lien avec moteurs thermiques
         4. ✅ bateaux
         5. ✅ batterie ❓ Produits compatibles
         6. ✅ bougie
         7. ✅ carburant
         8. ✅ chargeur ❓ Produits compatibles
         9. ✅ controleur ❓ Produits compatibles
         10. ✅ heliceavion ❓ Piéces détachées, Accessoires conseillés
         11. ✅ helico ❓ Onglets
         12. ✅ maquette ❓ Onglets
         13. ✅ matprem ❓ Onglets
         14. ✅ moteur_electrique ❓ Onglets
         15. ✅ moteur_thermique ❓ Onglets
         16. ~✅🧮📊💾👤🤏💬 pcedetthermik ❓ Pas d'affichage sur le site
         17. ✅ piece_heli
         18. ~✅🧮📊💾👤🤏💬 piece_voiture ❓ Pas d'affichage sur le site
         19. ~✅🧮📊💾👤🤏💬 quartz ❓ Pas d'affichage sur le site
         20. ✅ radio ❓ Onglets récepteurs compatibles
         21. ✅ recepteur ❓ Onglets produits compatibles
         22. ✅ servo ❓ Onglets
         23. ✅ voitures ❓ Onglets

Perso

1. ✅ Commander bière
   1. ✅ Commande
   2. ✅ Attente livraison
2. ✅ Remplir sondage sofia
3. ✅ Film the perfection
4. ✅ Eclater mauvaise herbe pot jardin
5. ✅ Réparer putain de sacoche
   1. ✅ & pins
6. ✅ Organisation week-end warhammer
7. ✅ Syndic
   1. ✅ Attente 27/07
   2. ✅ Payer moitié
   3. ✅ Virement
8. ✅ Loyer
   1. ✅ Attente 27/07

## 22/07/22

Perso

1. ✅ Cadeau anniv Ju

Auto entrepreneur

1. ✅ Facture 4/4 PB Modélisme
   1. ✅ Edition & envoi
   2. ✅ Règlement
   3. ✅ Mail de confirmation

PB Modelisme

1. 🚀 Analyse BDD > Excel > 1 feuille par table, contenant les champs, les descriptions & les correpsondances
   1. ✅ Analyse des champs utiles
      1. ✅ Référencer tous les champs ayant intégralement pour valeurs "NULL"

## 15/07/22

Perso

1. ✅ Boursorama > pougnoutte
2. ✅💩 Check commande auto anaca3
3. ✅💩 HF > Remboursement cashless
   1. 💩💩💩 Jusqu'au 10 juillet, donc volé lolilol
4. ✅ Chatte
   1. ✅ Carnet santé en ligne
   2. ✅ Collier gravé n° de téléphone
   3. ✅ Vérification ICAD
   4. ✅ Vérification Petlink.fr > pas de médaille
5. ✅ [Skald](https://mail.google.com/mail/u/0/#inbox/FMfcgzGllVqqnCLcTDzRlDQTwnhlHFdM). A donner a mes parents
6. ✅ Prog août
    1. Margot & Ryan
    2. Marc
    3. Quentin
    4. Mehmet
    5. Baydot fof
    6. week-end warhammer
7. ✅ Résilier ESET (besoin de contacter le support ?)
   1. ✅ Pas de renouvellement auto
8. ✅ Changer pass steam

Taf

PB Modelisme

1. ✅ RDV Nonore
   1. ✅ Go
   2. ✅ CRR + drive
   3. ✅ Mail
2. ✅ Gérer retours du rendez-vous > ✅ Site local & ✅ dev.pb-modelisme.com
   1. ✅✅ Ajouter le thème Divi + clé payante max
   2. ✅✅ Ajouter une dizaine de produits PB (avions) avec photos afin de donner accès aux pages profondes, panier, etc.
      1. ✅🐛 dev > il manquait des fichiers dans `/wp-includes/` ?
   3. ✅📌 Vérifier si besoin de retoucher aux pages préconstruite par woocommerce
      1. ✅ Probalement besoin de réassigner des templates à certaines pages (mon compte, boutique)
   4. ✅ Modifier les couleurs de base du site afin de mieux représenter le site PB
      1. ✅ Ajout du rouge en couleur principale du thème
   5. ✅ Ajouter le logo PB dans le menu
   6. ✅ Création de pages de démonstration de possibilité afin de donner du choix côté PB
      1. ✅ Hardware Store > 6 pages
      2. ✅ Bike Repair Services > 7 pages
   7. 🌱 Créer une page pour démo des modules
      1. ✅ Ajouter les modules, un par bloc, séparés
      2. ✅ Quelques exemples de blocs réseaux sociaux
      3. 🌱 Terminer A télécharger & installer
   8. ✅ Création du menu, avec le lien fonctionnel vers les avions ainsi que les pages de démo
   9. ✅ Personnaliser un poil plus les propositions de templates
   10. ✅ Importer uploads/ & bdd sur dev
   11. ✅ Vérifications menus
   12. ✅ Mail nonore & clients
   13. ✅ Retour nonore
       1. ✅ Passer le menu en rouge
       2. ✅ Page d'accueil plus customisée, basée sur template Hardware store
          1. ✅ Slider
          2. ✅ Nouveautés
3. ✅ Revoir versionning
   1. ✅ Stocker archives WP WC DIVI + stocker notre wp-content/
   2. ✅📝 Notes installation
4. ✅ Excel BDD > 1 feuille par table, contenant les champs, les descriptions & les correpsondances
   1. ✅ Récupérer les champs des tables contenant des produits
5. ✅📝 Gestion de l'import des images produits
   1. ✅💥 Passer doc en secret
   2. ✅ Ancien site
      1. ✅ Où sont elles stockées ? Attention aux catégories
      2. ✅ Création de l'url ?
      3. ✅ Stockage en base de données
      4. ✅ Gestion des images multiples
         1. ✅🚨 Soit ref table photo*, soit champ dédié ~MEDIA !
         2. 🌱🚨 voiture > possibilité de galeries supplémentaires, gérées ?
      5. ✅📝 Documentation pour CHACUNE des tables
   3. ✅ Nouveau site
      1. ✅ Vérifier comment sont importés les photos produits dans les exemples
         1. 🚀📌 Voir quand pas d'image, champ à importer peut être vide ?
      2. ✅ Méthode d'import
         1. ✅ Récupérer champs, tables & crafts d'urls

Champagne Didier Lapie

1. ✅🐛 Bug disparation de ma commande dans l'administration WordPress
   1. Rien dans la base de donnée, ni dans les backups avoisinants la date de la commande (4/07/22)
   2. Les commandes sont [gérées comme des posts WP](https://wordpress.org/support/topic/one-of-my-oder-is-missing-from-woocommerce-orders-tab/)
   3. L'adresse de ma commande renvoit vers une [nouvelle page par défaut de mentions légales](https://champagne-didier-lapie.com/wp-admin/post.php?post=1147&action=edit)
      1. Erreur humaine
      2. Bug exceptionnel
         1. Suite à la maj de WooCommerce ?
         2. Lié au fait que j'ai un compte admin ?
      3. Bug OVH/WC ?
   4. A suivre, les Lapie me renvoient un mail si une commande apparaît en mail mais pas dans l'admin
      1. Besoin de plus d'infos

Arrêter dev serveur & hebergement

1. ✅💡 Revoir sauvegardes sites
   1. Projet github de base en ligne
      1. Cloner
      2. Fichiers de base projet github + edit REAMDE.md adresse site
   2. Arbo
      1. _sauvegarde site avant mise a jour
         1. base de données **.zip**
         2. fichiers **.zip**
      2. nouveau site mis a jour
         1. base de données
            1. Export sql "date---XXX.sql.zip"
            2. Export all in one wp migration "220713---export-bdd-seulement-via-all-in-one-wp-migration_XXX"
         2. fichiers
            1. base wordpress 6.0 a laquelle appliquer le contenu de www **.zip**
            2. www/
               1. wp-content/ **.zip / SSI > 50mo .gitignore**
               2. wp-config.php
               3. README.md
   3. Adapter .gitignore
   4. Githubber & push
   5. Sauvegarde BDD OVH
   6. Sauvegarde site sur disque dur externe
      1. Faire un zip du dossier "date---XXX"
2. ✅ Faire [doc introduction management OVH](https://github.com/youpiwaza/prise-en-main-ovh)
3. ⏳ com--aldinfographie
   1. ✅ Console & clean éventuel
   2. ✅ Sauvegarde BDD
   3. ✅ Procédure sauvegarde site
   4. ✅📌 Tests & validation
   5. ✅ Mail infos
      1. ✅ Rassurer
      2. ✅ Prévenir mails qui vont arriver
         1. ✅ OVH
            1. ✅ Changement à faire infos proprio
         2. ✅ Récupérer sauvegarde via wetransfer
         3. ✅ Pièce jointe Identifiants clients en PDF
      3. ✅ lien vers doc ovh
      4. ✅ email administrateur wordpress
   6. ✅ Envoyer identifiants site au format pdf
   7. ✅ Envoyer sauvegarde au client via WeTransfer
   8. ✅ Changer email administrateur wordpress
   9. ✅ Passations NDDs
   10. ⏳ Passation hébergement
       1. SMS
       2. ⏳ Attente identifiant OVH
4. ⏳ com--champagne-didier-lapie
   1. ✅📌Tests & validation
      1. ✅⏳ Validation trop longue
   2. ✅ Procédure sauvegarde site
   3. ✅ Mail infos
   4. ✅ Envoyer identifiants site au format pdf
   5. ✅ Envoyer sauvegarde au client via WeTransfer
   6. ✅ Changer email administrateur wordpress
   7. ✅ Passations NDDs
   8. ⏳ Passation hébergement
       1. SMS
       2. ⏳ Attente identifiant OVH
5. ✅ com--maximelecuyer
   1. ✅📌Tests & validation
   2. ✅ Procédure sauvegarde site
   3. ✅ Mail infos
   4. ✅ Envoyer identifiants site au format pdf
   5. ✅ Envoyer sauvegarde au client via WeTransfer
   6. ✅ Changer email administrateur wordpress
   7. ✅ Passations NDDs
   8. ✅ Passation hébergement
6. ⏳ com--sophieberberian
   1. ✅📌 Tests & validation
      1. ✅⏳ Validation trop longue
   2. ✅ Procédure sauvegarde site
   3. ✅ Mail infos
   4. ✅ Envoyer identifiants site au format pdf
   5. ✅ Envoyer sauvegarde au client via WeTransfer
   6. ✅ Changer email administrateur wordpress
   7. ✨ Passations NDDs
   8. ⏳ Passation hébergement
       1. SMS
       2. ⏳ Attente identifiant OVH
7. ✅ Résilier nouveau serveur
   1. ⏳ Effectif 1er aout
8. Autre
   1. com--champagne-pascal-picard
      1. ✅ Procédure sauvegarde site
      2. ✅ Mail infos
      3. ✅ Envoyer identifiants site au format pdf
      4. ✅ Envoyer sauvegarde au client via WeTransfer
      5. ✅ Changer email administrateur wordpress
      6. ✅ Passations NDDs
         1. ✅ .com
         2. ✅ .fr
         3. ✅ Envoyés à Geoffrey
      7. ⏳ Passation hébergement
         1. SMS
         2. ⏳ Attente identifiant OVH
   2. ✅ MKasza
      1. ✅ Passations NDDs
9. ✅ Virer les sites de _dev/_current

## 08/07/22

PB Modelisme

1. 🌱⏳ Améliorations WP classiques
   1. ⏳🔒️ Attente https
   2. Vérifier Erreurs console ? Ressources dans wp-include/ en 404 > Besoin https
   3. WP admin > Santé du site
2. ✅ local > dev > Dupliquer la BDD grâce à modification de l'adresse dans wp-config ?? yay
   1. [doc offi](https://fr.wordpress.org/support/article/running-a-development-copy-of-wordpress/#modifier-ladresse-du-site)
   2. Nah, utilisation de all in one wp migration
3. ✅ Monitorer ancien serveur PB
    1. ✅ Attente confirmation Cédric > Attente lundi (en cas de pépin serveur)
    2. 💩 Création d'un accès SSH
       1. KO, connexion SSH désactivée, malgré création de clé :/
    3. 💩 Installation de htop
       1. Utilisateur pas dans les sudoers > Pas d'installation de paquets
       2. Utilisation de `top`, équivalent de `htop`
4. ✅ Structure de données > Catégories
    1. ✅ Inventaire des tables dans la BDD PB Modelisme actuel
    2. 🌱 Liste champs communs entre WC & PB (but discriminer perso)
       1. ✅ Cedric : Confirmer quelles sont les tables contenant les produits
    3. ✅ Lister catégories
       1. ✅ Ex: types/niveau/marques/etc.
       2. ✅ But : différencier catégories des champs personnalisés (choix via select)
       3. ✅ Créer sous WordPress afin de dégrossier
          1. 📝 On en aura besoin pour les imports de toutes manières
          2. ✅ Catégories générales
          3. ✅ Catégories produits
          4. ✅ Sous catégories accessoires
          5. ✅ Sous catégories matériaux
          6. ✅ Type avion
          7. ✅ Type Batterie
          8. ✅ Catégories bateau
          9. ✅ Type bateau
          10. 🌱 Type quartz > Catégorie de base ? Accessoires > Récepteur ?
              1. A migrer dans le nom du produit Quartz
          11. ✅ Type voiture
          12. ✅ Type moteur > Faire une catégorie dédiée aux moteurs ? Ou sous catégorie ? Ou champ dédié
          13. 🌱 Utilisation bateaux > Utilisé ? Rien sur quelques bateaux au pif
              1. batteries > A migrer dans la description du produit Batterie
          14. ✅ Utilisation controlleurs > Faire une catégorie dédiée aux controlleurs ? Ou sous catégorie ? Ou champ dédié
              1. ✅ Accessoires > Controleurs > (Type)
          15. ✅ vers boite > Faire une catégorie dédiée aux kits avions ? Ou sous catégorie ? Ou champ dédié
              1. ✅ Catégorie globale
          16. ✅ Niveaux avions
          17. ✅ Niveau drones & hélicos
          18. ✅ Type voiture
          19. ✅ Catégories maquettes
5. ✅ RDV client tech du Mercredi 06/07/22
   1. ✅ Préparer RDV client
   2. ✅ RDV Client
   3. ✅ Compte rendu
   4. 💩 Max: Envoyer à Cédric les images (gofullpage) des structures de chaque table
      1. ✅ Excel 1 feuille par table
   5. ✅ Passer catégories sur le dev
      1. ✅🐛 Dev > Changer adresse site `dev-pb-modelisme.masamune.fr` > `dev.pb-modelisme.com`
         1. ✅ Réinstallation BDD Wordpress
      2. ✅ Local & dev > Installer plugin all in one wp migration
      3. ✅ Local > Export
      4. ✅ Dev > Import
   6. ✅ Catégories
      1. ✅ Revoir TODO suite au RDV
      2. ✅ Ajouter les nouvelles catégories
      3. ✅ Passer en dev
      4. ✅ Envoyer mail a Cédric pour vérification des catégories
6. ✅ Excel BDD > 1 feuille par table, contenant les champs, les descriptions & les correpsondances
   1. ✅ Récupérer les champs des tables contenant des produits

Arrêter dev serveur & hebergement > Week end SEULEMENT

1. Migrer clients
   1. Ancien serveur
      1. ✅ masamune
         1. ✅ stockage
         2. masamune--fr
            1. ✅ Repartir d'une base propre WP et récupérer/convertir les trucs 1 par 1
            2. Refonte complète du site
               1. 🚀 Virer woocommerce & cleaner bdd
               2. ✅ CGV
                  1. ✅ Clause 5
                  2. ✅ Maj les BP de devis
               3. ✅ Page crédits
      2. ✅ MLecuyer
         1. ✅ Fixer une date pour faire la bascule (besoin accès SMS)
         2. ✅💩 Faire évoluer hébergement déjà pris par ML
            1. ✅ Nouvelle commande -_-
            2. ✅ Résilier l'ancien hébergement après
         3. ✅ Identifiants dans secrets
            1. ✅ Mise à jour ftp
            2. ✅ Mise à jour Base de données
            3. ✅ Mise à jour WordPress
         4. Ancien site > Installation all in one wp migration si possible
            1. ✅ Installation
            2. ✅ Export
         5. ✅ Uploader base wordpress
         6. ✅ Mise à jour wp-config
         7. ✅ Réinstallation wp
         8. ✅ Mise à jour identifiants
         9. ✅ Injecter anciens fichiers
            1. ✅💩 Résoudre bugs
               1. 💩 `plugins/leaflet-maps-marker` > maj > KO
               2. ✅ Virer tous les plugins
         10. ✅ Injecter bdd via all in one wp migration
         11. ✅ Repasser WordPress en FR
         12. ✅ Maj permaliens
         13. ✅ Mises à jour
         14. ✅💩 Résoudre bugs
             1. ✅ Restauration des plugins un par un
                1. ✅ advanced-custom-fields
                   1. ✅ Mise à jour
                2. ✅ acf-gallery
                3. ✅ acf-options-page
                4. ✅ acf-repeater
                5. ✅ Akismet Spam Protection
                   1. ✅ Mise à jour
                6. ✅ leaflet-maps-marker
                   1. ✅ Mise à jour
                7. ✅ ninja-page-categories-and-tags
                   1. ✅ Mise à jour
                8. ✅ wp-edit
                   1. ✅ Mise à jour
                9. 💩 wp-security-scan
                   1. Obsolète 6 ans + > Supprimer
         15. ✅ Theme de base > Mise à jour
         16. ✅💩 ACF > des données ont sautées
             1. ✅ Récupérer configuration ACF
             2. 💩 Ancien exporte en XML, version MAJ en JSON -_-
             3. 💩 Ancien site > mise à jour puis export > Mise à jour KO
             4. ✅ Nouveau site > ancienne version pour import
                1. 💩 PUIS Mise à jour
                2. ✅ On garde l'ancienne version du plugin
         17. ✅ OVH Manager > Sauvegarde BDD
         18. ✅📌 Tests & validation
             1. ✅ Mail ML
             2. ✅ Attente confirmation
             3. ✅🐛 Fix ancien bug "projets > placement sur grille"
         19. ✅ Wp admin > Changer adresse site
             1. ✅ Revoir url site en bdd
         20. ✅ Ovh manager > Multisite
         21. ✅ Basculer DNS
         22. ✅ Vérifier site
         23. ✅ Remettre adresse administrateur WP `admin_ml` > `maximelecuyer@hotmail.com`
         24. ✅ Remettre HTTPS
             1. ✅⏳ Attente propagation DNS
         25. ✅ Résilier l'ancien hébergement
         26. ✅ OVH Manager > Sauvegarde BDD
         27. ✅ Sauvegarde site sur disque dur externe
         28. ✅ Envoyer sauvegarde au client via WeTransfer
         29. ✅ Mail client confirmation & identifiants
   2. Nouveau serveur
      1. ⏳ ALD infographie
         1. ✅ Basculer DNS
         2. ✅ Vérifier wp-config.php
         3. ✅ Vérifier site
            1. ✅ Console
         4. ✅ Remettre HTTPS
            1. ✅⏳ Attente propagation
            2. 🚀 Console & clean éventuel
               1. ✅ Images manque https
                  1. En dur dans le theme -_- > modifié header.php & style.css
               2. ✅ 404 pour un [plugin > bootstrap](https://aldinfographie.fr/wp-content/plugins/portfolio-filter-gallery/js/bootstrap.min.js.map:)
               3. 💩? Problème flux instagram
               4. 💩 Problèmes affichage
               5. ✅ Mail nonore voir si elle peut rattraper le truc
                  1. ✅ Si ok good
      2. ✅ Champagne didier lapie
         1. ✅ Basculer DNS
         2. ✅ Re-balancer bdd (nouvelles commandes)
         3. ✅ Remettre HTTPS
         4. ✅✅ Réactiver paiement, crédit agricole
            1. ✅ Test paiement, attente propagation https
         5. ✅ Sauvegarde BDD
         6. ✅ Sauvegarde site sur disque dur externe
         7. 📌⏳ Tests & validation
             1. ✅ Mail
             2. ⏳ Attente confirmation
         8. ✅ Voir pour changer adresse site en bdd (+ maj wp-config)
      3. ⏳ Sophie berberian
         1. ✅ Relance clients : bascule auto si pas de news
         2. ✅ BAYDOT
            1. ✅ Basculer DNS
            2. ✅ Rajouter lignes DNS TXT afin de confirmer la propriété
         3. ✅ Renvoyer sauvegardes sites a baydot
         4. ✅ OVH Manager > Multisite > Modifier domaine > dossier racine `www`
         5. ✅ Vérifier wp-config.php
         6. ✅💩 Résolution erreur 500
            1. ✅ Ajout debug php
            2. ✅ Correction url en BDD
         7. ✅ Remettre HTTPS / En cours propa
            1. ✅ Corriger HTTPS en bdd sur certaines ressources
            2. ✅ Maj Sauvegarde DD
            3. ✅ Maj sauvegarde OVH Manager
         8. ✅ Sauvegarde BDD
         9. ✅ Sauvegarde site sur disque dur externe
         10. ✅ Envoyer sauvegarde au client via WeTransfer
         11. 📌 Tests & validation
             1. ✅ Mail
             2. ⏳ Attente confirmation

Auto entrepreneur

1. ✅ NDD > ALD
   1. ✅ Facture NDD
   2. ✅ Relance le 04/07/22
   3. ✅ Paiement

Perso

1. ✅ Changer pass mcdo
2. ✅ Créer compte site permis conduire
3. Chatte
   1. ✅ Changer filtre caisse
      1. ✅ Filtres livré jeudi 07/07
      2. ✅ Changés
4. ✅ Renouveler permis de conduire
   1. ✅ En attente de retour ~15/07/22
5. 💩 Boursorama > appeler pour compte pougnoutte + rachat crédit immo
   1. Mail envoyé, en attente de réponse
   2. Pas de négo, taux a 2,20

## 01/07/22

Taf

PB Modelisme

1. ✅ Hebergement > host `www/` > Rajouter un .htaccess deny all
2. ✅ Passage DNS de masa vers dev.pb
   1. ✅ Virer sous domaine masamune
   2. ✅ Virer pb > multisite > masa
3. ✅ Analyse de la structure de BDD WP + WooCommerce
   1. 💩 Faire des diffs
      1. ✅ Ajout d'un produit
      2. ✅ Ajout d'une [catégorie](https://fr.wordpress.org/support/article/taxonomies/)
      3. ✅ Ajout d'une sous catégorie
      4. 💩 Pas mal de trucs à côté de modifier, **besoin** de passer par import régulier, pas de sql à l'arrache
         1. 🔍 Plugin classique (+ manip dev pour champs persos) ou plugin payant
4. ✅🧠💥 Remise au propre des objectifs à court terme
5. ✅📌 Tests d'imports [plugin officiel](https://woocommerce.com/document/product-csv-importer-exporter/)
   1. ✅ Tester l'export de produits
   2. ✅ Tester l'import de produits
   3. ✅ Tester la mise à jour de produits
   4. ✅ Tester l'import avec colonnes custom [plugin officiel > github](https://github.com/woocommerce/woocommerce/wiki/Product-CSV-Importer-&-Exporter#adding-custom-import-columns-developers)
6. ✅📌 ACF
   1. ✅🔍 Voir ou ça en est
   2. ✅ Tester champs custom avec catégorie & sous catégories
   3. ✅ Export
   4. ✅ Import
   5. ✅ Mise à jour
7. 🔒️✅ Tester accès FTP/SSH/BDD ancien serveur
   1. 💩✅ KO, vu avec Cédric pour les nouveaux accès
   2. 📝✅ Maj des de "Ressources" & sacrets
8. ✅📌 Test export CSV avions ancien serveurs limit 50
    1. ✅ A envoyer vers sacrets quand terminé
9. 🚀 Structure de données
    1. ✅ Rassembler l'ensemble dans [un seul doc](https://docs.google.com/spreadsheets/d/1FB8e-0I9RhqWixoqdaXPjEZmjBATmI7j0GCd7tOVjrE/edit#gid=1110417694)
    2. ✅ Récupérer les caractéristiques d'un import WC (doc) + aidera à limiter les champs personnalisés

Serveurs > Migrer clients

1. Ancien serveur
   1. ✅ stockage
      1. ✅ Trier
      2. ✅ Uploader
      3. ✅ Vérifier
      4. ✅ Protéger accès racine

Perso

1. ✅ Création de "mon espace santé"
2. ✅ Faire virement remboursement emprunt juillet
3. ✅ Camping / Vacances
   1. ✅ Relance pour chèque de caution & 2eme bestiau
   2. ✅ Envoi carnets de santé bestiaux x2
4. ✅ Envoyer mail syndic pour pour pardon avoir zappé AS
5. ✅ Chatte disparue > passer à la boulangerie enlever l'avis de recherche

## 17/06/22

Perso

1. ⏳ Renouveler permis de conduire
   1. ✅ Démarche en ligne
   2. ✅ Lettre avec photo identité envoyée
2. ✅ [Changement propriétaire chatte](https://mail.google.com/mail/u/0/#inbox/FMfcgzGllCcNJCZHqcjqlkNJhlNFzwZC)

Taf

Cryptor > Clôture

1. ✅ Doc de fin de contrat a signer + signature electronique
   1. 💩 Signature
2. ✅ Facture
   1. ✅ Règlement

## 10/06/22

Taf

PB Modelisme

1. ✅ Facture juin
2. 🚀 Passage DNS de masa vers dev.pb
   1. ✅ Attente mise en place TXT & tests

Arrêter dev serveur & hebergement

1. Migrer clients
   1. ✅ Champagne didier lapie
      1. ✅ Commander hébergement Perf
      2. ✅ Maj tout dans ovh manager  
      3. ✅ Uploader base wordpress DE LA MEME VERSION QUE CELLE EN LIGNE
      4. ✅ Recup wp-config
      5. ✅ Réinstallation wp
         1. ✅ Test avec php 7.4 ????
            1. ✅💩 Un seul plugin qui bloque > Viré > Ok 8.1
      6. ✅ Maj identifiants
      7. ✅ Injecter anciens fichiers
      8. ✅ Injecter ancienne bdd via all in one wp migration
      9. ✅📌 Tests
      10. ✅ Maj permaliens
      11. ✅ Sauvegarder fichiers dans dossier `_backups`
      12. ✅ Mises à jour VIA ADMIN WP
      13. ✅ Remettre php 8.0 ou 8.1
      14. ✅ Re-sauvegardes
   2. 🚀 masamune
      1. 💩 masamune--fr
         1. ✅ Uploader base wordpress
         2. ✅ Recup wp-config
         3. ✅ Réinstallation wp
         4. ✅ Maj identifiants
         5. ✅ Virer tous les commentaires (indésirables)
         6. ✅ Injecter ancienne bdd
         7. ✅ Injecter Ancien fichiers
         8. 💩 KO > Theme & Plugins
            1. ✅ Virer tous les plugins & themes
            2. ✅ Virer toutes les tables alakon en bdd
         9. ✅ Maj permaliens
         10. ✅ Mises à jour
         11. 💩 Trop de merde
2. Ranger merdier dans /dev/current
   1. Sur disque dur externe
      1. ✅ ALD infographie
      2. ✅ Baptiste guereschi
      3. ✅ Champagne didier lapie
      4. ✅ Margot Kasza
      5. ✅ Sophie berberian

Perso

1. ✅ Préparer lettre icad + mail
2. ✅ Envoyer chèques vacances par courrier
3. ✅ app Hellfest + cashless
4. ✅ Rappeler vincent bbq
5. ✅ Prévenir darons pour Seth
6. ✅ Tel > contact Nick christophe's pal > Ajout contact photographe (concert/ethnique)
7. ✅ Chatte > annuler recherches & affiches
8. ✅ concert 10/06 maximum the hormone
   1. ✅ trains, et utiliser [reductions](https://mail.google.com/mail/u/0/#inbox/KtbxLxgZZVNcfFNSbtrStGMpWXmfCKPsJB)
9. Films
   1. Ciné
      1. ✅ Dernier Cronenberg
10. ✅ Badge salon open source
11. ✅ Renouveler carte fnac
12. ✅ Imprimer billets HF 1

## 03/06/22

Taf

PB Modelisme

1. ✅ Environnement de dev local
   1. ✅ Crafts n' tests > `pb-modelisme--com/_docs/craft-and-tests/01-craft-docker-compose-file/README.md`
   2. ✅ Création du dossier local & maj de la doc `_docs/local-environnement-setup.md`
      1. ✅🚨 Structure du projet pour insertion sur serveur > `wp-content/` à la racine du projet ?
   3. ✅ Installation persistante > Une fois l'installation de WordPRess terminée via wp-cli
      1. ✅ Populer github avec les fichiers `/wordpress`
      2. ✅ Local > pull
      3. ✅ OVH manager > Sauvegarde BDD
      4. ✅ Populer BDD locale > Installation
      5. ✅ Récupérer identifiants WP de OVH & populer secrets en local
   4. ✅ Ajout de wp-cli
      1. 💩 KO en `docker run`
      2. ✅🔨📌 Ajout au docker-compose
         1. ✅ Test au lancement
         2. ✅ Test des commandes basiques
      3. ✅👌 Mise au propre
         1. ✅ Local DC
            1. ✅ 🐛 Ajuster l'utilisateur
         2. ✅📝 Doc & principales commandes
   5. ✅🐛 Problème lors des mises à jour via admin wordpress (traductions, plugins, etc.)
      1. ✅ wp-config > passer outre les identifiants sftp
      2. ✅ Se connecter au conteneur wp en tant que root & `chown -R www-data:www-data wp-content/`
      3. ✅ FIX & Doc
2. ✅💻 Serveur OVH
   1. ✅ Commandé & livré
   2. ✅🔑 Récupérer les identifiants de base
   3. ✅🔒️ Modifier tous les identifiants de base qui sont quand même vraiment pas sécurisés
   4. ✅🙊 Maj secrets
   5. 💩🐛 Passer en multisite pour site de dev & WordPress 1 clic
      1. KO version de php ou nom d'admin trop long chp + DNS foireux
   6. ✅🔍 [Doc wp-cli](https://wp-cli.org/fr/)
   7. ✅ Installation de [wp-cli](https://make.wordpress.org/cli/handbook/guides/installing/)
   8. ✅ Installation de WordPress [via wp-cli](https://make.wordpress.org/cli/handbook/how-to-install/)
      1. ✅ Site de dev dispo sur [sous domaine masa](https://dev-pb-modelisme.masamune.fr/)
3. ✅⚡️👷 Flux de développement via git afin d'éviter les conflits
4. ⏳ Améliorations WP classiques
   1. ✅ Permaliens
   2. ✅ Virer les plugins inutiles
   3. ✅ Virer les thèmes inutiles
   4. ✅ Mises à jour
   5. ✅ SALT
   6. ✅ Virer `wp-config-sample.php`
5. 🚀 Passage DNS de masa vers dev.pb
   1. ✅ OVH Manager > multi-site > Prise en charge du NDD
   2. ✅ Call avec Cédric pour mise en place (entrée supl. vérif possession DNS > TXT)
6. Analyse de la structure de BDD WP + WooCommerce
   1. 🤏✅ MCD WordPress Vanilla
   2. ✅ Installation de woocommerce
   3. 🤏✅ MCD WP WC
   4. ✅ Plutôt comparaison exports SQL pour gain de temps

AE / Flinguer hebergement

1. ⏳ Baptiste guerechi > envoi archive sauvegarde
   1. Attente confirmation réception
2. masamune
   1. ✅📂💾 recup blog
   2. ✅📂 stockage
3. ⏳ mkasza > envoi archive sauvegarde
   1. Attente confirmation remise en place

## 27/05/22

Taf

PB Modelisme

1. ✅ Repo projet de base
   1. ✅ Fichiers de config
   2. ✅ READMEs
2. ✅ Repo de base
3. ✅💻 Commander hébergement

Arrêter dev serveur & hebergement

1. ✅ Envoyer mail clients
2. ✅ Virer `C:\Users\masam\Documents\_dev\nouveau serveur anciens backups`
3. ✅ Cleaner repo sacrets
4. ✅🔥 Ancien serveur
   1. ✅🔥 Lapie
   2. ✅🔥 emorizet
   3. ✅🔥 framboise
   4. ✅🔥 hadrien belkebir
   5. masamune
      1. ✅🔥 le reste
   6. ✅🔥 ppicard
   7. ✅🔥 rlafitte
   8. ✅🔥 sophie berberian
   9. ✅🔥 scripts
   10. ✅🔥 vmail
   11. ✅🔥 youpiwaza

Clôture cryptor

1. ✅ Boilerplate rupture de contrat

## 20/05/22

Taf

1. ✅ Mail à PB Modelisme

Serveur > Reprendre en main le projet

1. ✅ Relire les rôles 10 & 20
   1. `ansible-install-web-server\ansible\100---hello--masamune--fr----README--generated.md` > confusion entre nginx et wp > a cleaner (variable techno utilisée ou chp)
2. ✅ Reprendre en main les playbooks
   1. ✅📌 Test forge nginx > faire tourner l'exemple
   2. ✅📌 Test forge wordpress > faire tourner l'exemple
3. ✅🧽 Faire une grosse repasse sur les index de projet il manque plein de vars
   1. Note max du turfu : inspecter les fichiers générés (.md & .yml) & vérifier les variables, interprétées ou non
   2. BUG: génération des fichiers de sites > prefixe `200-` pas utilisé partout
4. 💩 Virer les projets générés à la racine, et rajouter dans `generated/~README` un `cd` vers le dossier généré
   1. Pas sûr que cela soit possible de lancer depuis un autre dossier, avec les fichiers en référence (hosts & /roles)
5. ✅📌 Vérifier (re)mise en place test-wordpress.masamune.fr

Serveur > Cleaner/Debug

📝👴 *Anciennes notes : Récupérer, vérifier, ranger, nettoyer*

1. ✅ Récupération des playbooks actuellement utilisés & vérifications avant
   1. ✅ cf. `ansible-install-web-server\commandes-backup-volumes-a-la-maing_secret.md`
   2. ✅💾🔥 cf. `ansible-install-web-server\ansible\tmp\_old`
   3. ✅🔥 cf. `ansible-install-web-server\ansible\roles\stack-web-nginx--generate-playbooks\vars\clients\lapie\champagne-didier-lapie--com\`
      1. Duplicata de idem-wordpress, qui n'a rien à faire la > suprression
   4. ✅ `ansible-install-web-server\ansible\roles\stack-web-wordpress--generate-playbooks\vars\clients`
2. ✅ Nettoyer (sous)dossiers/fichiers
   1. ✅🔥 /tmp/old, etc.
   2. ✅🧽 secrets > projets github à la racine, à c/c dans les projets locaux
      1. Dedup/virer `/clients` qui est redondant
3. ✅ Mettre à jour les fichiers générés pour WordPress
   1. 👷✅ Lapie > attention le .yml a été édité a la main cf. `C:\Users\masam\Documents\_dev\Backups serveurs\lapie old access and yml`
      1. ✅ Plus de ressources (cpu & ram)
      2. ✅ Gestion automatique du https
      3. ✅ Faire le diff avec les fichiers générés & mettre à jour, le serveur supporte bien la charge de toutes manières
      4. ✅📌 Tester nouvelle stack
   2. ✅ Faire le diff avec le site de nonore également
   3. ✅ Génération > WordPress > Pas de répliques (ni wp, ni mariadb)
   4. ✅ Mettre à jour les images wp & maria
4. ✅🚥 Traefik
   1. ✅🧽 Gestion automatique de la redirection http vers https
   2. ✅⬆️ [Maj image traefik](https://doc.traefik.io/traefik/migration/v2/#v248-to-v249)
   3. ✅🚀⚡️ enable http3 AFTER maj image
   4. ✅🐛 Gestion automatique des certificats https
   5. ✅📌 Checker diff logs
   6. ✅ Re-activate HTTPS production url `ansible/roles/core-reverse-proxy-traefik--generate/templates/traefik.yml.j2`
5. ✅🐛💥 Conteneur ne démarre pas, parfois
   1. ✅📌💡 Le conteneur wordpress ne démarrait pas, mais se lance dès qu'un autre est coupé
      1. ✅📌💡 Si on tente de relancer l'autre, il ne redémarre pas tant qu'une place n'est pas dispo
   2. ✅🔍Checker les logs avant de partir n'importe ou `C:\Users\masam\Desktop\220518-logs-trop de conteneurs en même temps.ini`
      1. 💩 [network ?](https://github.com/docker/compose/issues/6405#issuecomment-445345584)
   3. ✅🔍 Nombre max de stack/conteneurs que l'on peut lancer en simultané ? [SO](https://stackoverflow.com/a/37628520)
      1. ✅ A priori ~1k, sinon ressources
   4. [🔍 Runtime options with Memory, CPUs, and GPUs](https://docs.docker.com/config/containers/resource_constraints/)
      1. ✅🧠 A priori le problème provient des réservations : le serveur à 8 processeurs,
            avec les sites en places ~6.5 de réservés, dernier wordpress forcé a minimum 2 procs >> ne se lance pas
   5. ✅ Revoir politique de ressources sur les conteneurs
      1. ✅🔍 [Requis pour WP](https://wordpress.org/about/requirements/)
      2. ✅📌 Appliquer
6. ✅🔧 Activation de la mémoire swap
   1. 💩 Pas de configuration pour compose & stack pour le moment
7. ✅🔥🐛 host > /home/the_docker_peon/clientss
8. ✅🐛💥 Problèmes au niveau des backups
   1. ✅🔍🐛 Besoin d'arrêter les conteneur de temp de backup / restaurer
   2. ✅📌 Backup host > tester extraction archive
      1. ✅ mariadb
      2. 🔍🐛 wp
         1. 🚨 contient également wp-config 🚨 dev/prod
   3. ✅📌 Backup local > tester extraction archive
      1. ✅ mariadb
      2. ✅ wp
   4. ✅📌 Injection host > tester ok
   5. ✅📌 Injection local > tester ok
   6. ✅📌 Mise à jour des rôles de backup : stop au debut, re-deploy à la fin
      1. ✅ 🐛 Delay after stop
      2. ✅ Rôles admin 9X-
      3. ✅ Template de forge nginx
      4. ✅ Template de forge wordpress
9. ✅ Passer playbook hello en prefix 201
10. ✅ Clients en 300, 310, 320
11. ✅ Ansible > `[DEPRECATION WARNING]: "include" is deprecated, use include_tasks/import_tasks instead.`

AE

1. ✅ AE > Devis > Clauses rétractation si non payé
2. ✅ Maj facture [mention ae ou chp](https://www.autoentrepreneur.urssaf.fr/portail/accueil/sinformer-sur-le-statut/toutes-les-actualites/une-nouvelle-mention-obligatoire.html)

Perso

1. ✅ Faire la caisse de miaou²
2. ✅ Régularisation électricité

## 16/05/22

Perso

1. ✅ Bouchons oreilles thomann
2. ✅ Acheter etiqueteuse [Dymo](https://www.google.com/search?q=Dymo&oq=Dymo&aqs=chrome..69i57.330j0j1&sourceid=chrome&ie=UTF-8)
3. ✅ Couteaux > acheter guide, pierres++ & cuir
   1. ✅ Livraison 4 & 5 mai

## 06/05/22

Serveur

1. ✅ Récupérer les données de l'ancien pc & mieux versionner
2. ✅ Réinstaller la connexion ssh + tests

## 04/05/22

Process

- Tétrachiée de nouveaux plugins VSCode
  - ✅ Bookmarks
  - ✅🧠 changeCase
    - *Ctrl Shift X* > Choisir
    - *Ctrl Shift W* > Inverser
  - ✅ Code spell checker
  - ✅🧠 "Toggle quotes"
    - *Ctrl + ²*, curseur après la première de la paire de quotes à changer

Perso

1. ✅ Photos apart bérangère
2. ✅ Caisse chatte
3. 💩💩💩⏳ Changement de banque
   1. 💥⏳ Vérifier clôture encore reportée par l'autre sac a merde < OU PAS LOL 💩
4. ✅💩 Annuler concert kflay 14 mai > Pas annulable
5. ✅ Prendre RDV docteur checkup complet
   1. ✅ RDV pris le mardi 26/04 à 15h
   2. ✅ RDV Labo jeudi 28/04 à 8h30
6. Films
   1. ✅ 3615 pere noel

AE

1. ✅ 13/05/2022 > Facture NDD [MKasza](https://mail.google.com/mail/u/0/#inbox/FMfcgzGpFWLJXknFsqDNKVszJCqqvCpn)
2. ✅ Déclaration Auto entrepreneur
   1. ✅ Mars 2022
   2. ✅ Avril 2022

## 26/04/22

Perso

1. ✅ Acheter cable HDMI 5m
   1. ✅ 21/04
2. ✅ Acheter adaptateur pour paint shaker
   1. ✅ 20/04
3. ✅ RDV Malt du 21/04/22
4. ✅ Bières
   1. ✅ Mettre nouveau fût
   2. ✅ Renvoyer anciens fûts
5. ✅ Cadeau anniv dus

## 17/04/22

Perso

1. ✅ Déclaration impôts revenus
2. ✅ Mail J. ferrari
3. ✅ Finir tâches récurrentes

AE

1. ✅ Malt > Renvoyer docs
   1. ✅ Attestation de vigilance
      1. Message envoyé à l'URSAFF le 11/04/22
      2. Recu le 12/04, Renvoyé le 13/04
      3. EN attente de validation de la part de malt
   2. ✅ Avis de situation au répertoire SIREN
      1. Statut passé en public le 11/04/22, en attente de confirmation (24h?)
      2. Attestation à récupérer [ensuite](https://avis-situation-sirene.insee.fr/)
      3. Récupéré et envoyé le 13/04
      4. En attente de validation
2. ✅ Devis > Journée type 7h, 7h30

Cryptor

1. ✅ Devis 2/2
   1. ✅ Facture 2/3
   2. ✅ Facture 3/3
   3. ✅ Ajout au doc Paiement impots AE
2. ✅ Création de l'environnement client
3. ✅ Création du projet github infra

PB Modélisme

1. ✅ Relance PB Modelisme taf de leur côté > 19/04/22

## 11/04/22

Rapide

1. ✅ Virer Done
2. ✅ Versionner TODOs
3. ✅ Docs PB Modélisme
   1. ✅ Signature cahier des charges
   2. ✅ Devis
   3. ✅ Factures
   4. ✅ Maj doc Paiements & factures AE
4. ✅ Tâches récurrentes > terminer réinstallation environnement de dev
5. ✅ Cleaner TODOs
   1. ✅ Versionner TODOs
6. ✅ Réinstaller [environnement de dev](https://github.com/youpiwaza/install-dev-env) sur nouveau pc
   1. ✅ install-dev-env > Upgrade vers [ubuntu 22](https://linuxconfig.org/how-to-upgrade-ubuntu-to-22-04-lts-jammy-jellyfish) & ✅ doc
   2. ✅ install-dev-env > `01-terminal` terminé
   3. ✅ WSL
   4. ✅ Docker desktop

Perso

1. ✅ Paiement syndic
2. ✅ Commander bières
3. ✅ Poster lettre infos impôts

## 02 & 03/22

Taf

1. ✅ Lapie > Changer image accueil > ratafia
2. Raccourcis & process à intégrer au flow
   1. ✅🧠 Copier coller historique > Activer l'hitorique
      1. *windows + V*
   2. ✅ Better comments

Perso

1. ✅ Versionner TODOs
2. ✅ Régulariser impots janvier 2022 pour décembre 2021
   1. ✅ Demande de régularisation
   2. ✅ Virement ponctuel de régularisation
   3. ✅ Confirmation prise en compte
   4. ✅ Confirmation pas de frais de retard
3. ⏳ Changement de banque
   1. ✅ Ouverture de compte
   2. ✅ CB
   3. ✅ Provisionner
   4. ✅ Transfert des opérations courantes & soldes restants
   5. ✅ Message à l'ancienne banque pour résiliation
      1. ✅ Envoi lettre recommandée, en attente de bonne reception, envoyé le 04/03/2022
   6. ✅ Dernière facture 26D > Transmettre nouveau RIB
   7. ✅ Paiement AE
   8. ✅ Maj factures AE
   9. ✅ Maj bankin
   10. ✅ Récupérer IBANs enregistrés
   11. ✅ Maj amazon
   12. ✅ Maj Paypal
   13. ✅ Maj paiement le bon coin
   14. ✅ Analyser opérations en cours sur compte courant BRED et tout flinguer !!!
       1. ✅ Assurance Alan
       2. ✅ Popa
       3. ✅ Deliveroo
       4. ✅ Abo piscine
       5. ✅ Forfait tel sosh
       6. ✅ Urssaff
       7. ✅ OVH / via paypal
       8. ✅ SYS / via paypal
       9. ✅ Ameli : Vérifier ou refaire, service indisponible -_-
       10. ✅ Impôts
           1. ✅👤 Perso / Pas d'IBAN ou de mandat pour le moment
           2. ✅💩💩💩 Pro / Compte courant boursorama, à passer sur compte pro quand créé, cf ci-dessous
   15. ✅💩💩💩 Retour de l'autre connard > souscription à une autorisation de découvert au lieu de résiliation
       1. ✅  YAVAI PAS BESOIN LAUL
   16. ⏳ Vérifier clôture encore reportée par l'autre sac a merde
4. 💩 Compte Pro boursorama / C'est mort, whatever
5. ✅ Remplacement tireuse à bière
   1. ✅ Laver, étiquettes, paquet
   2. ✅ Renvoyer à SB via mondial relay
   3. ✅ Reçu & good

## 01/22

Vers

1. ✅ Mails
   1. ✅ Le bon coin
   2. ✅ Ameli
   3. ✅ Fond ecran gokudolls
2. ✅ Changer pass dashlane
3. ✅ 211127 Faire comptes > reste 300 balles en comptant les impots début décembre
4. ✅ Message banque 20 balles wtf
5. ✅ Rappeler conforama confirmer / 15 17 46 7
6. ✅ Emballer cadeau nonore
7. ✅ Facture taf
8. ✅ Facture hébergement
9. ✅ Taf
   1. ✅ Envoyer CRA et mes CRA
   2. ✅ Confirmer virement
   3. ✅ Déclaration AE novembre
   4. ✅ Noter Date prélèvement impôts octobre
   5. ✅ Loyer janvier
   6. ✅ Participation décembre
10. ✅ Litère chatte
11. ✅ Gérer trains pour chez anouk
    1. ✅ Retour max
    2. ✅ AR vigi
12. ✅ Choix & commande tireuse à bière
13. ✅ Rembourser daron
      1. ✅ reste 1250€
14. ✅ Imperméabiliser pompes
15. ✅ Carte électorale
16. ✅ Cadeaux nowel
    1. ✅ Theatre de paris michalak
    2. ✅ Tireuse à bière
    3. [Voyages a 1€](https://www.voyagespirates.fr/vols/mega-promo-vols-a-partir-de-1eur)
17. ✅ Envoyer pinata a pauline
18. ✅ Billets train anouk
19. ✅ Décaler billets cette semaine
20. ✅ Billets fin d'année
21. ✅ Bloodywook 22 mars trabendo

Lapie

1. ✅ Réparer galerie photos
2. ✅ Nouvelle photo ratafia
3. ✅Nouveau tarifs transports
   1. De 6 à 12 bouteilles 2€50 par bouteille
   2. De 18 à 96 bouteilles 2€ par bouteille
   3. Plus de 96 bouteille, livraison offerte (note max : Je l'ai donc détaxée, même si virtuellement cela ne change rien)
      1. 2 demi bouteilles comptent comme 1 bouteille
      2. 1 magnum compte comme  2 bouteilles
   4. ✅ Mettre à jour le choix automatique dans le panier en fonction du nombre de bouteilles
4. ✅ Mises à jour plugins & traductions
5. ✅ Pages référencement naturel "wikipedia" : à masquer
   1. ✅ Mise à jour de la page "Plan du site"
   2. 🚨 Note: Les pages n'ont pas été supprimées, mais ont été masquées (passée en publication "privée")
   3. 🚨 Note: Lorsqu'on est connecté en administrateur, le plan du site affiche les pages privées, mais pour le public non ;)

## 10/21

Trucs **la maintenant**

1. ✅ Ranger affaires
2. ✅ Wp fof
3. ✅ Billets train semaines suivantes
4. ✅ Gérer edt portable
5. ✅ Bière fof bédot / margot
6. ✅ SNCF Carte pro
   1. ✅ Commander carte
   2. ✅ Dématérialiser ~mail, appli pue la merde
   3. ✅ Résa prochains voyages
   4. ✅ Annuler billet credi et recommander moins cher ?
7. ✅ Thunes payées
   1. ✅ Mail 26 Digital + Excel Paiement AE
   2. Virements compte commun
      1. ✅ Dépannage > Impôts alakon
      2. ✅ Loyer novembre
      3. ✅ Syndic
   3. ✅ Vérifier & régler virements non effectués
      1. ✅ Alan
      2. ✅ Autres ? Nope
8. ✅ Message cartonnerie gg balance ginger
9. ✅ Avis google 26 Digital
10. ✅ Maintenance serveur
11. ✅ Mise en ligne site fof
12. ✅ Extraire Edt portable
13. ✅ Extraire edt mails
14. ✅ Dashlane twitch.tv changer pass

Trucs **persos**

1. ✅ Annuler [gorillaz](https://songkick.fnacspectacles.com/compteclient/detailTransaction.do?transactionId=4551758280325692730)
   1. Fnac songkick
   2. En attente de retour fnac songkick
   3. En attente retour paylogic
2. ✅ vignette crit'air 1
   1. ✅ Commandée le 05/09/21, en attente de retour
3. ✅ orga week end dralex
   1. ✅ Retour Angelike heberg

## 06/09/21

Trucs **persos**

1. ✅ Cadeau moman > Partitions compilation FF
2. ✅ Coiffeur > Coiff&Co sans RDV Adresse : 14 Rue de Courcelles, 51100 Reims
3. ✅ Croquettes chien 12kg

## 30/08/21

Trucs **persos**

1. ✅ maj wallpapers sur github
2. ✅ Répondre mercer enculés
   1. 210903 > Répondu par mail & [courrier recommandé](https://mail.google.com/mail/u/0/#search/mercer/FMfcgxwHNMWCgjZtpBWqGPQSkwCJgvKg)

Trucs **taf**

1. ✅ TO DO récurrents
   1. ✅ go checker chkdsk
   2. ✅ Firmware SSDs
2. ✅ Ranger la première page de Liste de liengs + remplacer par une intro au fichier
3. ✅ WP picard
    1. Facture NDD [picards](https://mail.google.com/mail/u/0/#inbox/FMfcgzGkZZwLntCGLnPgcLNCzSlJVKlg)
        1. Facture envoyée le ~18/08/21
        2. Payé le 6/09/21
    2. ✅ spam > virer commentaires
4. ✅ 26 Digital
   1. ✅ Horaires 9h à 18h
   2. ✅ Devis + Signatures
   3. ✅ Factures
      1. ✅ Envoi facture acompte septembre
   4. ✅ réservation trains
      1. ✅ Première semaine
         1. Aller : mardi 7 septembre 2021 à 06:45
         2. Retour : vendredi 10 septembre 2021 à 19:58
      2. ✅ 2eme semaine
         1. Aller : lundi 13 septembre 2021 à 06:45
         2. Retour : vendredi 24 septembre 2021 à 19:58
5. ✅ Ursaff > attestation de vigilance
   1. Message envoyé sur ae.urssaf.fr le 01/09/21
   2. ✅ Puis envoyer sur malt

Trucs **serveur**

1. ✅🐛 SSH / key KO (déjà ~merdique avant) avec la nouvelle version de filezilla (problème conversion en putty)
   1. ✅ Maj du script de clés ssh
      1. ✅ Maj role users
         1. ✅ Création de la clé sur l'hôte a partir de ansible user
         2. ✅ Test de connexion via bob
         3. ✅ DEPRECATED l'ancienne méthode
      2. ✅ Maj create sftp user
         1. ✅ Vérifier que toujours oké avec chroot prison
   2. ✅ Maj des clés SSH **1 par 1** pour les différents utilisateurs présents
   3. Note client ftp : passage de Filezilla à WinSCP
2. ✅ SFTP / Création d'un utilisateur ubuntu pour connexion ssh, qui remplace ftp (clé publique privée, etc.)
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
         3. ✅ Création d'utlisateurs : ansible\roles\users\tasks\main.yml
            1. 🔍 Utilisation de loop
            2. ✅🔍 Surcharger la variable user qui alimente la boucle ?
               1. ansible\2-generate-users-and-change-ssh-port.yml
               2. Not in our favor [doc ansible variable precedence](https://docs.ansible.com/ansible/latest/user_guide/playbooks_variables.html#variable-precedence-where-should-i-put-a-variable)
               3. [cheat](https://stackoverflow.com/questions/31310688/conditionally-define-variable-in-ansible#comment86310852_43403229)
            3. ✅ User default shell zsh if present
               1. Si package zsh est la > shell zsh
         4. ✅ Se remettre dans le bain
            1. ✅ Lire scripts de creation de user et les apprendre
            2. ✅ Lire les TODO ci-dessous dans la liste
            3. ✅ Relire articles tecmint
            4. ✅ Check contenu `/etc/ssh/sshd_config`
            5. ✅ Tester sshd_config > `sshd -t` > si retourne rieng c'est good
            6. ✅ Le user bob à possibilité de se promener grave (`cd ..`)> besoin de restriction /home >> Suivre tutos
               1. ✅ À la main
                  1. ✅ Ok dans répertoire à la racine /test_chroot
                  2. 💩 Tester avec ssh_d/*.conf
                     1. Créer un fichier `sshd_config.d/*.conf` par utilisateur
                     2. `/etc/ssh/sshd_config.d/*.conf` files are included at the start of the configuration file, so options set there will override those in /etc/ssh/sshd_config.
                     3. Attention
                        - For file transfer sessions using SFTP no additional
                        - configuration of the environment is necessary if the in-process sftp-server is used,
                        - though sessions which use logging may require /dev/log inside the chroot directory
                        - on some operating systems (see sftp-server(8) for details).
                     4. Note max:
                        1. Virtuellement c'est bon mais ça ne fonctionne pas (force command KO dans fichier autre que sshd_config ? wat)
                        2. ✅ Alternative: Utilisation de restrictions de groupe & pattern %u
                  3. ✅ Tester dans /home/the_docker_peon/
                  4. ✅ Ranger & Traduire notes
                  5. ✅ Cleaner noms groupes & arbo
            7. ✅ Noter commande pour supprimer user et re-tester script d'ajout
         5. ✅ Automatiser, créer des rôles
            1. ✅ Rôle préparation de prison chroot
            2. ✅ Rôle ajout utilisateur sftp
               1. ✅ IMO Créer un nouveau rôle et réutiliser certaines parties du rôle user plutôt que de goyer comme jamais
               2. ✅ Tuto
               3. ✅ Adapté aux projets
               4. ✅ Créer un playbook de create sftp user a la volée sans projet, pour créa accès direct
            3. ✅ Rôle suppression utilisateur sftp
               1. ✅ Virer tests
                  1. bob
                  2. bobby
                  3. bobba
         6. ✅ Cleaner
            1. ✅ user bob + /home
            2. ✅ la clé ssh de bob du serveur
            3. ✅ les tests /the_docker_peon/clients/_website_machin
         7. ✅ Génération des identifiants utilisateurs (doc .md pour client)
            1. Possibilité de se baser sur
               1. ansible\roles\users\tasks\generate-users-manual-commands.yml
               2. ansible\roles\users\templates\ssh-users-manual-commands.md.j2
         8. ✅ Lint ansible-install-web-server\ansible\roles\users\main.yml
         9. ✅ Update ansible-install-web-server\ansible\roles\users\README.md

## 23/07/21

Perso

1. ✅ Régime hyper prot

Serveur

1. ✅ Activer github copilot
2. ✅ install-dev-env > Compilation set up VSCode

## 25/07/21

Perso

1. ✅ Re-commander compléments alimentaires
2. ✅ Renouveler anti virus [eset](https://a7286.boutique-eset.com/renouveler-sa-licence?lic=EAV-0232681294&hash=yLLLFeMk6/TOqsPDgGPSeRsPxQgPBAtX0ZscRxHqkPC35cB7QkUa&utm_campaign=renew&utm_content=eav&utm_medium=ipm&utm_source=application&utm_term=_3_renew_4_fr_5_eav_6_30-26e_7_q3-2020)
3. ✅ Cadeaux vigi
4. ✅ Cadeau Julie

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
            2. Arbo logique ek details `THE_DOCKER_GUY/backups/volumes/clients/LE_CLIENT/SITE_COM/ANNEE/nom-volume---backup---$(date +%Y-%m-%d--%H.%M.%S).tar`
            3. Mais, les noms de volumes ont de l'info, ex : `client---dev--masamune-fr---wordpress--db`, mais les sauvegardes seront récurrentes (vite le bordel si beaucoup de fichiers)
            4. `THE_DOCKER_GUY/backups/volumes/ANNEE/TYPE/LE_CLIENT/SITE_COM/nom-volume---backup---$(date +%Y-%m-%d--%Hh%Mm%Ss).tar`
            5. Eg. `THE_DOCKER_GUY/backups/volumes/2021/clients/masamune/dev--masamune--fr/client---dev--masamune--fr---wordpress--db---backup---2021-05-27--11h23m57s.tar`
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
