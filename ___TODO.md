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

1. Orga anniv pougnoutte
   1. Redemander date a pougnoutte
   2. Demander contact & liste invités
   3. Demander si logement déjà vu
   4. Voir pour cagnotte permis moto
   5. Medieval tents

Taf

PB Modelisme

1. ✅ Environnement de dev local
   1. ✅ Crafts n' tests > `pb-modelisme--com/_docs/craft-and-tests/01-craft-docker-compose-file/README.md`
   2. ✅ Création du dossier local & maj de la doc `_docs/local-environnement-setup.md`
      1. ✅🚨 Structure du projet pour insertion sur serveur > `wp-content/` à la racine du projet ?
   3. ✅ Installation persistante > Une fois l'installation de WordPRess terminée via wp-cli
      1. ✅ Populer github avec les fichiers `/wordpress`
      2. ✅ Local > pull
      3. ✅ OVH manager > Sauvegarde BDD
      4. ✅ Populer BDD locale > Installation
      5. ✅ Récupérer identifiants WP de OVH & populer secrets en local
   4. ✅ Ajout de wp-cli
      1. 💩 KO en `docker run`
      2. ✅🔨📌 Ajout au docker-compose
         1. ✅ Test au lancement
         2. ✅ Test des commandes basiques
      3. ✅👌 Mise au propre
         1. ✅ Local DC
            1. ✅ 🐛 Ajuster l'utilisateur
         2. ✅📝 Doc & principales commandes
   5. ✅🐛 Problème lors des mises à jour via admin wordpress (traductions, plugins, etc.)
      1. ✅ wp-config > passer outre les identifiants sftp
      2. ✅ Se connecter au conteneur wp en tant que root & `chown -R www-data:www-data wp-content/`
      3. ✅ FIX & Doc
