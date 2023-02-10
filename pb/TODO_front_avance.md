# TODO / Front > Avancé

Reste à faire concernant les plugins, comportements, tris

## Réduction des prix des produits en fonction de la quantité commandée

Passer par un plugin payant, l'autre merde toujours et plus de réponse du support

1. Doit pouvoir gérer correctement HT & TVA, sur l'ensemble du site, panier, commandes, histo commandes
2. Doit pouvoir gérer TVA désactivée (comptes spéciaux)
3. Doit pouvoir être importé, cf. ancien plugin

✅ Prendre les 3 plus connus > bench > contacter pour voir tps de réponse

⏳💸 Attente achat plugin

## Page intermédiaires

Création des pages intermédiaires

Rouge PB / #941210

1. 🚀 Nouveautés
2. Produits phares
3. Inspiration
4. Promotions catégories
5. Promotions
6. Catégories principales
   1. Avions
   2. Drones
   3. Voitures
   4. Bateaux
   5. Maquettes
   6. Matériaux
   7. Accessoires
   8. Aerogtaphes
   9. Outillages
   10. Moteurs
   11. Carburants
   12. RadioS
   13. Pièces détachées
   14. Accessoires véhicules
         1. Toutes les sous cat
7. Détaillants
8. Accueil FAQs

## Menu principal, cf. `/_docs/craft-and-tests/19-menu-principal/README.md`

1. Faire une ébauche bootstrap custom, en local afin de ne pas péter un plomb
2. Remplacer sur site actuel
3. Recettage Nonore
4. Recettage PB

## Page Contact

