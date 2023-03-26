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
- 📝 Doc
- 📧 email envoyé/à envoyer
- ✨ Rien à toucher, déjà en place

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

1. ~💩 Cleaner TODO en vrai
2. ✅ Prio Evogue
3. 🌱 Evogue > Préparer cours JS
4. 🚀 Clôturer PB (Folio)
5. Déplacer Blog
6. Margot > site https

---

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
- ⏳ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur ⏳ mails, ⏳ edt portable, ⏳ favoris, ⏳ bureau. Si possible description + lien.
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
- ⏳ Vérifier impôts sur espace / Dernière vérif 15/08/2021
  - ⏳ Perso  / ⏳ 19/09/22
  - ⏳ Pro    / ⏳ 19/09/22 (CFE réglé le 17/11/2021) ~début décembre
    - [nouveau site ?](https://www.autoentrepreneur.urssaf.fr/portail/accueil/sinformer-sur-le-statut/toutes-les-actualites/le-guichet-unique-un-nouveau-ser.html)
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
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade && sudo apt -y clean && sudo apt -y autoremove && docker system prune -af
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
- Dashlane > Surveillance dark web > changer mots de passe

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

### 🚀 Evogue

1. ✅ Créer dossierS client dans drive
   1. ✅ Informations entreprise
2. ✅ Signature 2 contrats + ✅ drive
3. ✅ Mission fin mars 2023
   1. ⏳ Gestion transports
      1. ✅ Validation > Call Darren du 22/03/2023
         1. ✅📝 Prévisions
            1. TGV > ~90€
            2. Metro > recharge semaine 30€
            3. Note : sur contrat "Frais remboursable : Non" > Le TJM est à la base de 180€, ajusté à 211.30€ afin de couvrir les frais
      2. ⏳ Réserver
         1. ✅ TGV > 42€
         2. ⏳ Métro > à faire
      3. ⏳ Envoi factures
         1. ✅ TGV
         2. ⏳ Métro
   2. ✅ Ajout précis à l'emploi du temps
   3. ✅ Préparation ressources
      1. ✅ Cleaner boilerplates 📝 Slides sur drive, codes sur github, pas de doublons
         1. ✅ BP présentation
         2. ✅ Présentation max
         3. ✅ Packs débutants
            1. ✅ Boilerplate
            2. ✅ PHP
               1. ✅ renvoyer htdocs vers github
      2. ✨ Présentation (bp)
      3. ✅ Cours
         1. ✅ Plan (+ annonce pré-requis PHP/SQL/phpMyAdmin deja installés)
            1. ✅ PHP
            2. ✅ phpMyAdmin
            3. ✅ SQL
            4. ✨ Communication php > sql // Que du code
         2. ✅ TP / Codes finaux
            1. ✅ PHP
            2. ✅ phpMyAdmin
            3. ✅ SQL
            4. ✅ Communication php > sql
      4. ✅ Vérifier sommaires des presentation
   4. ✅👪 Visio 23/03/23 à 17h voir si tout est ok
   5. ✅ Archives pour BP & corrections & envoi sur stockage masamune
   6. ✅ Tinyurl du dossier drive présentations + ajout dans presentation
   7. ✅ Les présentations contiennent l'ensemble des liens utiles
      1. ✅ Faire une présentation pour les corrections > Dossier pas public
   8. ✅ Facture
      1. ✅ Editée
      2. ✅ Envoyée
      3. ✅ Maj Paiement & impôts
4. Mission Fin avril debut mai 2023
   1. ✨ Pas de transport, en visio
   2. Ajout précis à l'emploi du temps
   3. Préparation ressources
      1. ✨ Présentation (bp)
      2. ✅ Packs débutants
            1. ✅ JS
      3. Cours
         1. Pré-requis
         2. Plans
         3. Exos
      4. Corrections
         1. Exos
         2. Faire une présentation pour les corrections > Dossier pas public
      5. Vérifier sommaires des presentation
      6. Archives pour BP & corrections & envoi sur stockage masamune
      7. Les présentations contiennent l'ensemble des liens utiles
      8. Tinyurl du dossier drive présentations + ajout dans presentation
   4. Facture
      1. Editée
      2. Envoyée
      3. Maj Paiement & impôts

---

## 💩 Shame

Parfois, l'entropie.

Emplois du temps stockés sur mail, portable, favoris, bureau.

Extraire ici puis ranger & prioriser. Doit rester vide.

---

### 🔥 PB Modelisme

1. 💾 Backup + folio
   1. Faire des screens du site
   2. Faire des screens du code + stats
   3. Faire des screens de la documentation crée
   4. Contenus textes du folio
   5. Dump code, pas besoin de la BDD osef
      1. Sauvegarde HDD
2. 🔥 Benner
   1. Résilier serveur
3. ⏳🏥 AFE
      2. ⏳ Commission dans ~1 mois
4. ⏳🏥 Demande de RDV à l'URSSAF de Reims
   1. ✅ Faite le 17/03/2023
   2. ⏳ En attente de retour
5. Demande de remboursement des impots à l'URSSAF, suite au remboursement PB
   2. ✅ Message via urssaf avec détails nouvelles déclarations le 20/03/2023
   3. ⏳ En attente de retour & remboursements
   4. Maj [Paiements AE](https://docs.google.com/spreadsheets/d/1A_TqOQnmzq6xWCgo1wQAJDJZJHzmXre_WNpPy23vIQ4/edit#gid=1999333802)
   5. Maj impots sur le revenu 2022

---

### Auto entrepreneur

Administratif, etc.

1. Mise à jour devis
   1. Ajouter clause devis possibilité évolution de tarifs si sous estimation
   2. En cas d'arrêt des travaux / litige > remboursement de l'hébergement avancé
2. 🌱 Payer impôts CFE rattrapage 2020
   1. Avis en mai 2023, 473€, [à payer en juin](https://mail.google.com/mail/u/0/#inbox/KtbxLvhVcWmcxbbZhnsRMnQSnbSMnkJCGq)

---

### Masamune 2

Branding, CV & sites

1. CV > `/cv-portfolio-tout`
   1. Rajouter le liens vers les [tests techniques](https://github.com/youpiwaza/tests-techniques/)
   2. Regrouper l'ensemble des textes
   3. Sauvegarde github
   4. Sauvegarde sur DD sites web
2. 🚀 blog.masamune.fr
   1. Copie des articles ~10/62 -- Certains vont sauter donc osef
   2. Vérifier galeries > lien vers fichier média
   3. ✅ Faire une repasse sur les commentaires
   4. Vérifier les liens des articles
   5. Rapatrier les medias (zip boilerplates)
      1. Migrer liens vers https / github
      2. [Débrander](http://blog.masamune.fr/jcQpjm9NxDpQydRi/wp-admin/post.php?post=1162&action=edit)
   6. Pages de base
      1. Expliquer refonte
         1. Moins de temps donc plus d'articles et plus regulier
         2. 404
         3. Voir si on conserve certaines anciennes pages
      2. Pages secondaires > renvoi vers masa.fr RGPD blah
   7. [Ajuster templates](https://blog-new.masamune.fr/wp-admin/site-editor.php?postType=wp_template)
   8. Plugins alakon ?
      1. Speed
   9. Fin
      1. Vérifier https
      2. Réindexer site
      3. robots.txt
      4. sitemap
      5. Mise en cache
3. masamune.fr > prod-old
   1. Sauvegarde github
   2. Sauvegarde sur DD sites web
   3. 🌱 Maj liens cv expériences pro
      1. Pas oublier le https
   4. Yootoob > Ajouter écrans de fin / liens vers le site masamune.fr une fois terminé
   5. Service > Retour sur CV > 50€
4. ⚡️💸 Résilier ancien serveur
5. github > cleaner
   1. Renommer préfixer technos
   2. Voir faire un projet liste de liens vers les projets regroupés en catégories
   3. dédoublonner default-config-files-for-github-repository & base-repository-github
   4. Repo dédié checklist fin de site
      1. [Base](https://docs.google.com/spreadsheets/d/1RHnaEn4WmYvjrAjmFAq8tfbINpSEE5XwtTZ3cJkn88g/edit?usp=share_link)
6. Inscription EAN
   1. Inscription [crème de la crème](https://mail.google.com/mail/u/0/#inbox/FMfcgzGqQmNcddHDMfMMGTKJmgzNsvbd)
   2. Inscription Jean-Paul.io
   3. [odoo](https://www.odoo.com/fr_FR/jobs)
   4. [capgemini](https://www.linkedin.com/safety/go?url=https%3A%2F%2Ffr.capgemini.talentnet.community%2F&trk=flagship-messaging-web&messageThreadUrn=urn%3Ali%3AmessagingThread%3A2-MjdmZGZlYjgtZjIxNy00ZDM0LTg2ODYtMzIyYzMwNzcxMzUzXzAxMg%3D%3D&lipi=urn%3Ali%3Apage%3Amessaging_thread%3B984fd009-b4db-44e3-b159-e504a3614444)
7. [Malt PER](https://resources.malt.com/fr/freelances/articles-freelance/reduction-dimpots-avez-vous-pense-a-cette-solution/)

---

### Perso dev

1. 💥 Maj > Installation de l'environnement de dev
   1. Update to latest [Node.js](https://nodejs.org/en/) pour windows
   2. Update to latest [Node.js](https://nodejs.org/en/) pour WSL
      1. [Doc](https://learn.microsoft.com/fr-fr/windows/dev-environment/javascript/nodejs-on-wsl)
      2. Installer curl si besoin
      3. Installer nvm
         1. `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/master/install.sh | bash`
         2. Fermer et relancer terminal
         3. Test `command -v nvm` > Doit renvoyer "nvm"
      4. Installer / Maj Node
         1. `nvm install node`
         2. Tester `node -v`
   3. Majs globales
      1. `sudo apt update`
      2. `sudo apt --fix-broken install`
         1. Si KO réinstaller package
         2. `sudo apt remove PACKAGE`
         3. Eventuellement `sudo apt install PACKAGE`
         4. `sudo apt update && sudo apt upgrade`
         5. `sudo apt --fix-broken install`
         6. `sudo apt -y clean && sudo apt -y autoremove`
         7. Fermer et relancer terminal
         8. ♻️ Recommencer 2-3 fois parce que linux
      3. `sudo apt upgrade`
   4. WSL > Installer npm / yarn / gulp **en global**
      1. `sudo apt install npm`
      2. `sudo apt install yarn`
      3. `sudo apt install gulp`
2. Environnement de dev local > [Move Mountains With Next.js and Compose](https://www.youtube.com/watch?v=-iaLmOGZuD4)

---

### Perso perso

1. Appli radiateurs et config
2. ♻️ Acheter flotte > magnésium
3. MSG maison
    1. [Recette](https://www.youtube.com/watch?v=sE3dYCphy2M)
4. 🔍 Régime
    1. PORK PANKO low carb !
    2. [Low carb](https://www.dietdoctor.com/low-carb) / keto
       1. Most fruits and fruit juice / **Although low-sugar berries — such as blackberries, raspberries, and strawberries — are ok in small to moderate amounts.**
    3. Keto wheat flour > farine avec prot ? [hey](https://www.youtube.com/watch?v=g2fTYDftlCg)
    4. Non fat ricotta cheese / provolone cheese
5. gochujang
    1. [amazon](https://www.amazon.fr/s?k=gochujang+jebiwon)
    2. [idem](https://www.amazon.fr/s?k=doenjang)
6. 🔍 Champignon Lingzhi contre la fatigue & insomnie > Y'en a à grand frais !
7. [Figs Claymore](https://figurama-collectors.com/collections/claymore/products/claymore-teresa-vs-priscilla-elite-exclusive-statue?variant=38322217484463) si le site fonctionne un putain de jour
8. Réserver saut en parachute
9. 🌱 Orga anniv pougnoutte mars 2023
    1. Idées cadeaux
       1. Vélo, a voir en revenant de vacances
       2. Robe style médiéval, demander à Mélanie
       3. Machine pour frapper sa propre monnaie (étain), initiales VL (Vigi & Lucifer)
       4. Bouclier armoiries normandie viking (VL)
       5. Machine à coudre
    2. Redemander date a pougnoutte > mars...
    3. Demander contact & liste invités
    4. Demander si logement déjà vu
    5. Voir pour cagnotte permis moto
    6. Medieval tents
10. [Resto reims](https://www.google.com/maps/place/LA+GRILLADI%C3%88RE+REIMS)
    1. Inviter parents

---

1. Maj tout masamune
   1. 🤏 Virer la merde de _dev/
   2. masamune
      1. clean secrets ids ffs
      2. cv
      3. blog--masamune--fr
         1. Repartir d'une base propre WP et récupérer/convertir les trucs 1 par 1
      4. masamune--fr
         1. Refonte complète du site
            1. Checker image signature gmail
            2. Virer woocommerce & cleaner bdd
            3. Page Contact
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
      5. Github > projet dédié checklist fin de site, à partir de [chaos](https://github.com/youpiwaza/chaos-boilerplate-front)
      6. Remettre tous les anciens trucs max dans un seul dossier sur un seul dd (~bureau ancien pc)
         1. & dossier Bureau/shame
   3. Résilier ancien serveur

---

Déplacer sites clients

1. com--aldinfographie
2. com--champagne-didier-lapie
3. com--sophieberberian
4. com--champagne-pascal-picard
5. com--margot-kasza
   1. Stocké sur ancien so you start !

---

Environnement de dev local clean

1. Gestion de containers via portainer (actuellement en extension sur docker desktop)
2. Tester diff performances etntre images officielles & ubuntu avec reinstallation (ou dockerfile)

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

Slurp [cours 3WA](https://e.3wa.fr/user/profile.php?id=2257)

---

### Trucs persos

1. Musiques taf & portable
2. Blog groupe metal que j'aime bieng ou pas en concert
3. Export photos tel & maj drive
4. Peinture Chtulu
    1. [How to paint Extreme Light Sources - OSL tutorial](https://www.youtube.com/watch?v=c48UiPSBfcg)
    2. [INDESTRUCTIBLE Gaming Bases - Quick & Easy](https://www.youtube.com/watch?v=tRFfsAG-Yf8)
    3. Green gold pour le [grand ancien](https://www.youtube.com/watch?v=AgJqjIMd6k8)

---

Tout est extrait :)

---

### Priorisation

Ordonner puis ranger dans le flux. Doit rester vide.

---

---

Tout est priorisé :)

---