2. ✅💻 Serveur OVH
   1. ✅ Commandé & livré
   2. ✅🔑 Récupérer les identifiants de base
   3. ✅🔒️ Modifier tous les identifiants de base qui sont quand même vraiment pas sécurisés
   4. ✅🙊 Maj secrets
   5. 💩🐛 Passer en multisite pour site de dev & WordPress 1 clic
      1. KO version de php ou nom d'admin trop long chp + DNS foireux
   6. ✅🔍 [Doc wp-cli](https://wp-cli.org/fr/)
   7. ✅ Installation de [wp-cli](https://make.wordpress.org/cli/handbook/guides/installing/)
   8. ✅ Installation de WordPress [via wp-cli](https://make.wordpress.org/cli/handbook/how-to-install/)
      1. ✅ Site de dev dispo sur [sous domaine masa](https://dev-pb-modelisme.masamune.fr/)
3. ✅⚡️👷 Flux de développement via git afin d'éviter les conflits
4. ⏳ Améliorations WP classiques
   1. ✅ Permaliens
   2. ✅ Virer les plugins inutiles
   3. ✅ Virer les thèmes inutiles
   4. ✅ Mises à jour
   5. ✅ SALT
   6. ✅ Virer `wp-config-sample.php`
   7. ⏳🔒️ Erreurs console ? Ressources dans wp-include/ en 404 > Besoin https
      1. Santé du site
5. 💥💥💥 host `www/` > Rajouter un .htaccess deny all
6. 🚀 Passage DNS de masa vers dev.pb
   1. ✅ OVH Manager > multi-site > Prise en charge du NDD
   2. ✅ Call avec Cédric pour mise en place (entrée supl. vérif possession DNS > TXT)
   3. ⏳ Attente mise en place TXT & tests
7. 💥 local > dev > Dupliquer la BDD grâce à modification de l'adresse dans wp-config ?? yay
   1. [doc offi](https://fr.wordpress.org/support/article/running-a-development-copy-of-wordpress/#modifier-ladresse-du-site)
8. Analyse de la structure de BDD WP + WooCommerce
   1. 🤏✅ MCD WordPress Vanilla
   2. ✅ Installation de woocommerce
   3. 🤏✅ MCD WP WC
   4. ✅ Plutôt comparaison exports SQL pour gain de temps
   5. 🚀 Faire des diffs
      1. Ajout d'un produit
      2. Ajout d'une [catégorie](https://fr.wordpress.org/support/article/taxonomies/)
      3. Ajout d'une sous catégorie

Arrêter dev serveur & hebergement

1. Migrer clients
   1. Ancien serveur    `94.23.208.218`
   2. Nouveau serveur   `188.165.253.170`
   3. [Check ip site](https://geekflare.com/tools/whois-hosting)
   4. Légende, dans l'ordre
      1. 🤔 On conserve ?
      2. 🌱 A faire
      3. 📂 Dump fichier OK
      4. 💾 Dump BDD OK
      5. 📱 Relane par sms
      6. 💻 Serveur commandé OK
      7. ⬆️ Mise en ligne OK
      8. 📌 Test sans DNS OK
      9. 🔗 DNS Migré OK
      10. 📧🔑 Envoi des identifiants
      11. ✅ Terminé
   5. Nouveau serveur > all in 1 wp migration
      1. ✅📂💾 ✅📱 💻⏳ Sophie berberian
         1. À transférer
      2. ✅📂💾 ✅📱 ⏳💻 Champagne didier lapie
         1. En attente de retour mails/sms
      3. ✅📂💾 ✅💻⏳ ALD infographie
         1. À transférer
      4. Si champ & ald KO > Export bdd via migration & gestion des fichiers par `ansible-install-web-server/commandes-backup-volumes-a-la-maing_secret.md`
   6. Ancien serveur
      1. 📧🔑 Heberg picard > Déjà en place sur un hébergement dédié, à cleaner
      2. Identifiants
         1. ftp > Enregistré dans winscp
         2. [mysql](http://94.23.208.218/phpMyAdmin-NEW/) > Enregistré dans dashlane
      3. ✅ Récupérer tout `/home`
         1. et trier
      4. ✅📂💾 ✅📱 Baptiste guerechi
         1. Envoyer dump datas par wetransfer, pas de remise en ligne
      5. ✅📂💾 ✅💻⏳ masamune
         1. ✅📂💾 blog
         2. ✅📂💾 site
      6. ✅📂💾 ✅📱 mkasza
         1. Envoyer dump datas par wetransfer, pas de remise en ligne
      7. ✅📂💾 ✅📱 ⏳💻 MLecuyer
         1. En attente de retour mail/sms
      8. `/mysql` ? Attendre fin récup BDDs
2. Remettre tous les anciens trucs max dans un seul dossier sur un seul dd (~bureau ancien pc)
3. Cleaner google drive
4. Résilier les deux serveurs ? ou garder likorne > Bare metal Nginx pour wam ?

Clôture cryptor

1. ✅ Doc de fin de contrat a signer + signature electronique
   1. ⏳ Signature
2. ✅ Facture
   1. ⏳ Règlement

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
- ⏳ Virer ce qui traine
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
  - ⏳ Mai 2022
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
  - ⏳ Drivers > [detection auto](https://www.touslesdrivers.com/index.php?v_page=29) > Lancer éxécutable, ça ouvre une page recap, et suivre liens dl
  - ✅ Firmware SSDs / Dépend du constructeur > Voir site officiel, avec un peu de chance logiciel auto alakon
    - ✅ Dell support assist
    - ✅ Alienware update
  - ✅ Docker desktop (tray > icône > RC > Check for updates) / Attention, besoin de redémarrer a la main pour installation
  - ✅ Logiciels alakon
    - ✅ Ouvrir VScode > Auto update plugins etc.
    - ~~Filezilla~~ ✅ WinSCP, ✅ OBS, ✅ VLC, ESET, [Xnview classic (Pas MP)](https://www.xnview.com/fr/xnview/#downloads)
    - ⏳ Powershell [sans prise de tête](https://aka.ms/powershell-release?tag=stable) > ~`PowerShell-VERSION-win-x64.msi`.
      - ( [Doc](https://docs.microsoft.com/fr-fr/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-7.1) )
    - ✅ Nvidia driver
  - ✅ Supprimer les fichiers temporaires
    - Exec > `temp` // Devrait ouvrir `~c:Windows\Temp`
    - Supprimer tout, Ignorer ceux utilisés
  - ✅ WSL
    - Version Ubuntu
      - Si majeure, ré-effectuer [install-dev-env](https://github.com/youpiwaza/install-dev-env)
    - Packages & terminal

```bash
omz update
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade && sudo apt -y autoremove && docker system prune -af
```

- ⏳ Maj budget couple
- ⏳ Téléphone
  - ⏳ Maj de la base
  - ⏳ Maj des applications
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
- ✅ Tout est Versionné, pas de WIP qui traîne

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

1. Résilier ESET (besoin de contacter le support ?)
2. Trouver logiciel budget couple
3. 🚀 Musiques taf & portable
4. ✅ concert 10/06 maximum the hormone
      1. 🚀 trains, et utiliser [reductions](https://mail.google.com/mail/u/0/#inbox/KtbxLxgZZVNcfFNSbtrStGMpWXmfCKPsJB)
      2. Prendre un poil plus tôt
5. Blog groupe metal que j'aime bieng ou pas en concert
6. Films
   1. Ciné
      1. Nick cage
      2. Dernier Cronenberg
      3. Everything everywhere all at once
   2. death of dick long
7. Export photos tel & maj drive
8. Peinture Chtulu
    1. [How to paint Extreme Light Sources - OSL tutorial](https://www.youtube.com/watch?v=c48UiPSBfcg)
    2. [INDESTRUCTIBLE Gaming Bases - Quick & Easy](https://www.youtube.com/watch?v=tRFfsAG-Yf8)
    3. Green gold pour le [grand ancien](https://www.youtube.com/watch?v=AgJqjIMd6k8)
9. [Patinoire](https://mail.google.com/mail/u/0/#inbox/FMfcgzGmvLQjSdlzHqNgpnCFgHjXWZlW)
10. Retrouver Permis conduire
11. DL vidéos WTF youtoob
12. [Changement propriétaire chatte](https://mail.google.com/mail/u/0/#inbox/FMfcgzGllCcNJCZHqcjqlkNJhlNFzwZC)
13. Faire article mise en place/réparation/optimisation de pc
    1. [hey](https://www.drivereasy.com/knowledge/100-disk-usage-windows-10-fixed/)
    2. [hoy](https://www.makeuseof.com/tips-fix-100-disk-usage-improve-windows-performance/)
14. Faire article maintenance PC
15. Faire article découverte ansible
16. double authentification OVH manager
17. Mettre à jour CV !
18. Rdv médecins
    1. Ophtalmo
    2. Cardiolog0ue
    3. Oreillologiste
19. CPF > Langage des signes / Amazon AWS / Jenkins git hooks
20. !site perso > cours particuliers code > 50€ heure (+, compter impôts)
21. [Boeuf ethique](https://www.leboeufethique.fr/)
22. Portable > reset usine
23. Saut en parachute reims BA prunay

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
