# TODO / Back

Reste à faire concernant les imports de données depuis l'ancien site

---

## ⏳ Imports restants manuels

Cédric > Produits > Imports manuels > Ne ré-importer que ce qui est visible > Lister les produits ou m'envoyer requête ?

- Faire une requête par catégorie pour faire ressortir les produits à importer.

## ⏳ Contenus complexes ~ onglets

Cédric me renvoie tous les champs normalisés comme liste de peinture

✅📝 Règles d'affichage front pour les champs contenant du nouveau (Relation) & legacy :

- Si il y a des peintures ajoutée via le nouveau champ relation, on n'affiche que elles
- Si il n'y en a pas mais qu'il y a des peintures dans le champ légacy
  - on les affiche
- 🚨 Pas de mix des deux.

---

## 🚀 Import des clients, ainsi que des commandes

Tables concernées "usr", "commande" & "article".

- `usr` contient l'ensemble de nos clients
- `commande` regroupe toutes les infos de la commande ou des ventes magasins (paiement, adresse, n° de colis...)
- `article` contient la référence, l'ID, le numéro de la table dans laquelle l'article ce trouve, les quantités commandé, livrée, le tarif au moment de la commande.... etc

### ⏳ Importer les comptes clients, table `usr`

1. ⏳📌 Recettage Cédric
2. Importer l'ensemble des clients

### Importer l'historique des commandes clients, tables `commande` & `article`

Besoin des articles & des comptes clients

1. Import des commandes
2. Association des commandes aux clients / ventes caisses

Plugin [Product Import Export for WooCommerce](https://wordpress.org/plugins/product-import-export-for-woo/) ?

---

## Done

### ✅ Done / Ajustements Page Un produit

- ✅ Liste de peintures > Virer de la description, onglet uniquement
- ✅ Liste de peintures > Clean affichage conditionnel new / legacy
- ✅ Pièces détachées > passer en onglet + Utiliser l'affichage de "Peintures conseillées"

### Done / Importer les comptes clients, table `usr`

1. ✅📝 (Cédric) Documenter la BDD actuelle
2. ✅ cf. `/_docs/craft-and-tests/21-wc-import-clients/README.md`
3. ✅ Importer les 30 derniers clients

### Done / Importer l'historique des commandes clients, tables `commande` & `article`

1. `commande`
   1. ✅(Cédric) 📝 Documenter la BDD actuelle
      1. ✅ Base en place, en attente de complétion / validation
2. `article`
   1. ✅(Cédric) 📝 Documenter la BDD actuelle
      1. ✅ Base en place, en attente de complétion / validation
