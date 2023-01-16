# TODO / Back

Reste à faire concernant les imports de données depuis l'ancien site

---

## ⏳ Contenus complexes ~ onglets

Cédric me renvoie tous les champs normalisés comme liste' de peinture

Affichage front :

Si il y a des peintures ajoutée via le nouveau champ relation, on n'affiche que elles

Si il n'y en a pas mais qu'il y a des peintures dans le champ légacy
  on les affiche

> Pas de mix des deux.

### Ajustements Page Un produit

Liste de peintures > Virer de la description, onglet uniquement

Pièces détachées > passer en onglet + Utiliser l'affichage de "Peintures conseillées"

---

## Import des clients, ainsi que des commandes

Tables concernées "usr", "commande" & "article".

- `usr` contient l'ensemble de nos clients
- `commande` regroupe toutes les infos de la commande ou des ventes magasins (paiement, adresse, n° de colis...)
- `article` contient la référence, l'ID, le numéro de la table dans laquelle l'article ce trouve, les quantités commandé, livrée, le tarif au moment de la commande.... etc

### Importer les comptes clients, table `usr`

1. ⏳(Cédric) 📝 Documenter la BDD actuelle
   1. ✅ Base en place, en attente de complétion / validation

### Importer l'historique des commandes clients, tables `commande` & `article`

Besoin des articles & des comptes clients

1. Import des commandes
2. Association des commandes aux clients / ventes caisses

Plugin [Product Import Export for WooCommerce](https://wordpress.org/plugins/product-import-export-for-woo/) ?

1. `commande`
   1. ⏳(Cédric) 📝 Documenter la BDD actuelle
      1. ✅ Base en place, en attente de complétion / validation
2. `article`
   1. ⏳(Cédric) 📝 Documenter la BDD actuelle
      1. ✅ Base en place, en attente de complétion / validation
