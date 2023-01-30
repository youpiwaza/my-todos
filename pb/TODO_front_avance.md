# TODO / Front > Avancé

Reste à faire concernant les plugins, comportements, tris

## Réduction des prix des produits en fonction de la quantité commandée

Passer par un plugin payant, l'autre merde toujours et plus de réponse du support

1. Doit pouvoir gérer correctement HT & TVA, sur l'ensemble du site, panier, commandes, histo commandes
2. Doit pouvoir gérer TVA désactivée (comptes spéciaux)
3. Doit pouvoir être importé, cf. ancien plugin

✅ Prendre les 3 plus connus > bench > contacter pour voir tps de réponse

⏳💸 Attente achat plugin

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
        1. Colles conseillées > Requête complexe en fonction de la sous catégorie
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

## Page statiques

1. ✅ Analyse de la concurrence / inspiration
    1. ✅ Faire valider par PB avant de passer à la refonte
    2. ✅ Je suis décideur & je fais au mieux, cf. [mail du 25/01/23](https://mail.google.com/mail/u/0/#inbox/KtbxLzGLlqFwflnkMgjQWGCgcRHSqpBjJq)
2. Lister les pages à réaliser & arborescence
3. Prioriser
4. Yapuka

## Page Contact

Page [Contact](https://dev.pb-modelisme.com/contact/)

1. Vérifier cookies machins (carte)
2. Rajouter Captcha
3. Formulaire > Peut importe le service, envoyer à la meme adresse mail

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
