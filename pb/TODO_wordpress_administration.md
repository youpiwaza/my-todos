# TODO / WordPress > Administration

Reste à faire concernant les plugins, le confort de gestion PB

## Réception des commandes

1. Faire ressortir le différentiel entre le nombre de produits en stocks, ainsi que la nouvelle quantité de stocks, afin d'imprimer le bon nombre d'étiquettes (pour les nouveaux produits)
2. Affichage automatique des produits dont la commande a été passée avec l'état "en réapprovisionnement" afin de pouvoir honorer la fin de commande des la reception
   1. Avec impression auto également, mais avec nom client et n° commande en plus
   2. Faire un test de parcours utilisateur qui passe une commande avec un produit en reapprovisionnement, puis maj le stock et voir comment cela marche + impriessions ecrans et retours Cédric

### Générer Code barre PB

Revoir avec Cédric > Plugin payant ?

1. Gérer la gestion des codes barres (c'est un tout)
   1. Flux d'entrée : à la main
   2. **Plugin "réception de marchandise"**
      1. ATUM ?
   3. [Exemple PB](https://pb-modelisme.com/bakofice/btest.php)
      1. Changement de quantité > Génère des codes barres (étiquettes produits)

### Mise à jour des tarifs

Mise à jour des tarifs : prix d’achat et prix de vente public, via plugin (bulk edit)

---

## Page Marques

Possibilité d'affichage front conditionnel, toutes les marques "attention", ~chinoiseries

## Page reliquats clients

Afficher les produits qui n'était pas en stock lors de la commande (produits en attente, permet de vérifier lors de la réception d'une commande).

1. Créer un nouveau statut de commande "Article/s en attente"
2. Commande partiellement honorée (produit pas en stock en attente, articles sur commande uniquement, problème stock)

## Gestion de la page cookies

🐛 Plugin cookies (compmlianz KO 01/2023)

## Repasse sur les pages admin

Avec Cédric (mise en forme des champs persos)

---

## WooCommerce

### Configuration de la TVA

À faire par PB mais je reste la en soutien

### Gestion des moyens de paiements

En attente de retours PB

1. Moyens classiques > codes sandox
2. Caise/espèces > Choix d'un logiciel

Paypal, carte bleue (CIC), virements, chèques, espèces, divers (chèques cadeaux, juste pour la caisse)

---

## Comptes clients "Détaillants"

1. Affichage d’une grille tarifaire pro
2. Possibilité de virer la TVA, ou d'appliquer des réductions globales ou par produit en fonction du rôle. A voir comment sont déterminées les réductions ?

Déjà fait :

1. ✅ Ajout de rôle via un plugin
2. ✅ Ajout de plugin (ELEX) de la possibilité de rajouter des réductions globales (fixes ou %) ou par porduit
3. ✅ Voir dans thème enfant/config > Possibilité de fine tuning
4. à configurer par PB

## Gestion des transports

yup

---

## SAV

yup

---

## Done

### ✅ Done / Gérer le spam

- ✅ Activation du plugin akismet
- ✅ En attente de retour de Cédric
