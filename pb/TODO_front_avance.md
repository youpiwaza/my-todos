# TODO / Front > Avancé

Reste à faire concernant les plugins, comportements, tris

## Réduction des prix des produits en fonction de la quantité commandée

Passer par un plugin payant, l'autre merde toujours et plus de réponse du support

1. Doit pouvoir gérer correctement HT & TVA, sur l'ensemble du site, panier, commandes, histo commandes
2. Doit pouvoir gérer TVA désactivée (comptes spéciaux)
3. Doit pouvoir être importé, cf. ancien plugin

✅ Prendre les 3 plus connus > bench > contacter pour voir tps de réponse

⏳💸 Attente achat plugin

## Un produit > Retours à traiter

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
          1. 🚀📌 Produits > Catégorie > ["Matériaux"](https://dev.pb-modelisme.com/wp-admin/edit.php?s&post_status=all&post_type=product&action=-1&product_cat=materiaux&product_type&stock_status&filter_action=Filtrer&paged=1&action2=-1)

## Un produit > Contenus complexes ~ onglets

Cédric me renvoie tous les champs normalisés comme liste de peinture

✅📝 Règles d'affichage front pour les champs contenant du nouveau (Relation) & legacy :

- Si il y a des peintures ajoutée via le nouveau champ relation, on n'affiche que elles
- Si il n'y en a pas mais qu'il y a des peintures dans le champ légacy
  - on les affiche
- 🚨 Pas de mix des deux.

1. Onglets supplémentaires
    1. Avions
       1. Pièces détachées / Plan
       2. Articles conseillés
    2. Bateaux
       1. Pièces détachées
    3. Batteries
       1. Produits compatibles
          1. Contenu
       2. Chargeurs compatibles
          1. Contenu
    4. Controleurs
       1. Produits compatibles > Requête à récupérer / convertir
          1. Contenu
    5. Helices avions
       1. Piéces détachées > Requête complexe
       2. Accessoires conseillés > Requête à récupérer / convertir
    6. Helicos
       1. Piéces détachées > Requête à récupérer / convertir > `site actuel pb modelisme\Helico\prodassoc.php` > lol nope
       2. Piéces Upgrade > Requête complexe > idem
    7. Maquettes
       1. Produits de finitions > Récupérer requête complexe (plusieurs catégories)
    8. Matériaux
        1. Colles conseillées
           1. cf. Mail du [28/01/23](https://mail.google.com/mail/u/0/#inbox/FMfcgzGrcPHMWNbGMQcvcNqQHlnJkXnC)
           2. Renommer "Colles"
           3. Contenu > Affichage de la catégorie colles
    9. Moteurs thermique
        1. Piéces détachées > Requête complexe table constitue ?
    10. Pièces hélicoptères
        1. Machines compatibles > 🔗 Table "compose"
    11. Pièces voitures
        1. ? > 🔗 Table "construite"
    12. Recepteurs
        1. Utilisation conseillée/s > 🔗 table "categorieavion", 🔗 table "utilise"
        2. Produits compatibles
    13. Servos
        1. Piéces détachées
    14. Voitures
        1. Pièces détachées > Récupérer requête ancien site
        2. Pièces Options > Pieces voitures avec champs OPT à 2 (pièces pour upgrade)
           1. Note max : Ref à la catégorie pièces détachées pour voitures

## Menu principal, cf. `/_docs/craft-and-tests/19-menu-principal/README.md`

1. ✅ Analyse de la concurrence / inspiration
    1. ✅ Faire valider par PB avant de passer à la refonte
    2. ✅ Je suis décideur & je fais au mieux, cf. [mail du 25/01/23](https://mail.google.com/mail/u/0/#inbox/KtbxLzGLlqFwflnkMgjQWGCgcRHSqpBjJq)
2. Menu principal
   1. Lister la nouvelle arborescence
   2. Anciens contenus conservés
   3. Nouveaux contenus à mettre en avant
   4. Suggestions suite à l'analyse de la concurrence
   5. Page intermédiares, cf. leroy merlin
3. Faire une proposition de menu amélioré (images / onglets, etc.)
4. Faire une proposition de rubriques optimisées
5. Recettage Nonore
6. Recettage PB

## Pages statiques

1. ✅ Analyse de la concurrence / inspiration
    1. ✅ Faire valider par PB avant de passer à la refonte
    2. ✅ Je suis décideur & je fais au mieux, cf. [mail du 25/01/23](https://mail.google.com/mail/u/0/#inbox/KtbxLzGLlqFwflnkMgjQWGCgcRHSqpBjJq)
2. Lister les pages à réaliser & arborescence
   1. Services > Se baser sur les pages services du site actuel
      1. réparations et la découpe
      2. [Services](https://pb-modelisme.com/Accessoires/listeprod.php?cat=35)
      3. Cookies et confidentialité
      4. Plan du site
   2. Mail Cédric du [28/01/23](https://mail.google.com/mail/u/0/#inbox/FMfcgzGrcPHMMxrqFCqSCKtvsjfZCcXw)
      1. Mentions légales : ok
      2. CGV : OK
3. Prioriser
4. Yapuka

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
