# Taf en cours

Légende :

- 🚀  En cours / **1 MAX A LA FOIS**
- ✅  Terminé
- ⏩  Suite
- 🚧  WIP / Work In Progress / Entamé, pas terminé
- 📌  A tester
- 🔍  Lecture/Vidéos
- 🌱  Plus tard, besoin dépendance ou flemme sur le coup
- ♻️  Récurrent
- 🚚  Contenus/notes dans les autres fichiers TODO
- 💩  KO
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

1. Changer filtre caisse chatte
2. Chatte > carnet santé en ligne
3. Boursorama > appeler pour compte pougnoutte + rachat crédit immo
4. Renouveler SNCF [carte liberté](https://mail.google.com/mail/u/0/#inbox/FMfcgzGpGTHLtBRvZFhznpZbcwdGBzTg) ?
5. Chatte disparue > passer à la boulangerie enlever l'avis de recherche
6. 🚀 [Skald](https://mail.google.com/mail/u/0/#inbox/FMfcgzGllVqqnCLcTDzRlDQTwnhlHFdM). A refourguer a mes parents
7. ⏳ Renouveler permis de conduire
   1. ⏳ En attente de retour ~15/07/22
8. Chatte > collier gps + gravé n° de téléphone
9. Orga anniv pougnoutte
    1. Redemander date a pougnoutte
    2. Demander contact & liste invités
    3. Demander si logement déjà vu
    4. Voir pour cagnotte permis moto
    5. Medieval tents
10. Fête fin juin/début juillet ?
    1. Potes HF
    2. Margot & Ryan
    3. Thelma
    4. etc.

Taf

NDD

1. ⏳ ALD
   1. ✅ Facture NDD
   2. ⏳ Paiement

PB Modelisme

1. 🌱⏳ Améliorations WP classiques
   1. ⏳🔒️ Attente https
   2. Vérifier Erreurs console ? Ressources dans wp-include/ en 404 > Besoin https
   3. WP admin > Santé du site
2. 🌱 local > dev > Dupliquer la BDD grâce à modification de l'adresse dans wp-config ?? yay
   1. [doc offi](https://fr.wordpress.org/support/article/running-a-development-copy-of-wordpress/#modifier-ladresse-du-site)
3. ✅ Hebergement > host `www/` > Rajouter un .htaccess deny all
4. ✅ Passage DNS de masa vers dev.pb
   1. ✅ Virer sous domaine masamune
   2. ✅ Virer pb > multisite > masa
5. ✅ Analyse de la structure de BDD WP + WooCommerce
   1. 💩 Faire des diffs
      1. ✅ Ajout d'un produit
      2. ✅ Ajout d'une [catégorie](https://fr.wordpress.org/support/article/taxonomies/)
      3. ✅ Ajout d'une sous catégorie
      4. 💩 Pas mal de trucs à côté de modifier, **besoin** de passer par import régulier, pas de sql à l'arrache
         1. 🔍 Plugin classique (+ manip dev pour champs persos) ou plugin payant
6. ✅🧠💥 Remise au propre des objectifs à court terme
7. ✅📌 Tests d'imports [plugin officiel](https://woocommerce.com/document/product-csv-importer-exporter/)
   1. ✅ Tester l'export de produits
   2. ✅ Tester l'import de produits
   3. ✅ Tester la mise à jour de produits
   4. ✅ Tester l'import avec colonnes custom [plugin officiel > github](https://github.com/woocommerce/woocommerce/wiki/Product-CSV-Importer-&-Exporter#adding-custom-import-columns-developers)
8. 📌 ACF
   1. 🔍 Voir ou ça en est
   2. Export
   3. Import
   4. Mise à jour

Arrêter dev serveur & hebergement > Week end SEULEMENT

1. Migrer clients
   1. Ancien serveur
      1. Identifiants
         1. ftp > Enregistré dans winscp
         2. [mysql](http://94.23.208.218/phpMyAdmin-NEW/) > Enregistré dans dashlane
      2. masamune
         1. blog--masamune--fr
            1. Repartir d'une base propre WP et récupérer/convertir les trucs 1 par 1
         2. 💩 masamune--fr
            1. Repartir d'une base propre WP et récupérer/convertir les trucs 1 par 1
               1. ✅ Articles & pages récupérés
               2. 🚨 Infos dans ACF
               3. 🚨 Remplacer toutes les conneries des plugins
               4. 🚨 Dossier alakon /wp-content/gallery > Contient des images pour le folio
                  1. Voir si il n'y avait pas un dossier ou un repo git contenant tout le folio
         3. ✅ stockage
            1. ✅ Trier
            2. ✅ Uploader
            3. ✅ Vérifier
            4. ✅ Protéger accès racine
      3. MLecuyer
         1. Fixer une date pour faire la bascule (besoin accès SMS)
         2. Faire évoluer hébergement déjà pris par ML
         3. Identifiants dans secrets
         4. Uploader base wordpress
         5. Recup wp-config
         6. Réinstallation wp
         7. Maj identifiants
         8. Injecter anciens fichiers
         9. Injecter ancienne bdd
         10. Maj permaliens
         11. Mises à jour
2. Ranger merdier dans /dev/current
   1. Sur disque dur externe
3. 📌⏳ Tests clients
   1. ⏳ ALD infographie
      1. ✅ Relance clients : bascule auto si pas de news
      2. Basculer DNS
      3. Remettre HTTPS
   2. ⏳ Champagne didier lapie
      1. ✅ Relance clients : bascule auto si pas de news
      2. Basculer DNS
      3. Remettre HTTPS
      4. Réactiver paiement, crédit agricole
   3. ⏳ Sophie berberian
      1. ✅ Relance clients : bascule auto si pas de news
      2. BAYDOT
         1. Basculer DNS
         2. Remettre HTTPS
4. Envoyer identifiants clients + passations
   1. champagne pascal picard
5. Remettre tous les anciens trucs max dans un seul dossier sur un seul dd (~bureau ancien pc)
6. Cleaner google drive
7. Résilier les deux serveurs ? ou garder likorne > Bare metal Nginx pour wam ?

Environnement de dev local clean

1. Gestion de containers via portainer (actuellement en extension sur docker desktop)

### Sinon, priorisation classique

1. Tâches récurrentes
2. Tâches en attente
3. Tâches critiques
4. Tâches rapides
5. Tâches WIP
6. Autres fichiers TODO classiques (Taf > AE > Perso)

## ♻️ Tâches récurrentes ♻️

Tâches à *vérifier au moins une fois par semaine*, afin d'éviter un bordel plus tard/exponentiel

- ✅ Déplacer les terminés ✅ à chaque début de semaine dans done.md
- 💩 Déplacer les TODO 🌱 dans _TODO_shame.md
- ✅ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur ✅ mails, ✅ edt portable, ✅ favoris, ✅ bureau. Si possible description + lien.
- ✅ Nettoyer le fichier __TODO
  - ✅ Status
  - ✅💥 Ce fichier > ### Shame 💥 Cleaner pour vrai les trucs ou je ne passe jamais
    - ✅ Ranger dans fichiers TODO correspondant
      - ✅ Prioriser
- ✅ Virer ce qui traine
  - ✅ sur le bureau
  - 💩 dans le dossier _shame du bureau
  - 💩 Lel ~(local)/_dev/_shame
  - ✅ Vider corbeille
  - ✅ Vider téléchargements
  - ✅ Dans les mails
- ✅ Déplacer veille onglets dans TODO_veille
- 💩 Ranger DD boulot
- 💩 Lel Veille / Un truc par semaine, genre le vendredi aprem, a githuber
- ⏳ Déclaration Auto entrepreneur
  - ⏳ Juin 2022
- ⏳ Vérifier impôts sur espace / Dernière vérif 15/08/2021
  - ⏳ Perso  / ⏳ 23/05/22
  - ⏳ Pro    / ⏳ 23/05/22 (CFE réglé le 17/11/2021)
- ⏳ Vérifier messages [Ameli](https://assure.ameli.fr/)
- ⏳ Maj locales / Environnement de dev / Dernière maj le 01/06/21
  - ⏩ CHKDSK / Besoin de param `/f` ou [ne répare pas](https://docs.microsoft.com/fr-fr/windows-server/administration/windows-commands/chkdsk), `/r` également
    1. Invite de commande ou Powershell **en admin**
    2. `chkdsk c: /f /r` (et en fonction de vos disques.. && `chkdsk d: /f /r`, etc.)
    3. `>Blah blah besoin de redémarrer O/n` >> `O`
    4. Redémarrer / Attendre 5 ans et demi sauf si t'as un SSD/Nvme
  - ✅ Windaube
    - ✅ Update alakon
    - ⏳ [.net](https://dotnet.microsoft.com/download) > Runtime
    - ✅ Panneau de conf > "Fichiers temporaires" > "Fichiers temporaires" (dans les catégories) > Supprimer
  - ✅ Drivers > [detection auto](https://www.touslesdrivers.com/index.php?v_page=29) > Lancer éxécutable, ça ouvre une page recap, et suivre liens dl
  - ⏳ Firmware SSDs / Dépend du constructeur > Voir site officiel, avec un peu de chance logiciel auto alakon
    - ⏳ Dell support assist
    - ⏳ Alienware update
  - ⏳ Docker desktop (tray > icône > RC > Check for updates) / Attention, besoin de redémarrer a la main pour installation
  - ✅ Logiciels alakon
    - ✅ Ouvrir VScode > Auto update plugins etc.
    - ~~Filezilla~~ ✅ WinSCP, ✅ OBS, ✅ VLC, [Xnview classic (Pas MP)](https://www.xnview.com/fr/xnview/#downloads)
    - ~~Powershell~~ Pris en compte par Windows update
      - [sans prise de tête](https://aka.ms/powershell-release?tag=stable) > ~`PowerShell-VERSION-win-x64.msi`.
      - ( [Doc](https://docs.microsoft.com/fr-fr/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-7.1) )
    - ✅ Nvidia driver
  - ✅ Supprimer les fichiers temporaires
    - Exec > `temp` // Devrait ouvrir `~c:Windows\Temp`
    - Supprimer tout, Ignorer ceux utilisés
  - ✅ WSL 2
    - Version Ubuntu
      - Si majeure, ré-effectuer [install-dev-env](https://github.com/youpiwaza/install-dev-env)
    - Packages & terminal

```bash
omz update
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade && sudo apt -y autoremove && docker system prune -af
```

- 🤡 Maj budget couple
- ✅ Téléphone
  - ✅ Maj de la base
  - ✅ Maj des applications
  - ⏳ Tous les 6 mois > reset usine
- ✅ Compléments alimentaires
  - ✅ Anaca3
    - ✅ Attente livraison
    - ♻️ Renouvelement auto 1 fois/mois amazon
  - ✅ Huile de foie de morue
  - ✅ Choline Inositol
  - ✅ Trucs foie/reins
  - ✅ Ginseng / "Super ginko"
  - ✅ Mix vitamine
  - ✅ Doc > vitamine D tous les 6 mois
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

### Trucs **persos**

1. Concert [BFMV & Jinjer](https://www.songkick.com/concerts/40452239-bullet-for-my-valentine-at-lolympia)
2. Concert sum41 & simple plan 20/07/22 Paris bercy ? [hey](https://www.seetickets.com/fr/tr/event/sum-41-simple-plan/accor-arena/8818007)
3. Résilier ESET (besoin de contacter le support ?)
4. Trouver logiciel budget couple
5. 🚀 Musiques taf & portable
6. Blog groupe metal que j'aime bieng ou pas en concert
7. Films
   1. Ciné
      1. Nick cage
      2. Everything everywhere all at once
   2. death of dick long
8. Export photos tel & maj drive
9. Peinture Chtulu
    1. [How to paint Extreme Light Sources - OSL tutorial](https://www.youtube.com/watch?v=c48UiPSBfcg)
    2. [INDESTRUCTIBLE Gaming Bases - Quick & Easy](https://www.youtube.com/watch?v=tRFfsAG-Yf8)
    3. Green gold pour le [grand ancien](https://www.youtube.com/watch?v=AgJqjIMd6k8)
10. [Patinoire](https://mail.google.com/mail/u/0/#inbox/FMfcgzGmvLQjSdlzHqNgpnCFgHjXWZlW)
11. DL vidéos WTF youtoob
12. Faire article mise en place/réparation/optimisation de pc
    1. [hey](https://www.drivereasy.com/knowledge/100-disk-usage-windows-10-fixed/)
    2. [hoy](https://www.makeuseof.com/tips-fix-100-disk-usage-improve-windows-performance/)
13. Faire article maintenance PC
14. Faire article découverte ansible
15. double authentification OVH manager
16. Mettre à jour CV !
17. Rdv médecins
    1. Ophtalmo
    2. Cardiolog0ue
    3. Oreillologiste
18. CPF > Langage des signes / Amazon AWS / Jenkins git hooks
19. !site perso > cours particuliers code > 50€ heure (+, compter impôts)
20. [Boeuf ethique](https://www.leboeufethique.fr/)
21. Portable > reset usine
22. Saut en parachute reims BA prunay

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
