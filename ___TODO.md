# Taf en cours

Légende :

- 🚀 En cours / **1 MAX A LA FOIS**
- ✅ Terminé
- ⏩ Suite
- 🚧 WIP / Work In Progress / Entamé, pas terminé
- 📌 A tester
- 🔍 Lecture/Vidéos
- 🌱 Plus tard, besoin dépendance ou flemme sur le coup
- ♻️ Récurrent
- 🚚 Contenus/notes dans les autres fichiers TODO
- 💩 KO
- ⏳ en attente
- 🤏 Petite partie

## 🧠⏫ Raccourcis & process à intégrer au flow

- Dactylo le midi > [typing study](https://www.typingstudy.com/fr/lesson/3/part/8)
- Tétrachiée de nouveaux plugins VSCode
  - TO DO Tree
  - polacode > joli print de code
- [Toolbox de ouf](https://geekflare.com/tools/toolbox)
- Test plugin wakatime (stats vscode)

## 🚀 Priorisation, simple ⏩

Indiquer ici les *tâches à effectuer en priorité*

- Si besoin de focus, mettre une ou 2 tâches ici.
- Ne pas tout fourrer ici, *respecter la priorisation*, sinon tout est fait à l'arrache

Perso

1. 🔍 Régime
   1. 💥💥💥 PORK PANKO low carb ! 💥💥💥
   2. [Low carb](https://www.dietdoctor.com/low-carb) / keto
      1. Most fruits and fruit juice / **Although low-sugar berries — such as blackberries, raspberries, and strawberries — are ok in small to moderate amounts.**
   3. Keto wheat flour > farine avec prot ? [hey](https://www.youtube.com/watch?v=g2fTYDftlCg)
   4. Non fat ricotta cheese / provolone cheese
2. Voir spectacle chateau sedan pour quand vigi reviendra [hey](https://www.chateau-fort-sedan.fr/evenements)
3. gochujang
   1. [amazon](https://www.amazon.fr/s?k=gochujang+jebiwon)
   2. [idem](https://www.amazon.fr/s?k=doenjang)
4. 🔍 Champignon Lingzhi contre la fatigue & insomnie
5. [Figs Claymore](https://figurama-collectors.com/collections/claymore/products/claymore-teresa-vs-priscilla-elite-exclusive-statue?variant=38322217484463) si le site fonctionne un putain de jour
6. Alan santé > Trouver professionnels autour & prendre RDV
7. 🌱⏳ Cadeau anniv pougnoutte
    1. Vélo, a voir en revenant de vacances
8. Réserver saut en parachute
9. Renouveler SNCF [carte liberté](https://mail.google.com/mail/u/0/#inbox/FMfcgzGpGTHLtBRvZFhznpZbcwdGBzTg)
   1. Carte liberté valable juqu'au 19/10/22
   2. Promo carte 50% en ce moment
10. 🌱 Orga anniv pougnoutte
    1. Redemander date a pougnoutte > mars...
    2. Demander contact & liste invités
    3. Demander si logement déjà vu
    4. Voir pour cagnotte permis moto
    5. Medieval tents

PB Modelisme

1. 👪 RDV client jeudi 01/09/22
    1. ✅ RDV
    2. Cleaner compte rendu
       1. 📧 Envoi
    3. Mail Cédric, intégrer retours, [hey](https://mail.google.com/mail/u/0/#inbox/FMfcgzGqQJrPndBccNvXhJNvglQJpdvg)
    4. Tâches relatives
       1. Installer [WPC Frequently Bought Together for WooCommerce](https://fr.wordpress.org/plugins/woo-bought-together/) / Produits fréquemment achetés ensemble
2. 🚀📌 Finaliser les tests d'import : importer un produit avec l'ensemble des champs
    1. ✅📝 Détails `secrets > /_docs/craft-and-tests/16-tests-imports-finaux_secret/`
    2. 🚀 (Re)mise en place
       1. 🚀 Rétablir champs legacy dernier achat date & prix pour éviter conversion complexe en répéteur ? avec nouveaux champs dispos pour nouveau site
       2. Idem champs requêtes onglets, si besoin de taper dedans (affichage conditionnel > onglet vieux contenu ou onglet données nouveau site)
       3. 🌱 Liste peintures des maquettes > Faire à la main via requête sql `SELECT * FROM maquette WHERE QUANTITEM > 0 AND PAINTLIST IS NOT NULL ORDER BY PAINTLIST DESC` pour savoir lesquelles faires
          1. ET SURTOUT demander a cédric de convertir en références/CDACCESSOIRES ! sinon galères
       4. Rajouter tout ça a l'import
    3. Prix importé en HT
        1. Import OK
        2. Affichage sur site ?
        3. Calcul TTC ok ? arrondi machin mes couilles
    4. 🔍 Réductions en cas de prix réduit pour commande de multiples éléments
       1. Check quantité voir si à la maing ✌️ > Accessoires + de 500
    5. 💥 [Guidelines](https://woocommerce.com/document/product-csv-importer-exporter/#general-guidelines)
       1. Attention pour les **nombres décimaux** : remplacer séparateur "." par virgule ","
          1. 📌 A vérifier, lors de l'export de contrôle les décimaux (pour les **champs classiques de woocommerce**) `"Longueur (mm)"` utilise un point `46.6`
       2. Use 1 or 0 in your CSV, if importing a Boolean value (true or false)
       3. Multiple values in a field get separated with commas.
       4. Wrapping values in quotes allows you to insert a comma.
       5. Prefix the id with id: if referencing an existing product ID. No prefix is needed if referencing an SKU. For example: id:100, SKU101
       6. It is not possible to assign a specific post ID to product on import. Products will always use the next available ID, regardless of the ID included in the imported CSV.
       7. Pas de serialisation dans les données
    6. Import des images produits
        1. [Doc](https://woocommerce.com/document/product-csv-importer-exporter/#images)
    7. 🙊 Sauvegarder tests dans repo secret
    8. 👪 Faire valider
3. Générer Code barre PB ? Revoir avec cedric
4. Affichage front ACF
    1. [Tuto](https://capitainewp.io/formations/acf/champ-relationnel/)
5. Footer > Virer france relance
6. Importer l'ensemble d'une catégorie de produits
    1. Faire valider
7. Autoriser la recherche par SKU/UGS, & par les autres refs
8. 🌱 Importer les anciens comptes clients ?
    1. Besoin des articles
9. 🌱 Importer les commandes
    1. Besoin des articles & des comptes clients
    2. Plugin [Product Import Export for WooCommerce](https://wordpress.org/plugins/product-import-export-for-woo/) ?
       1. The Order Export & Order Import for WooCommerce Add-On is required to export WooCommerce Orders.
10. Plugin de bundle en freemium, [prix pas déconnant](https://wpclever.net/downloads/product-bundles/)
11. Apparence > Personnaliser > WooCommerce (pages profondes & générées automatiquement)
12. 📧 Repasse catégories > Notes pour clients
    1. Il y a énormément de catégorie redondantes / inutiles, ex matériaux > plaques
       1. Ptet voir pour faire une grosse repasse et faire des catégorie générales, avec des taxonomies
          1. Ex: plutôt que "plaque lisse blanche" "plaque lisse noire" "plaque pavage" > plaque avec attributs couleur & texture...
          2. "Tube carré" "Tube rond" >> Tubes > forme
13. Devis > Bouton client, passer à état "commande en cours"
14. Fin de site
    1. ACF > Ranger champs en onglets ptet ? [doc](https://www.advancedcustomfields.com/resources/tab/)
    2. wp-config > DEBUG true > & cleaner un  peu si possible
    3. Liens menus > virer liens persos "#" & remplacer par le bon contenu dynamique
    4. Doc : css custom des menus : Admin wp > quad menu > options > [customize](https://dev.pb-modelisme.com/wp-admin/admin.php?page=quadmenu_options)
    5. Installer plugin wishlist [mais pas celui la (KO)](https://fr.wordpress.org/plugins/woo-smart-wishlist/)

Arrêter dev serveur & hebergement

1. Migrer clients
   1. Ancien serveur
      1. Identifiants
         1. ftp > Enregistré dans winscp
         2. [mysql](http://94.23.208.218/phpMyAdmin-NEW/) > Enregistré dans dashlane
      2. masamune
         1. 🚀 clean secrets ids ffs
         2. blog--masamune--fr
            1. Repartir d'une base propre WP et récupérer/convertir les trucs 1 par 1
         3. masamune--fr
            1. Refonte complète du site
               1. Checker image signature gmail
               2. 🚀 Virer woocommerce & cleaner bdd
               3. 🚀 Page Contact
                  1. Captcha
                  2. Tester formulaire
                  3. SPF DKIM DMARC
               4. Cours particuliers code > 50€ heure (+, compter impôts)
            2. Fin du site
               1. Vérifier toutes les pages (liens, traductions)
               2. Page plan du site
               3. Menus
               4. Mentions légales > Lien page de contact
               5. analyse des cookies + maj RGPD et éventuellement bandeau
         4. Github > projet dédié checklist fin de site, à partir de [chaos](https://github.com/youpiwaza/chaos-boilerplate-front)
      3. Résilier ancien serveur
2. 💥📌 Migration changer propriétaire > mettre dans "domaine" le nom de l'hébergement
   1. Retour support ovh "Veillez à bien inclure votre nom de service "XXX.cluster029.hosting.ovh.net" dans "domaine"."
   2. ⏳ com--aldinfographie
      1. 💩 Vérifier passations NDDs "Déjà en cours de changement de propriétaire"
         1. ⏳ Attente de voir si changement margot ok puis relance
      2. ⏳ Passation hébergement
          4. Passation
             1. Demande + réception PDF
             2. Compléter PDF, need signature à la main
                1. Max
                2. Nonore
             3. Sauvegarder PDFs dans drive
             4. Pièces jointes
                1. Max > Pièce identité
                2. Nonore > Pièce identité
             5. Envoi à suivi-procedure@ovh.net
             6. Validation
   3. ⏳ com--champagne-didier-lapie
      1. 💩 Vérifier passations NDDs "Déjà en cours de changement de propriétaire"
         1. ⏳ Attente de voir si changement margot ok puis relance
      2. ⏳ Passation hébergement
          4. Passation
             1. Demande + réception PDF
             2. Compléter PDF, need signature à la main
                1. Max
                2. Lapie
             3. Sauvegarder PDFs dans drive
             4. Pièces jointes
                1. Max > Pièce identité
                2. Lapie > Pièce identité
             5. Envoi à suivi-procedure@ovh.net
             6. Validation
   4. ⏳ com--sophieberberian
      2. ⏳ Passation hébergement
          3. ⏳ Passation
             1. Demande + réception PDF
             2. Compléter PDF, need signature à la main
                1. Max
                2. Bedot
             3. Sauvegarder PDFs dans drive
             4. Pièces jointes
                1. Max > Pièce identité
                2. Bedot > Pièce identité
             5. Envoi à suivi-procedure@ovh.net
             6. Validation
   5. com--champagne-pascal-picard
      1. 💥💥💥 Faire facture noms de domaines 2022, cf. bureau
      2. ⏳ Passation hébergement
         1. ⏳ Passation
             1. Demande + réception PDF
             2. Compléter PDF, need signature à la main
                1. Max
                2. Bedot
             3. Sauvegarder PDFs dans drive
             4. Pièces jointes
                1. Max > Pièce identité
                2. Bedot > Pièce identité
             5. Envoi à suivi-procedure@ovh.net
             6. Validation
   6. ⏳ MKasza
      1. 💩 Vérifier passations NDDs "Déjà en cours de changement de propriétaire"
      2. 📌 Relance, si ça marche go relancer les autres
3. ⏳ Résilier nouveau serveur
   1. ✅ Demander résiliation
   2. ⏳ Effectif 1er novembre 2022
4. 🤏 Virer la merde de _dev/
5. Remettre tous les anciens trucs max dans un seul dossier sur un seul dd (~bureau ancien pc)
   1. & dossier Bureau/shame
6. Cleaner google drive

Environnement de dev local clean

1. Gestion de containers via portainer (actuellement en extension sur docker desktop)
2. Tester diff performances etntre images officielles & ubuntu avec reinstallation (ou dockerfile)

### Sinon, priorisation classique

1. Tâches récurrentes
2. Tâches en attente
3. Tâches critiques
4. Tâches rapides
5. Tâches WIP
6. Autres fichiers TODO classiques (Taf > AE > Perso)

## ♻️ Tâches récurrentes ♻️

Tâches à *vérifier au moins une fois par semaine*, afin d'éviter un bordel plus tard/exponentiel

- ⏳ Déplacer les terminés ✅ à chaque début de semaine dans done.md
- 💩 Déplacer les TODO 🌱 dans _TODO_shame.md
- ✅ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur ⏳ mails, ⏳ edt portable, ⏳ favoris, ⏳ bureau. Si possible description + lien.
- ⏳ Nettoyer le fichier __TODO
  - ⏳ Status
  - ⏳💥 Ce fichier > ### Shame 💥 Cleaner pour vrai les trucs ou je ne passe jamais
    - ⏳ Ranger dans fichiers TODO correspondant
      - ⏳ Prioriser
- ⏳ Virer ce qui traine
  - ⏳ sur le bureau
  - 💩 dans le dossier _shame du bureau
  - 💩 Lel ~(local)/_dev/_shame
  - ⏳ Vider corbeille
  - ⏳ Vider téléchargements
  - ⏳ Dans les mails
- ⏳ Déplacer veille onglets dans TODO_veille
- 💩 Ranger DD boulot
- 💩 Lel Veille / Un truc par semaine, genre le vendredi aprem, a githuber
- ⏳ Déclaration Auto entrepreneur
  - ⏳ Juin 2022
  - ⏳ Juillet 2022
- ⏳ Vérifier impôts sur espace / Dernière vérif 15/08/2021
  - ✨💥💥💥 Perso  / ✨ 01/08/22
  - ⏳ Pro    / ⏳ 11/07/22 (CFE réglé le 17/11/2021) ~début décembre
- ⏳ Vérifier messages [Ameli](https://assure.ameli.fr/)
- ⏳ Maj locales / Environnement de dev / Dernière maj le 01/06/21
  - ⏳ CHKDSK / Besoin de param `/f` ou [ne répare pas](https://docs.microsoft.com/fr-fr/windows-server/administration/windows-commands/chkdsk), `/r` également
    1. Invite de commande ou Powershell **en admin**
    2. `chkdsk c: /f /r` (et en fonction de vos disques.. && `chkdsk d: /f /r`, etc.)
    3. `>Blah blah besoin de redémarrer O/n` >> `O`
    4. Redémarrer / Attendre 5 ans et demi sauf si t'as un SSD/Nvme
  - ⏳ Windaube
    - ⏳ Update alakon
    - ⏳ [.net](https://dotnet.microsoft.com/download) > Runtime
    - ⏳ Panneau de conf > "Fichiers temporaires" > "Fichiers temporaires" (dans les catégories) > Supprimer
  - ⏳ Drivers > [detection auto](https://www.touslesdrivers.com/index.php?v_page=29) > Lancer éxécutable, ça ouvre une page recap, et suivre liens dl
  - ⏳ Firmware SSDs / Dépend du constructeur > Voir site officiel, avec un peu de chance logiciel auto alakon
    - ⏳ Dell support assist
    - ⏳ Alienware update
  - ⏳ Docker desktop (tray > icône > RC > Check for updates) / Attention, besoin de redémarrer a la main pour installation
  - ⏳ Logiciels alakon
    - ⏳ Ouvrir VScode > Auto update plugins etc.
    - ~~Filezilla~~ ⏳ WinSCP, ⏳ OBS, ⏳ VLC, [Xnview classic (Pas MP)](https://www.xnview.com/fr/xnview/#downloads)
    - ~~Powershell~~ Pris en compte par Windows update
      - [sans prise de tête](https://aka.ms/powershell-release?tag=stable) > ~`PowerShell-VERSION-win-x64.msi`.
      - ( [Doc](https://docs.microsoft.com/fr-fr/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-7.1) )
    - ⏳ Nvidia driver
  - ⏳ Supprimer les fichiers temporaires
    - Exec > `temp` // Devrait ouvrir `~c:Windows\Temp`
    - Supprimer tout, Ignorer ceux utilisés
  - ⏳ WSL 2
    - Version Ubuntu
      - Si majeure, ré-effectuer [install-dev-env](https://github.com/youpiwaza/install-dev-env)
    - Packages & terminal

```bash
omz update
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade && sudo apt -y autoremove && docker system prune -af
```

- ⏳ Téléphone
  - ⏳ Maj de la base
  - ⏳ Maj des applications
  - ⏳ Tous les 6 mois > reset usine
- ⏳ Compléments alimentaires
  - ⏳ Anaca3
    - ⏳ Attente livraison
      - Pas les clés de la BAL lelelelelelelelelel omégadrole putain QU'EST CE QU'ON S'ESCLAFFE
  - ⏳ Huile de foie de morue
  - ⏳ Choline Inositol
  - ⏳ Trucs foie/reins
  - ⏳ Ginseng / "Super ginko"
  - ⏳ Mix vitamine
  - ⏳ Doc > vitamine D tous les 6 mois
  - ⏳ Miel gelée royale
- ⏳ Tout est versionné, pas de WIP qui traîne

---

## ⏳ En attente

Rieng

### ⏳🌱 Vérifications sur la longueur

Rieng

## 💥 Tâches critiques

Bug clients majeurs, interruptions de service, etc.

Rieng

## ⚡️ Tâches rapides ✨

Indiquer ici les *tâches en dehors du flux général* (urgences, corrections process, trucs qui perturbent et doivent être fait, tâches ultra rapides, etc.)

Rieng

## 🚧 WIP 🚧

Si travail en cours, indiquer les *notes & liens* ici

Rieng

## 💼 Taf 💼

### Masamune

1. CPF > Non périssable > ~2k€
2. slurp cours [3wa](https://e.3wa.fr/user/profile.php?id=2257)
3. install-dev-env > docker-compose pour les principales technos : js & phpay
   1. Nginx + conteneur de gestion de conteneurs
4. 🔍 [tmux](https://nickjanetakis.com/blog/who-else-wants-to-boost-their-productivity-with-tmux)
5. 🔍 [keys remap](https://nickjanetakis.com/blog/remap-and-set-global-hotkeys-on-windows-10-with-auto-hotkey)

### Auto-entrepreneur

1. Migration avant 2023 [google analytics 4](https://mail.google.com/mail/u/0/#inbox/FMfcgzGpFWSCZKSSbnBjmgLtgpFfLWxC)
2. Veille
   1. [Arrêt maladie : les démarches du travailleur indépendant](https://www.ameli.fr/assure/droits-demarches/maladie-accident-hospitalisation/arret-travail-maladie/arret-travail-maladie-independants)
   2. 💥 CPF [Prise en charge des formations des travailleurs indépendants](https://entreprendre.service-public.fr/vosdroits/F31148)
   3. [Quand prendre sa retraite ?](https://www.lassuranceretraite.fr/portail-info/home/actif/travailleur-independant/depart-retraite/inde-quand-retraite.html)
3. Référencement AE
   1. [hey](https://www.cominjob.com/candidat/)
   2. [hoy](https://www.ouiboss.com/)
   3. [prout](https://www.freelance-informatique.fr/)
4. Renvoi doc AE décla 0€ années passées [hey](https://mail.google.com/mail/u/0/#inbox/FMfcgxmXKmkCGqSQkpPRbBrSKWcsbCpr)
5. Maj document de base à partir de celui de PB Modelisme
   1. Cdc
   2. Devis
   3. Factures
   4. Statut
   5. Etc.

---

### Trucs persos

1. Changer pass crosoft
2. Concert [Psykup petit bain jeudi 27/10/22 21€](https://mail.google.com/mail/u/0/#inbox/FMfcgzGpGnMjGCklxkVmPzNShRbwJCpr)
3. Concert [BFMV & Jinjer](https://www.songkick.com/concerts/40452239-bullet-for-my-valentine-at-lolympia)
4. Concert sum41 & simple plan 20/07/22 Paris bercy ? [hey](https://www.seetickets.com/fr/tr/event/sum-41-simple-plan/accor-arena/8818007)
5. Trouver logiciel budget couple
6. 🚀 Musiques taf & portable
7. Blog groupe metal que j'aime bieng ou pas en concert
8. Films
    1. Ciné
       1. Nick cage
       2. Everything everywhere all at once
    2. death of dick long
9. Export photos tel & maj drive
10. Peinture Chtulu
    1. [How to paint Extreme Light Sources - OSL tutorial](https://www.youtube.com/watch?v=c48UiPSBfcg)
    2. [INDESTRUCTIBLE Gaming Bases - Quick & Easy](https://www.youtube.com/watch?v=tRFfsAG-Yf8)
    3. Green gold pour le [grand ancien](https://www.youtube.com/watch?v=AgJqjIMd6k8)
11. [Patinoire](https://mail.google.com/mail/u/0/#inbox/FMfcgzGmvLQjSdlzHqNgpnCFgHjXWZlW)
12. DL vidéos WTF youtoob
13. Faire article mise en place/réparation/optimisation de pc
    1. [hey](https://www.drivereasy.com/knowledge/100-disk-usage-windows-10-fixed/)
    2. [hoy](https://www.makeuseof.com/tips-fix-100-disk-usage-improve-windows-performance/)
    3. Faire article optimiser pc famille
       1. DD plein
          1. Reco SSD/Nvme
       2. windows update
       3. Conflits anti virus
       4. Si HDD > Defrag
       5. chkdsk
14. Faire article maintenance PC
15. Faire article découverte ansible
16. double authentification OVH manager
17. Mettre à jour CV !
18. Rdv médecins
    1. Ophtalmo
    2. Cardiolog0ue
    3. Oreillologiste
19. CPF > Langage des signes / Amazon AWS / Jenkins git hooks
20. [Boeuf ethique](https://www.leboeufethique.fr/)
21. Portable > reset usine

## 💩 Shame

Parfois, l'entropie.

Emplois du temps stockés sur mail, portable, favoris, bureau.

Extraire ici puis ranger & prioriser. Doit rester vide.

---

---

Tout est extrait :)

---

### Priorisation

Ordonner puis ranger dans le flux. Doit rester vide.

---

---

Tout est priorisé :)

---
