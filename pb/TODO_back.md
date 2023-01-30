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

1. Onglets supplémentaires
    1. Avions
       1. Pièces détachées / Plan
          1. ✅🧠 Logique
             1. 🔗 Lien avec la table accessoires
                1. `accessoires.REFLIENACC LIKE % avions.REFAVION %`
                2. `REFLIENACC` peut contenir une ou plusieurs entrées ~
                   1. 54209
                   2. ,214211,
                   3. ,214211,PB8100,PB8000,HRR503,HRR504,HRR508,HRR510,HRR505
                   4. NULL
       2. Articles conseillés
          1. Contenu > Lien avec la table accessoires ?
    2. Bateaux
       1. Pièces détachées
          1. Contenu `REFLIENACC`
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
          1. Contenu `REFLIENACC`
       2. Accessoires conseillés > Requête à récupérer / convertir
          1. Contenu > Même requête que Controleurs > Produits compatibles
    6. Helicos
       1. Piéces détachées > Requête à récupérer / convertir > `site actuel pb modelisme\Helico\prodassoc.php` > lol nope
          1. Contenu
       2. Piéces Upgrade > Requête complexe > idem
          1. Contenu
    7. Maquettes
       1. Produits de finitions > Récupérer requête complexe (plusieurs catégories)
          1. Contenu
             1. `site actuel pb modelisme/Maquette/detailprod.php?shw=4`
                1. `site actuel pb modelisme/Maquette/prodassoc.php` > `switch case '4'`
                2. Même requête que Helicos > Piéces détachées en plus complexe
    8. Matériaux
        1. Colles conseillées > Requête complexe en fonction de la sous catégorie
           1. Contenu
    9. Moteurs thermique
        1. Piéces détachées > Requête complexe table constitue ?
           1. Contenu > Le mieux serait de créer un champ avec les ref concaténées
    10. Pièces hélicoptères
        1. Machines compatibles > 🔗 Table "compose"
           1. Contenu
    11. Pièces voitures
        1. ? > 🔗 Table "construite"
           1. Contenu
    12. Recepteurs
        1. Utilisation conseillée/s > 🔗 table "categorieavion", 🔗 table "utilise"
           1. Contenu
        2. Produits compatibles
           1. Contenu
    13. Servos
        1. Piéces détachées
           1. Contenu
    14. Voitures
        1. Pièces détachées > Récupérer requête ancien site
           1. Contenu
        2. Pièces Options > Pieces voitures avec champs OPT à 2 (pièces pour upgrade)
           1. Note max : Ref à la catégorie pièces détachées pour voitures
           2. Contenu

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

1. 🚀 Import des commandes
   1. ✅ 🔍 R&D&T
      1. ✅ Créer 2 commandes de test
         1. ✅ 1 seul article
         2. ✅ Articles multiples
      2. 📌 Trouver un plugin
         1. ✅ Tester export
            1. ✅ Commande ok
            2. ✅ Produits ok
            3. 💸 Champs persos ok / version payante / 129$ / an
         2. ✅ Tester import
         3. ✅ Linter export champs complexes
         4. ✅📌 Tester les options d'import
            1. ✅ Produits sans id wordpress > via SKU
            2. ✅ Utilisateur sans id wordpress > via mail/nom ? mais osef ça marche
         5. ✅ Maj doc structure
            1. ✅ Se servir de l'export articles multiples, du csv d'exemple, des champs complexes éclatés
            2. ✅ Documenter les champs du plugin
               1. [Plugin](https://www.webtoffee.com/category/documentation/order-import-export-plugin-for-woocommerce/)
               2. [Import > Filter datas](https://www.webtoffee.com/export-woocommerce-order-coupons/#Step_3_Fil_3)
                  1. Ptet aider si batch
               3. ✅ `/_docs/craft-and-tests/22-wc-import-commandes/Liste-des-champs-a-l-import.md`
                  1. ✅ Rajouter les champs lors de l'export par cols & rows
            3. ✅ Maj doc structure > Correspondances Legacy/WC
         6. ✅ Discriminer champs WC de champs persos
   2. 🚀 Création de la requête
      1. ✅📧 Mail demande d'infos
         1. Pas mal de champs ambigus pour moi (je suis pas dans la vente/livraison), notamment sur les taxes/réductions/frais/frais expédition, etc.
            1. Besoin de repasser sur la doc Structure > onglets commande & article
            2. Et comparer avec les tableaux de `/22-wc-import-commandes/Liste-des-champs-a-l-import.md`
         2. `commande`.`ETATCMD` différence entre "Livr" & "Livrée"
         3. `commande`.`ETATCMD` différence entre "Livrée" & "Reçue"
         4. `commande`.`ETATCMD` > Certains états ne correspondent pas aux champs par défaut WC, on fait des status personnalisés ?
            1. "dispo en magasin"
            2. "Livr"
         5. `commande`.`PORTCMD` (Expédition > Total de l'envoi) peut être négatif ou NULL ou 0.01 ?
         6. WC > `Expédition > Total de la taxe sur l'envoi`
            1. Y a t-il une taxe à calculer sur l'envoi ? Ex: C'est en TTC et il faut faire ressortir la TVA ?
            2. Sur `commande`.`PORTCMD` TTC ?
         7. WC > Commande > Devise. L'intégralité des transactions sont-elles en euros ?
         8. `commande`.`TYPEPAIMENTCMD` > Pas sûr que l'on puisse indiquer plusieurs méthodes de paiement pour une seule commande sur WC...
         9. `commande`.`PORTCMD` & `TYPELIVRAISON` > Parfois il y a des frais de livraison sans transporteurs, parfois des transporteurs sans frais de livraison...
         10. Table `pays` > Il manque le `CDPAYS` 201
   3. 📌 Tests
   4. Validation PB
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