Page [Contact](https://dev.pb-modelisme.com/contact/)

1. Vérifier cookies machins (carte)
2. Rajouter Captcha
3. Formulaire > Peut importe le service, envoyer à la meme adresse mail
4. Supprimer l'adresse mail affichée en clair, on ne conserve que le formulaire

## Page Marques

Page [Marques](https://dev.pb-modelisme.com/marques-partenaires/) > Revoir le contenu de la page

1. Première partie colonnage par type de véhicules
   1. Chaque colonne contient 3 à 5 marques choisies pour ce type de véhicules
2. En 2eme partie - broder du contenu on a plein de marque
3. 3eme partie > liste de A a Z
4. Traduction du plugin

## Un produit > Autoriser les commandes en réapprovisionnement ?

1. AFF___ Etat 2 & 📝 Sur commande VRAI
   1. > Front > "En réapprovisionnement"
2. AFF___ Etat 2 & 📝 Sur commande FAUX
   1. > Front > "Sur commande"

---

## Moteur de recherche

Autoriser la recherche par SKU/UGS, & par les autres refs

### Tris

1. Faire l'inventaire des tris existants
2. Voir si il y a des choses à rajouter/supprimer

---

## Clients

### Devis

1. ✅ Ajouter un statut à la commande "Devis"
2. Page dédiée sur l'interface client
   1. Faire apparaître les devis
   2. Bouton client, passer à état "commande en cours"

### Possibilité imprimer/dl factures en pdf, etc

yup

---

## Pages d'affichage des catégories

yup

## Multilinguisme

via plugin Google translate

## Plugin "liste de souhaits"

yup

---

## Done

## Done / Menu principal, cf. `/_docs/craft-and-tests/19-menu-principal/README.md`

1. ✅ Eclater l'ancien menu bordélique, tout reset, virer barre supérieure
2. ✅ Liste l'arborescence du menu
3. ✅ Analyse de la concurrence / inspiration
    1. ✅ Faire valider par PB avant de passer à la refonte
    2. ✅ Je suis décideur & je fais au mieux, cf. [mail du 25/01/23](https://mail.google.com/mail/u/0/#inbox/KtbxLzGLlqFwflnkMgjQWGCgcRHSqpBjJq)

## Done / Un produit > Retours à traiter

Mail du [28/01/23](https://mail.google.com/mail/u/0/#inbox/FMfcgzGrcPHMWNbGMQcvcNqQHlnJkXnC)

1. ✅ Pas d'affichage du nombre d'article en stock
   1. Admin WC > Produits > Inventaire > Ne jamais afficher le stock restant
2. ✅ Mention du stock plus visible (plus gros et indicateur visuel)
3. ✅ Groupes miniatures produits
   1. ✅ Remplacer par les visuels "séparés", et non collés les unes aux autres
      1. ✅👷 Visuel souhaité onglet "Produits similaires", "Aérographes / Comrpesseurs", "Colles"
      2. ✅ Remplacer Description > "Matériel à prévoir"
         1. ✅ En faire un onglet dédié, commun à tous
            1. ✅♻️ Clean chargement des onglets communs
            2. ✅ Supprimer le contenu de la description
            3. ✅ Création de l'onglet
            4. ✅ Ajout du contenu
            5. ✅⚡️ Nouveau visuel > Mise à jour de la fonction commune
      3. ✨ Onglets / ✨ Mis à jour automatiquement via la fonction commune
         1. ✨ "Peintures conseillées"
         2. ✨ "Pièces détachées"
         3. ✨ Chargeurs > "Produits compatibles"
         4. ✨ Moteurs > "Bougies conseillées"
         5. ✨ Moteurs > "Carburants conseillés"
      4. ✅ En dessous de la fiche produit
         1. ✅ Produits associés
         2. ✅ Produits similaires
            1. Prend Toute la largeur si premier bloc absent ~~**OU** en faire un onglet~~
4. ✅ Miniatures produits, ajouter
   1. ✅ Tarif
   2. ✅ Etat du stock
   3. ✅ Bouton acheter
   4. ✅ Style
5. ✅ Caractéristiques techniques
   1. ✅ Ne pas afficher les dimensions du colis
   2. ✅ Afficher les icônes après le texte
6. ✅ Prix multiples plus gros
7. ✅ "Zone achat" clairement identifiable, cf. site PB actuel (~ajouter un cadre)
8. ✅ [voiture test](https://dev.pb-modelisme.com/produit/test-voiture-completement-rempli/)
    1. ✅ Bug affichage eco taxe
    2. ✅ Nombre de moteur, n'afficher que le chiffre
9. ✅ [Récepteurs](https://dev.pb-modelisme.com/produit/test-recepteurs-completement-rempli/)
    1. ✅ Supprimer onglet utilisation conseillée
    2. ✅ Caractéristiques techniques
       1. ✅ "Est cumulable ?" > Supprimer "Est"
       2. ✅ "Est compatible télémétrie ?" > Supprimer "Est"
       3. ✅ Portée > Affichée en mètres
          1. 👌 Ajusté pour l'ensemble des champs : si unité mm
             1. Si > 1 000 000 > affiché en km
             2. Sinon si > 1 000 > affich& en m
10. ✅ [Servos](https://dev.pb-modelisme.com/produit/test-servos-completement-rempli/)
    1. ✅ Caractéristiques techniques
       1. ✅ Supprimer Diamètre
       2. ✅ Supprimer Diamètre exterieur du tube
11. ✅ [Radios](https://dev.pb-modelisme.com/produit/test-radio-completement-rempli/)
    1. ✅ Déplacer Carac techniques dans onglet
       1. ✅ Déplacer "Ref servo" et "ref récepteur" dans un onglet "produits associés"
          1. ✅ Virer des CT
          2. ✅ Créer onglet
          3. ✅ Charger onglet
          4. ✅ Contenu
             1. ✅ Récupérer le produit de référence via SKU
             2. ✅ x2
             3. ✅ Afficher
                1. ✅👌 Si SKU trouvé on affiche le produit
                2. ✅ Sinon on affiche la ref
                3. ✅ x2
12. ✅ [Pièces voitures](https://dev.pb-modelisme.com/produit/test-pieces-voitures-completement-rempli/)
    1. ✅ Renommer Onglet "construite" en "châssis associé"
13. ✨ Pièce moteur thermique
    1. ✨ Supprimer l'onglet "documents"
       1. 👌 Affichage conditionnel pour tous les produits plutôt
14. ✅ Pièces hélicos
    1. ✅ Supprimer diamètre
15. ✅ [Moteur thermique](https://dev.pb-modelisme.com/produit/test-moteurs-thermiques-completement-rempli/)
     1. ✅ Carac techniques
        1. ✅ Remplacer compatibilité par "Usage courant :"
        2. ✅ Hélices conseillées > Afficher "Diamètre min x pas min" et "diamètre max x pas max"
16. ✅ [Moteurs électriques](https://dev.pb-modelisme.com/produit/test-moteurs-electriques-completement-rempli/)
    1. ✅ Carac tech
       1. ✅ Supprimer champ "capacité"
17. ✅ [Matériaux](https://dev.pb-modelisme.com/produit/test-materiau-completement-rempli/)
    1. ✅ Onglet "Colles conseillées"
       1. ✅ Renommer "Colles"
       2. ✅ Contenu > Affichage de la catégorie colles
18. ✅ [Maquettes](https://dev.pb-modelisme.com/produit/test-maquette-completement-remplie/)
    1. ✅ Masquer onglet "pièces détachées"
    2. ✅🐛 Onglet "Produits conseillés" > Mauvais contenu ?*
       1. Yep, il correspond à la catégorie moteurs électriques, c'est corrigé
    3. ✅ Carac techniques
       1. ✅ Supprimer poids
       2. ✅ Supprimer nombre de moteurs
          1. ✅👌 Pas affiché si non défini / NULL
19. ✅ [Matériaux](https://dev.pb-modelisme.com/produit/test-materiau-completement-rempli/)
    1. ✅ Maj de l'import : Ajouter le nom de la sous catégorie au nom du produit
       1. ✅ Par exemple le site affiche 3x5 au lieu de baguette balsa 3x5
       2. ✅ Mise à jour de la requête craft
       3. ✅📌 Export CSV
       4. ✅ Mise à jour de la requête finale
       5. ✅ Import lancé en mise à jour
          1. ✅📌 Produits > Catégorie > ["Matériaux"](https://dev.pb-modelisme.com/wp-admin/edit.php?s&post_status=all&post_type=product&action=-1&product_cat=materiaux&product_type&stock_status&filter_action=Filtrer&paged=1&action2=-1)

## Done / Pages statiques

1. ✅ Analyse de la concurrence / inspiration
    1. ✅ Faire valider par PB avant de passer à la refonte
    2. ✅ Je suis décideur & je fais au mieux, cf. [mail du 25/01/23](https://mail.google.com/mail/u/0/#inbox/KtbxLzGLlqFwflnkMgjQWGCgcRHSqpBjJq)

## ✅ Done / Un produit > Retours à traiter

Mail du 31/01/23.

1. ✅ Front > Un produit > Supprimer l'onglet "Brand"
2. ✅ Front > Un produit > Bouton acheter plus coloré, mieux mis en avant

## Done / Page d'accueil

1. ✅ Nouvelle page afin de regrouper les pages d'illustration de thème
2. 📌 Associer des blocs Divi aux contenus retenus
   1. (Manque du gras niveau template > go [divi online store](https://www.elegantthemes.com/layouts/category/online-store))
      1. 5 blocs > [Travel Agency Home Page](https://www.elegantthemes.com/layouts/business/travel-agency-home-page)
      2. Grille produits > [Boutique Landing Page](https://www.elegantthemes.com/layouts/business/boutique-landing-page)
      3. Grille Panaché > [Jeweler Landing Page](https://www.elegantthemes.com/layouts/art-design/jeweler-landing-page)
   2. ✅ Produits / Carousel / Divi [slider](https://www.elegantthemes.com/preview/Divi/slider/)
      1. Produits récents avec mise en avant
      2. Produits phares avec mise en avant
      3. Inspiration, catégorie mise en avant
      4. Marques populaires
   3. ✅ Promotions / **brs-boutique > Popular Products**
      1. Catégories ou produits
      2. Offres du moment : promotions temporaires
   4. ✅ Boutique, 2 lignes de textes + lien vers à propos / **Hardware Store Shop Page All tools**
      1. Kwaksé, engagements, nombre de produits & marques, expertise
   5. ✅ Catégories principales ~Véhicules / **Hardware Store Landing Page Shop categories**
   6. ✅ Services / **brs-accueil > Services**
   7. ✅ Incontournables : 2 blocs, carousels ? ou 2 lignes 1 titre 4 produits carousel / **Hardware Store Home Page giving back environnement** c'un carousel en faire 2
      1. Nouvelles sorties
      2. Recommandations
   8. ✅ Inspiration / **hs-accueil triple bloc GET UP TO 65% OFF**
      1. A découvrir
         1. Maquettes **(bloc fixe de gauche)**
         2. Tunnels d'intérêts sur sous page : Peinture, sculpture, matériaux, décors, collections **Carousel à droite**
      2. Tendances (~en fonction de la saison) **Bloc du bas**
   9. ✅ Bandeau avantages / **brs-boutique > Bandeau Free Shipping** OU **hs-accueil weekly savings**
      1. 4 colonnes, Picto + 1 titre et c'est tout (~livraison, expertise, disponibilité, pièces détachées rares)
   10. ✅ Tunnels utilisateurs catégories profondes (~sous catégories accessoires) / **hs-a-propos 3 images Giving Back to the Environment**
       1. Matériaux (Bois, flocages)
       2. Outillage (Aero, tournevis, colles, peintures, etc.)
       3. Pièces détachées
   11. ✅ Actualités, 2 blocs, 1 carousel, 1 fixe **Hardware Store Home Page giving back environnement**
       1. Actualités du site (articles)
       2. Cross média (youtube)
   12. ✅ Mise en avant de pages profondes / **hs-accueil Popular Brands > Faire 5 colonnes**
       1. Produits phares
       2. Bonnes affaires
       3. Destockage
       4. Espace sociétés (détaillants)
       5. Aide
          1. FAQs / **hs-contact faq**
          2. Contact
3. ✅ Mise en place des blocs
   1. ✅ Produits / Carousel / Divi [slider](https://www.elegantthemes.com/preview/Divi/slider/)
      1. ✅ Produits récents avec mise en avant
      2. ✅ Produits phares avec mise en avant
      3. ✅ Inspiration, catégorie mise en avant
      4. ✅ Marques populaires
   2. ✅ Promotions / **brs-boutique > Popular Products**
      1. ✅ Catégories ou produits
      2. ✅ Offres du moment : promotions temporaires
   3. ✅ Boutique, 2 lignes de textes + lien vers à propos / **Hardware Store Shop Page All tools**
      1. ✅ Kwaksé, engagements, nombre de produits & marques, expertise
   4. ✅ Catégories principales ~Véhicules / **Hardware Store Landing Page Shop categories**
   5. ✅ Services / **brs-accueil > Services**
   6. ✅ Incontournables : 2 blocs, carousels ? ou 2 lignes 1 titre 4 produits carousel
      1. ✅ Nouvelles sorties
      2. ✅ Recommandations
   7. ✅ Inspiration / **hs-accueil triple bloc GET UP TO 65% OFF**
      1. ✅ À découvrir
         1. ✅ Maquettes **(bloc fixe de gauche)**
         2. ✅ Tendances (~en fonction de la saison) **Bloc du bas**
      2. ✅ Tunnels d'intérêts sur sous page : Peinture, sculpture, décors, collections, matériaux **Carousel à droite**
   8. ✅ Bandeau avantages / **brs-boutique > Bandeau Free Shipping** OU **hs-accueil weekly savings**
      1. 4 colonnes, Picto + 1 titre et c'est tout (~livraison, expertise, disponibilité, pièces détachées rares)
   9. ✅ Tunnels utilisateurs catégories profondes (~sous catégories accessoires) / **Bike repair > landing > Services**
       1. ✅ Accessoires en général
       2. ✅ Outillage (✅ Aero, ✅ tournevis, colles & produits, carburants, etc.)
       3. ✅ Pièces détachées
       4. ✅ Batteries
   10. ✅ Actualités, 2 blocs, 1 carousel, 1 fixe **Hardware Store Home Page giving back environnement**
       1. Actualités du site (articles)
       2. Cross média (youtube)
   11. ✅ Mise en avant de pages profondes / **hs-accueil Popular Brands > Faire 5 colonnes**
       1. Produits phares
       2. Destockage
       3. Espace sociétés (détaillants)
       4. Aide
          1. FAQs / **hs-contact faq**
          2. Contact
4. ✅ Mettre en place les liens vers les pages existantes
   1. ✅ & référencer les pages à créer
5. ✅ Check le responsive
   1. ✅ Tablette
      1. 🌱 Pas parfait, forcer quelques colonnages
   2. ✅ Mobile
6. ✅📧 Envoi à Nonore pour recettage graphismes
