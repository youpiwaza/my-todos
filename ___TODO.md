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
- 👪 Réunion ou call

## 🧠⏫ Raccourcis & process à intégrer au flow

- 🤯 Plugin VSCode pour WSL
- Dactylo le midi > [typing study](https://www.typingstudy.com/fr/lesson/3/part/8)
- Tétrachiée de nouveaux plugins VSCode
  - TO DO Tree

## 🚀 Priorisation, simple ⏩

Indiquer ici les *tâches à effectuer en priorité*

- Sert de sommaire > Ctrl + F vers détails plus bas
- Si besoin de focus, mettre une ou 2 tâches ici.
- Ne pas tout fourrer ici, *respecter la priorisation*, sinon tout est fait à l'arrache

1. Trier
   1. En premier les trucs éclatables en quelques minutes, virer tt ce qui parasite
   2. Prioriser
      1. Rangement HF
      2. Urgent
      3. Avec dédoublonnage

---

### Sinon, priorisation classique

1. Tâches récurrentes
2. Tâches en attente
3. Tâches critiques
4. Tâches rapides
5. Tâches WIP
6. Tâches Taf, si besoin de séparer par clients
7. Tâches Persos, afin que ça n'empiète pas trop ailleurs
8. Autres fichiers TODO classiques (Taf > AE > Perso)

## ♻️ Tâches récurrentes ♻️

Tâches à *vérifier au moins une fois par semaine*, afin d'éviter un bordel plus tard/exponentiel

- ✅ Déplacer les terminés ✅ à chaque début de semaine dans done.md
- 💩 Déplacer les TODO 🌱 dans _TODO_shame.md
- ✅ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur ✅ mails, ✅ edt portable, ✅ favoris, ✅ bureau. Si possible description + lien.
- ✅ Nettoyer le fichier __TODO
  - ✅ Status
  - ⏳💥 Ce fichier > ### Shame 💥 Cleaner pour vrai les trucs ou je ne passe jamais
    - ⏳ Ranger dans fichiers TODO correspondant
      - ⏳ Prioriser
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
- ⏳ Déclaration Auto entrepreneur / Avril 2023
- ⏳ Vérifier impôts sur espace
  - ⏳ Perso  / Revenus 2022
  - ⏳ Pro    / 11/04/2022
- ⏳ Vérifier messages [Ameli](https://assure.ameli.fr/)
- ⏳ Maj locales / Environnement de dev / Dernière maj le 01/06/21 / lel
  - ⏳ CHKDSK / Besoin de param `/f` ou [ne répare pas](https://docs.microsoft.com/fr-fr/windows-server/administration/windows-commands/chkdsk), `/r` également
    1. Invite de commande ou Powershell **en admin**
    2. `chkdsk c: /f /r` (et en fonction de vos disques.. && `chkdsk d: /f /r`, etc.)
    3. `>Blah blah besoin de redémarrer O/n` >> `O`
    4. Redémarrer / Attendre 5 ans et demi sauf si t'as un SSD/Nvme
  - ⏳ Windaube
    - ✅ Update alakon
    - ⏳ [.net](https://dotnet.microsoft.com/download) > Runtime
    - ⏳ Panneau de conf > "Fichiers temporaires" > "Fichiers temporaires" (dans les catégories) > Supprimer
  - ⏳ Drivers > [detection auto](https://www.touslesdrivers.com/index.php?v_page=29) > Lancer éxécutable, ça ouvre une page recap, et suivre liens dl
  - ⏳ Firmware SSDs / Dépend du constructeur > Voir site officiel, avec un peu de chance logiciel auto alakon
    - ⏳ Dell support assist
    - ⏳ Alienware update
    - ⏳💸 System mechanic
  - ⏳ Docker desktop (tray > icône > RC > Check for updates) / Attention, besoin de redémarrer a la main pour installation
  - ⏳ Logiciels alakon
    - ✅ Ouvrir VScode > Auto update plugins etc.
    - ~~Filezilla~~ ✅ WinSCP, ✅ OBS, ✅ VLC, [Xnview classic (Pas MP)](https://www.xnview.com/fr/xnview/#downloads)
    - ~~Powershell~~ Pris en compte par Windows update
      - [sans prise de tête](https://aka.ms/powershell-release?tag=stable) > ~`PowerShell-VERSION-win-x64.msi`.
      - ( [Doc](https://docs.microsoft.com/fr-fr/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-7.1) )
    - ✅ Nvidia driver
  - ⏳ Supprimer les fichiers temporaires
    - Exec > `temp` // Devrait ouvrir `~c:Windows\Temp`
    - Supprimer tout, Ignorer ceux utilisés
  - ✅ WSL 2
    - Version Ubuntu
      - Si majeure, ré-effectuer [install-dev-env](https://github.com/youpiwaza/install-dev-env)
    - Packages & terminal

```bash
omz update
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade && sudo apt -y clean && sudo apt -y autoremove && docker system prune -af && npm install -g npm@latest
```

- ✅ Téléphone
  - ✅ Maj de la base
  - ✅ Maj des applications
  - ⏳ Tous les 6 mois > reset usine
- ~⏳ Compléments alimentaires
  - ⏳ Anaca3
  - ⏳ Huile de foie de morue
  - ⏳ Choline Inositol
  - ⏳ Trucs foie/reins
  - ⏳ Ginseng / "Super ginko"
  - ⏳ Mix vitamine
  - ⏳ Doc > vitamine D tous les 6 mois
  - ✅ Miel gelée royale
  - ⏳♻️ Acheter flotte > magnésium
- ⏳ Tout est versionné, pas de WIP qui traîne
- ♻️ majs tous les wordpress
- ♻️ Article blog
- Dashlane > Surveillance dark web > changer mots de passe

---

## ⏳ En attente

### Perso

1. ⏳ Relance syndic > clé qui n'ouvre pas le local à poubelle
   1. ⏳ Mail envoyé le 11/04/23 > Vu lors de l'AG > Changement de serrurier ?

---

### ⏳🌱 Vérifications sur la longueur

rieng

---

## 💥 Tâches critiques

Bug clients majeurs, interruptions de service, etc.

Rieng

---

## ⚡️ Tâches rapides ✨

Indiquer ici les *tâches en dehors du flux général* (urgences, corrections process, trucs qui perturbent et doivent être fait, tâches ultra rapides, etc.)

Rieng

---

## 🚧 WIP 🚧

Si travail en cours, indiquer les *notes & liens* ici

Rieng

---

## 💼 Taf 💼

### 💼 Jus Mundi

1. 🎯 Objectifs en gros > Institutions Overview
2. ♻️👌 Clean / Prevent unnecessary feedbacks
   1. Add translations
   2. Add plural / none
   3. Add max number of documents displayed
   4. Reponsive > styles from figma > ~Redesign to act
   5. Remove comments
   6. Remove lines if empty > 1
   7. If a component hasn't content, auto-close it
   8. ♻️ Refacto duplicate code to `computed` or `method`
   9. Jeter un oeil au linter
3. ♻️ CRA
4. 🤯 Sur notion il y a les screenshots, filtre JC uniquement, pas JM

---

### 👨‍🏫 Evogue

1. ⏳ Préparer les prochaines missions
   1. ⏳ 2306 - Mission juin 2023 - 3 jours - JS PHP - Visio🎥
      1. ⏳ Cours à préparer
         1. ⏳ Projet API / Pokédex > Lier à JS avec bouton qui call et met à jour en live
            1. A voir en fonction de l'avancement fin de la 2eme journée
   2. Mission du 31 juillet au 4 aout / 5 jours / DevOps
      1. 🏭 Appliquer BP
      2. ⏳ En attente de contrat, 1ère partie 1 jour juillet ok, manque 4 jours août
         1. Réserver trains
         2. Trouver logement
2. 🏭 Pré-requis PHP / Mysql installation etc.
3. Mettre dans mes cours > debrander
   1. Blog

---

## Masamune

1. 👥 Dédoublonner la TODO
2. Vérifier si des screens des anciens sites ont bien été pris

### Déplacer blog

1. Appliquer les recommandations de la google search console, onglets déjà ouverts
   1. 🚨 Problème indexation des pages
      1. /dev-et-prog/gestion-de-l-encodage-utf-8-via-excel/
      2. /dev-et-prog/mysql-bonnes-pratiques-creer-un-utilisateur/
      3. les deux `<meta name="robots" content="noindex, nofollow`
      4. 💩💩 Cela se passe lorsqu'un 🚨 **COMMENTAIRE** 🚨 est rajouté ???
2. [30 SEO hacks](https://aioseo.com/seo-hacks-to-grow-your-traffic/)
   1. & liste fin de site
3. Recherche `?s=Truc` > `/recherche/` ? si c'possible
4. Process ajout article > MD en dehors de www
    1. Prévoir des images pour l'intérieur de l'article (3+), pour le SEO
       1. title & alt
    2. Sur chaque article > Ai1SEO > Partage > FB > Image à la une
    3. Forcer création du cache de page `/?action=wpfastestcache&type=preload`
5. 🚨🔥 [Et merde](http://recup-blog.masamune.fr/)
   1. Rapatrié de mémoire
6. 📌 Check retours mails DMARC
7. Guthib
8. Nouveaux articles + diffusion sur la durée
    1. PHP 8.2
    2. Cours
    3. Article de blog déplacer ce putain de wordpress
       1. Permaliens
       2. Enregistrer divi afin de finir de basculer les urls
    4. [Lien vers la doc ~htaccess ovh](https://help.ovhcloud.com/csm/fr-documentation-web-cloud-hosting?id=kb_browse_cat&kb_id=e17b4f25551974502d4c6e78b7421955&kb_category=98441955f49801102d4ca4d466a7fdb2)
    5. Mushroom ketchup
       1. Pas faire au gros sel, sel fin, moins de 5% du poids
       2. Ajout bout de vigne
          1. Micro onde 2 min + image unreal tournament chambre a pression fig1 avant (gonflay) fig2 apres (explosé) avec paint crade tête de fourmi à la place de celle du mec
          2. Fumé > chalumeau
       3. Si trop salé > Ajouter des poterres émincées à la mandoline, et cuire 10-15mn
          1. ça épaissit, nice
          2. Après filet d'huile d'olive > four > Chips
    6. Emails SPF DKIM DMARC avec ressources du site checklist + ce que mwa j'ai rajouté
       1. Attente retour ticket OVH
    7. Corrections "rapides" afin d'optimiser le référencement du blog
       1. Validateurs
       2. images > title & alt & h & w
9. 📌⏳ Vérifier [Google analytics](https://analytics.google.com/analytics/web/#/report-home/a26782507w69814287p71948494)
10. 📌⏳ [Google search console](https://search.google.com/search-console?resource_id=sc-domain%3Ablog.masamune.fr)
    1. [Insight](https://search.google.com/search-console/insights/?resource_id=sc-domain%3Ablog.masamune.fr&hl=fr&ga_view_id=71948494)
    2. 📝 [Tuto](https://support.google.com/webmasters/answer/6258314?hl=fr)
11. ⚡️🔌💸 Fastest cache premium quand il y aura une promo
12. 🌱 Changer de theme le 2023 est vraiment moisi aucun controle
    1. 🐛 F.FIX images du theme > pas d'attribut title -_- > dans le nouveau wp "title" correspond au nom de la page dédiée au média
       1. Vérifier qu'aucune des anciennes image ne fait plus de 50ko, cf. wagyu qui était a 200ko > Flemme en vrai
       2. Les grilles d'articles n'utilisent pas les miniatures d'images mais les grandes ? wtf
       3. Toutes les images > Attributs `height` & `width`
    2. Pas de defer/async sur les ressources (css/js/fonts surtout)
    3. Cleaner pour [accessibe](https://accessibe.com/accessscan)
13. 🌱 Faire une newsletter
    1. GA > search console > conversion

### Déplacer site vitrine

1. Bleu masa osef #43a8d3, plus clair #49cced, Rouze #9b000e, Rauz #ff00ff
2. ~Types de clients > PME / Renfort d'équipe / gros clients ?
3. 🚀 Pages de bases
   1. Accueil
      1. Projets > 2 autres carousel
      2. 🌱 Images profil > Photo
      3. Changer images de fond
   2. Contact
   3. A propos
   4. ~~🌱 Prestations / Services~~
   5. Portfolio > affichage des principales catégories
4. Pages secondaires
   1. CGV
   2. Crédits
   3. Mentions légales
   4. RGPD
5. Menus
6. Header
7. Footer
8. 🍻 Passer en ligne
    1. 🚀 Maj accès benner ancien
    2. 🌱 SPF SI besoin (ptet pour tout masamune ?)
9. 📋 Process nouveau projet
    1. Cloner `cv-portfolio-tout/portfolio/projets/_BP_README.md`
    2. Remplir les informations de base
    3. Rapatrier images si c'pas déjà fait et clean
       1. Process `cv-portfolio-tout/README.md`
          1. Récupérer depuis `/Desktop/tas de merde now/masamune.fr dump fichiers/uploads`
          2. A bouger dans `cv-portfolio-tout/portfolio`
          3. 🔥 Infos sensibles > noms projets, noms clients, identifiants
       2. Vérifier si logo entreprise dans le dossier
       3. `README.md` portfolio > textes title & alt
       4. WP > Ajouter aux médias
    4. 🚀 Page WordPress
       1. Titre du projet : NOM_PROJET
       2. Date de publication : Date dans CV & Premier du mois & 12:00
       3. Publier > Vérifier Url
       4. Catégories > Ajouter uniquement enfants
          1. Si nouvelles catégories ajouter au BP
       5. Tags > Pluriel uniquement
          1. Sujets du site
          2. Styles/Ambiance minimaliste / moderne / luxe / classique / one page
       6. Image en avant > Carré ( 512 x 512, TinyPNG )
          1. Title `Masamune / PROJET / CLIENT / TYPE_PROJET`
       7. Extrait
          1. `Réalisation d'un site vitrine pour un architecte, qui souhaitait un design minimaliste, et une administration simple à prendre en main.`
          2. Type de projet, type de client, objectifs du projet.
          3. 2 lignes max
       8. Désactiver commentaires
    5. 💾 Rapatrier textes dans portfolio `cv-portfolio-tout/portfolio/projets/CLIENT/README.md`
    6. Utiliser Divi
       1. Choisir la mise en page
       2. Télécharger le modèle
       3. Charger à partir de la bibliothèque "YYMMDD (latest) Projet"
       4. Remplacer les contenus
          1. Si pas d'image > Fond > Motif > Cube + #49CCED
          2. Vérifier si vidéo youtube
       5. 🚨 Pas oublier
          1. Liens > Ajouter liens
          2. Images > Visionneuse ou lien fichier direct
             1. CSS perso `max-height: 300px; overflow: hidden; width: 100%;`
             2. Styles > Espacement > Marge externe basse > 2em
          3. Missions > logo client à la place de celui masamune
          4. Vérifier en mode texte à la fin qu'il n'y a pas d'ajout de balises alakon `<div><span>&nbsp;`
          5. 📱 Responsive
    7. 💾 Github
10. 🌱 Check contenus ancien site avant bennage, notemment pour les anciens projets
11. 🌱 Ajouter des descriptions aux [catégories (de projet)](https://prod.masamune.fr/wp-admin/term.php?taxonomy=project_category&tag_ID=3&post_type=project&wp_http_referer=%2Fwp-admin%2Fedit-tags.php%3Ftaxonomy%3Dproject_category%26post_type%3Dproject)
12. 🌱 Portefeuille (autres projets) > Ajuster catégories similaires
13. 🌱 Ajuster Portefeuille (autres projets) quand 3+
14. Test plugin SiteGround Optimizer

---

1. masamune.fr > prod-old
   1. Sauvegarde github
   2. Sauvegarde sur DD sites web
   3. 🌱 Maj liens cv expériences pro
      1. Pas oublier le https
   4. Yootoob > Ajouter écrans de fin / liens vers le site masamune.fr une fois terminé
   5. Service > Retour sur CV > 50€
2. 🌱 Sites masamune apray 🌱
   1. Rajouter ancien folio
   2. Rajouter screens siteS v3
   3. Blog > articles en TODO
3. github > cleaner
   1. Renommer préfixer technos
   2. Voir faire un projet liste de liens vers les projets regroupés en catégories
   3. dédoublonner default-config-files-for-github-repository & base-repository-github

---

1. Maj tout masamune
   1. Voir logs séparés, problème htaccess stockage.masamune.fr
   2. 🤏 Virer la merde de _dev/
   3. [Perso branding](https://andela.com/insights/personal-branding-for-technology-professionals)
   4. Maj liste de liens
      1. 1 colonne intemporel
      2. 1 colonne par année decroissante (récent)
   5. masamune
      1. clean secrets ids ffs
      2. masamune--fr
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
      3. Remettre tous les anciens trucs max dans un seul dossier sur un seul dd (~bureau ancien pc)
         1. & dossier Bureau/shame
2. Migration avant 2023 [google analytics 4](https://mail.google.com/mail/u/0/#inbox/FMfcgzGpFWSCZKSSbnBjmgLtgpFfLWxC)
3. Dashlane > virer tous les identifiants merdiques

---

1. install-dev-env > docker-compose pour les principales technos : js & phpay
   1. Nginx + conteneur de gestion de conteneurs
2. 🔍 [tmux](https://nickjanetakis.com/blog/who-else-wants-to-boost-their-productivity-with-tmux)
3. 🔍 [keys remap](https://nickjanetakis.com/blog/remap-and-set-global-hotkeys-on-windows-10-with-auto-hotkey)

### Auto entrepreneur

1. Mise à jour devis
   1. Ajouter clause devis possibilité évolution de tarifs si sous estimation
      1. Non > Si gros projet > découpage en plein de minis devis afin de mieux contrôler les délais
   2. En cas d'arrêt des travaux / litige > remboursement de l'hébergement avancé
2. Renvoi doc AE décla 0€ années passées [hey](https://mail.google.com/mail/u/0/#inbox/FMfcgxmXKmkCGqSQkpPRbBrSKWcsbCpr)
3. CPF > Non périssable > ~2k€
4. Inscription EAN
   1. Maj linked in
   2. [hey](https://www.cominjob.com/candidat/)
   3. [hoy](https://www.ouiboss.com/)
   4. [prout](https://www.freelance-informatique.fr/)
   5. Inscription [crème de la crème](https://mail.google.com/mail/u/0/#inbox/FMfcgzGqQmNcddHDMfMMGTKJmgzNsvbd)
   6. Inscription Jean-Paul.io
   7. [odoo](https://www.odoo.com/fr_FR/jobs)
   8. [capgemini](https://www.linkedin.com/safety/go?url=https%3A%2F%2Ffr.capgemini.talentnet.community%2F&trk=flagship-messaging-web&messageThreadUrn=urn%3Ali%3AmessagingThread%3A2-MjdmZGZlYjgtZjIxNy00ZDM0LTg2ODYtMzIyYzMwNzcxMzUzXzAxMg%3D%3D&lipi=urn%3Ali%3Apage%3Amessaging_thread%3B984fd009-b4db-44e3-b159-e504a3614444)
   9. [Andela](https://client.andela.com/)
   10. [JS / Easypartner](https://forms.easypartner.fr/t/rpxghfLTNFus?firstname=Maxime&lastname=CHEVASSON&email=masamune.code@gmail.com)
5. [Malt PER](https://resources.malt.com/fr/freelances/articles-freelance/reduction-dimpots-avez-vous-pense-a-cette-solution/)
6. Veille
   1. [Arrêt maladie : les démarches du travailleur indépendant](https://www.ameli.fr/assure/droits-demarches/maladie-accident-hospitalisation/arret-travail-maladie/arret-travail-maladie-independants)
   2. 💥 CPF [Prise en charge des formations des travailleurs indépendants](https://entreprendre.service-public.fr/vosdroits/F31148)
   3. [Quand prendre sa retraite ?](https://www.lassuranceretraite.fr/portail-info/home/actif/travailleur-independant/depart-retraite/inde-quand-retraite.html)

---

## 💪 Perso

1. [Bible Dry age](https://www.fumoir.net/accessoires-maturation/403-la-bible-dry-ager-de-la-maturation-de-viande-version-anglaise.html)
2. Musiques taf & portable
3. Peinture Chtulu
    1. [How to paint Extreme Light Sources - OSL tutorial](https://www.youtube.com/watch?v=c48UiPSBfcg)
    2. [INDESTRUCTIBLE Gaming Bases - Quick & Easy](https://www.youtube.com/watch?v=tRFfsAG-Yf8)
    3. Green gold pour le [grand ancien](https://www.youtube.com/watch?v=AgJqjIMd6k8)
4. Bouffe mayzon
    1. [Gochuan mayson](https://www.youtube.com/watch?v=GyzWB5wh4Yw)
    2. [Vinaigres](https://www.youtube.com/watch?v=V9nfVu9zGxk)
    3. [Pickles](https://www.youtube.com/watch?v=LBvr0K-6NIY)
    4. [4 recettes](https://www.youtube.com/watch?v=WZS07jU4U50) Moutarde fermentée / Huile origan / Sésame tahini / Cashew miso
5. Appli radiateurs et config
6. MSG maison
    1. [Recette](https://www.youtube.com/watch?v=sE3dYCphy2M)
7. 🔍 Régime
    1. PORK PANKO low carb !
    2. [Low carb](https://www.dietdoctor.com/low-carb) / keto
       1. Most fruits and fruit juice / **Although low-sugar berries — such as blackberries, raspberries, and strawberries — are ok in small to moderate amounts.**
    3. Keto wheat flour > farine avec prot ? [hey](https://www.youtube.com/watch?v=g2fTYDftlCg)
    4. Non fat ricotta cheese / provolone cheese
8. 🔍 Champignon Lingzhi contre la fatigue & insomnie > Y'en a à grand frais !
9. 🌱 Orga anniv pougnoutte mars 2023
    1. Idées cadeaux
       1. Vélo, a voir en revenant de vacances
       2. Robe style médiéval, demander à Mélanie
       3. Machine pour frapper sa propre monnaie (étain), initiales VL (Vigi & Lucifer)
       4. Bouclier armoiries normandie viking (VL)
       5. Machine à coudre
       6. Table air hockey
    2. Redemander date a pougnoutte > mars...
    3. Demander contact & liste invités
    4. Demander si logement déjà vu
    5. Voir pour cagnotte permis moto
    6. Medieval tents
10. Musique groupe "3 days grace"
11. Anime "Redo of healer"

---

## 💩 Shame

Parfois, l'entropie.

Emplois du temps stockés sur mail, portable, favoris, bureau.

Extraire ici puis ranger & prioriser. Doit rester vide.

---

1. ⚡️ Rapide
   1. ✅ Envoyer RIB à [Antouin](https://www.facebook.com/messages/t/1374335482651102)
      1. ⏳💸 Vérifier remboursement, tétine 10€, et un body bébay 6 mois 18€, donc 28 € en tout :)
   2. ✅ Cashless HF 2023 > Remboursement
      1. ✅ Puce Vigi `JLOXXX`, billet `66 40 XXX`, `masaXXX@gmail.com` > Demandé le 20/06/23
         1. ⏳💸 Vérifier remboursement, 269,45€ balles
      2. ✅ Puce Max `OYJXXX`, billet `66 40 XXX`, `hebXXX@gmail.com` > Demandé le 20/06/23
         1. ⏳💸 Vérifier remboursement, ~20 balles
   3. Prendre les places pour le festival ketfest à gisord
   4. 473€ CFE, 16 juin 2023 > Garder trace paiement, il y a un mail également
   5. FB/Mail Bérangère organisation vacances : Du 23 juillet au soir jusqu'au 26 ~matin
   6. Sauce piquante.fr > Lien vers sauce pour darons > Renvoyer par [mail](https://www.sauce-piquante.fr/3-sauce-barbecue)
   7. Rappels badminton + ajouter emplois du temps tel : mercredi et vendredi
   8. Partage fb nouvel article blog
   9. Vérification [changement flixbus ?](https://mail.google.com/mail/u/0/#inbox/FMfcgzGsnBlBrVpFBvdVljFsgTdhFmQV)
   10. 🎵 Concert little big 21 octobre strasbourg
   11. ⏳ Gérer [évolution google analytics](https://mail.google.com/mail/u/0/#inbox/FMfcgzGsmWwnjMCCzPJJrGwvqRmTkVrP) / Cleaner tout
       1. ⏳ Attendre 48h et vérifier présence de données pour chacun

---

1. 🔨 Normal / Chop chop
   1. Ranger hellfest
      1. Préparer/regrouper t-shirts javier (2 anciens & 3 nouveaux)
      2. Mes darons
      3. Récupérer photos & vidéos, compresser, drive, partager // Egalement dans 2eme groupe FB métalleux
   2. 🧽 Cleaner bordel ambiant appartement
      1. Truc cafay dans vinaigre blanc
      2. Nettoyer frigo
      3. Cuisine
      4. Poubelles
      5. Verre
      6. Aspi
      7. Brita
      8. Jardin > Récolter, cleaner
         1. Aller racheter des pots > Fraisiers replanter truc de dinde au milieu
   3. 🏃 Aller chercher colis amazon > gélules huile de foie de morue, cf. sms
   4. 🏃 Aller récupérer une fig qui attend au GW de reims [depuis 2022](https://mail.google.com/mail/u/0/#inbox/FMfcgzGsnBfQZmhMMmRJJQVMGsqWDKdH)
   5. 🏃 Acheter flotte > magnésium
   6. Anniv vigi
   7. ⏳💸 Attente retour francis pour payay le Hellfest

---

1. 🌱 Moins urgent
   1. Retrouver le correcteur de posture
   2. 👨‍⚕️ Alan > évolution offres > [baisser tarifs ?](https://mail.google.com/mail/u/0/#inbox/FMfcgzGsnBhjwhRxzJXXKQRLjbNbRPML)
   3. Préparer prochaine séance de tatoo
   4. 🏃 Magazine "science des épices" > Voir si toujours dispo ou pdf en ligne
   5. OST Ghost in the shell le film
      1. Choper des images d'inspi
      2. Toshop de proposition combler le blanc ?
   6. Musiques Hellfest
      1. 1 earth
      2. Architects
      3. Crisix
      4. In flames > dernier album
      5. Pantera
      6. Skynd
   7. Checker taf > micro frontend 1500 -2500 / journée

---

1. Site vitrine
   1. Page catégories avec les projets existants
   2. Site en construction
2. ⚡️ [heberg wp](https://wpmudev.com/hosting/#dev-plans)
3. Maj CV
   1. Maj age
   2. Process maj cv > maj fr--masamune & reup
4. Evogue
    1. Donner les cours > Projet API / Pokédex
5. OVH Manager > desactiver protection transfert domaine et re-test
6. ⏳ Jus Mundi
    1. ⏳ En attente de retour de Javier pour la dernière mini-intégration avant de passer aux choses sérieuses
7. Masamune > Déplacer anciens sites
    1. 🌱 Finaliser blog
    2. Finir Déplacer site vitrine
    3. CV tout est good
8. Perso
    1. 🎂 [Orga anniv pougnoutte](https://drive.google.com/drive/folders/1gjOfZsH-a8l7yWM7sCDSziNkCIQbeWbY?usp=drive_link)
       1. 🚀 Liste des invités
       2. Dates
       3. Lieux
       4. Activités
       5. Dépenses
       6. Images
       7. Espace de discussion
    2. ⏳💸 Appeler BRED, cf. edt tel
       1. Changer de conseiller
       2. Remboursement des frais injustifiés
       3. Résiliation de "BPCE Assurances IARD"
       4. Call & mails envoyés le [11/05/2023](https://drive.google.com/drive/folders/1bqIpMlzVT7OYL9FkUdm9h6LbAFJCG4q7)
    3. Meuble bar > cleaner éclats de la réparation
    4. 🍔 [Croissants high hydration dow](https://www.youtube.com/watch?v=GSlBVCbgFhE)
    5. Rappeler Gauthier
    6. Rappeler Anouk
    7. 👨‍⚕️ RDV dermato > Obligé d'appeler
        1. Julie Plee / 03 26 85 42 88
        2. Ziad Reguaï / 03 52 15 08 08
    8. 👨‍⚕️ Alan > Faire exos pour le dos > Pas sur le site internet, appli seulement :/

---

### Priorisation

Ordonner puis ranger dans le flux. Doit rester vide.

---

---

Tout est priorisé :)

---
