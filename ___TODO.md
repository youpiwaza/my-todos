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
- ❌ Nope

## 🧠⏫ Raccourcis & process à intégrer au flow

- 🤯 Plugin VSCode pour WSL
- Dactylo le midi > [typing study](https://www.typingstudy.com/fr/lesson/3/part/8)

Installation de google analytics via [tag manager](https://tagmanager.google.com/)

## 🚀 Priorisation, simple ⏩

Indiquer ici les *tâches à effectuer en priorité*

- Sert de sommaire > Ctrl + F vers détails plus bas
- Si besoin de focus, mettre une ou 2 tâches ici.
- Ne pas tout fourrer ici, *respecter la priorisation*, sinon tout est fait à l'arrache

1. ⏳ Evogue > Envoyer facture 4 jours aout pour DevOps
   1. ⏳ Attente de savoir si mission 1 semaine fin août
   2. Attente paiement
   3. Confirmer reception
2. Blog > 📌🐛 Corriger Indexation
3. Perso > Orga anniv pougnoutte
4. Recup photos facebook

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

- ✅ Déplacer les terminés ⏳ à chaque début de semaine dans done.md
- 💩 Déplacer les TODO 🌱 dans _TODO_shame.md
- ✅ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur ✅ mails, ✅ edt portable, ✅ favoris, ✅ bureau. Si possible description + lien.
- ✅ Nettoyer le fichier __TODO
  - ✅ Status
  - ✅ Ce fichier > ### Shame 💥 Cleaner pour vrai les trucs ou je ne passe jamais
    - ⏳ Ranger dans fichiers TODO correspondant
      - ⏳ Prioriser
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
- ✅ Déclaration Auto entrepreneur / aout 2023
- ✅ Vérifier impôts sur espace
  - ✅ Perso  / Revenus 2022
  - ✅ Pro    / 11/04/2022
- ⏳ Vérifier messages [Ameli](https://assure.ameli.fr/)
- ✅ Maj locales / Environnement de dev / Dernière maj le 01/06/21 / lel
  - ✅ CHKDSK / Besoin de param `/f` ou [ne répare pas](https://docs.microsoft.com/fr-fr/windows-server/administration/windows-commands/chkdsk), `/r` également
    1. Invite de commande ou Powershell **en admin**
    2. `chkdsk c: /f /r` (et en fonction de vos disques.. && `chkdsk d: /f /r`, etc.)
    3. `>Blah blah besoin de redémarrer O/n` >> `O`
    4. Redémarrer / Attendre 5 ans et demi sauf si t'as un SSD/Nvme
  - ✅ Windaube
    - ✅ Update alakon
    - ✅ [.net](https://dotnet.microsoft.com/download) > Runtime
    - ⏳ Panneau de conf > "Fichiers temporaires" > "Fichiers temporaires" (dans les catégories) > Supprimer
  - ⏳ Drivers > [detection auto](https://www.touslesdrivers.com/index.php?v_page=29) > Lancer éxécutable, ça ouvre une page recap, et suivre liens dl
  - ⏳ Firmware SSDs / Dépend du constructeur > Voir site officiel, avec un peu de chance logiciel auto alakon
    - ⏳ Dell support assist
    - ⏳ Alienware update
    - ⏳💸 System mechanic
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
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade && sudo apt -y clean && sudo apt -y autoremove && docker system prune -af && npm install -g npm@latest && sudo npm install -f --global yarn && pnpm add -g pnpm && bun upgrade --canary
```

- ⏳ Téléphone
  - ⏳ Maj de la base
  - ⏳ Maj des applications
  - ⏳ Tous les 6 mois > reset usine
- ~⏳ Compléments alimentaires
  - ⏳ Anaca3
  - ✅ Huile de foie de morue
  - ✅ Choline Inositol
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

rieng

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

1. 🎯 Objectifs en gros > . . .
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

1. Préparer les prochaines missions
   1. Mission du 31 juillet au 4 aout / 5 jours / DevOps
      1. ✅ Docker
         1. ✅ Tutoriaux docker desktop en premier
         2. ✅ Correction via Dockerfile
            1. [Nginx](https://github.com/youpiwaza/server-related-tutorials/blob/master/01-docker/04-my-tests/01-min-static-site/site/Dockerfile)
            2. avec PHP
         3. ✅✨ Correction [docker compose](https://github.com/youpiwaza/server-related-tutorials/tree/master/01-docker/04-my-tests/02-compose-nginx-php)
         4. ~~Exemples avec conteneur en SSH > Configurer un serveur web~~
      2. ✅📌 Vérifier sommaires
      3. ✅📌 Vérifier temps de présentations
      4. ✅ Cleaner corrections
      5. ✅ Re-balancer dans DRIVE /prof en écrémant
      6. 🚀 Balancer dans repo prof / corrections etc.

---

### Masamune

1. 🚨 Impots juillet décalés, idem août yay fun
2. Taf us turing
3. OVH Manager > desactiver protection transfert domaine et re-test
4. ⚡️ [heberg wp](https://wpmudev.com/hosting/#dev-plans)
5. Maj CV > age

### Blog

1. 📌🐛 Corriger Indexation
2. [Article blog](https://blog.masamune.fr/wp-admin/post.php?post=192&action=edit)
      1. Juste à compléter, image déjà en place
3. Article blog
   1. WordPress > Divi > Améliorer Pagespeed en chargeant les styles, fonts & scripts nous même (thème enfant)
      1. Google web fonts > [Helper fonts](https://gwfh.mranftl.com/fonts), cf masamune.fr pour mise en place
      2. styles.css
      3. functions.php
         1. Google recaptcha
         2. Google Tag Manager / Google Analytics
         3. Script perso dans un fichier alakon
      4. Sinon dans le footer php > utiliser `async` ou `defer`
   2. Notes jardin
      1. Frequence arrosage sauge basilic 1x tous les 3jours, préférer par en dessous (coupelles). Tomates tous les jours
      2. Piments poivrons, semis sur peau de banane (et dans engrais)
      3. Récolter herbes aromatiques ~toutes les 2 semaines
   3. Falafels & houmous, photos déjà faites, recette dans carnet
   4. Captures écran > installer & configurer OBS Observer
   5. Logos > Augmenter la taille, nettoyer, crispyyy > tinypng
   6. [99 /  Bonus / Outils du Dev](https://docs.google.com/presentation/d/10XK2uOq3G0MnlsokNBBqV7VPkTIGprrhRxHnnX4Hrdo/edit#slide=id.g20f9d5d5cf0_0_0)
4. Ranger doc robots.txt dans un article de blog
   1. [google](https://developers.google.com/search/docs/crawling-indexing/robots/robots_txt?hl=fr)
   2. [bing](https://www.bing.com/webmasters/help/how-to-create-a-robots-txt-file-cb7c31ec)

---

### Site vitrine

1. 🚀 404
2. Mobile > Passions > Carousel KO
3. Maj pages secondaires blog ?
4. CGV
    1. Revoir clause 6 retard de paiement > Cleaner avec celle devis/factures
    2. Rassembler 8 & 13, propriété intelectuelle
    3. Vérifier uniformité et versionner > SST
5. Vérifier permaliens
6. Vérifier console
7. Faire un backup texte / Gros cc contenus textes sur word, par page
    1. images pages > fr--masamune/assets
8. Repasse prestations ? [hey](https://docs.google.com/document/d/1w88CIdw7LNbKpmFHZbWhWxXU2kAeXVSHKGaAcSUJyfg/edit?pli=1)
9. Toutes les images mises en avant pour les pages
    1. Config partages all in one seo
10. Pages auto
    1. Page de recherche
    2. Page affichage des résultats de recherche
    3. Page cat projet > [hey](https://masamune.fr/categorie-projet/developpeur-web/) avec liens sur la page d'accueil
    4. RGPD > Revoir via génération automatique (google analytics, wp, plugins)
11. 📌 Google search console
    1. Problèmes indexation

---

### Perso 2

1. Retrouver le correcteur de posture
2. 👨‍⚕️ RDV dermato > Obligé d'appeler
   1. Julie Plee / 03 26 85 42 88
   2. Ziad Reguaï / 03 52 15 08 08
3. 👨‍⚕️ Alan > Faire exos pour le dos > Pas sur le site internet, appli seulement :/
4. Changer les filtres a flotte > Voir si besoin d'en racheter, de mémoire 1
5. Meuble bar > cleaner éclats de la réparation
6. 🍔 [Croissants high hydration dow](https://www.youtube.com/watch?v=GSlBVCbgFhE)

---

#### 🎂 Orga anniv pougnoutte

Idées cadeaux

1. ✅ Zaylda
2. Cagnotte permis moto
3. Portefeuille kewl
4. Vélo, a voir en revenant de vacances
5. Robe style médiéval, demander à Mélanie
6. Machine pour frapper sa propre monnaie (étain), initiales VL (Vigi & Lucifer)
7. Bouclier armoiries normandie viking (VL)
8. Machine à coudre
9. Table air hockey

---

#### 🌱 Moins urgent

1. Toutes les musiques de salvatore ganacci
2. 👨‍⚕️ Alan > évolution offres > [baisser tarifs ?](https://mail.google.com/mail/u/0/#inbox/FMfcgzGsnBhjwhRxzJXXKQRLjbNbRPML)
3. 🏃 Magazine "science des épices" > Voir si toujours dispo ou pdf en ligne
4. OST Ghost in the shell le film
5. Musiques Hellfest
   1. 1 earth
   2. Architects
   3. Crisix
   4. In flames > dernier album
   5. Pantera
   6. Skynd
   7. metal jap
      1. Gyzeh
      2. Fumata

---

## 💩 Shame

Parfois, l'entropie.

Emplois du temps stockés sur mail, portable, favoris, bureau.

Extraire ici puis ranger & prioriser. Doit rester vide.

### Github

1. Renommer préfixer technos
2. Voir faire un projet liste de liens vers les projets regroupés en catégories
3. dédoublonner default-config-files-for-github-repository & base-repository-github

---

### 🌱 later

1. install-dev-env > docker-compose pour les principales technos : js & phpay
2. [Perso branding](https://andela.com/insights/personal-branding-for-technology-professionals)
3. [tmux](https://nickjanetakis.com/blog/who-else-wants-to-boost-their-productivity-with-tmux)

---

### Auto entrepreneur

1. Mise à jour devis
   1. Ajouter clause devis possibilité évolution de tarifs si sous estimation
      1. Non > Si gros projet > découpage en plein de minis devis afin de mieux contrôler les délais
   2. En cas d'arrêt des travaux / litige > remboursement de l'hébergement avancé
2. Renvoi doc AE décla 0€ années passées [hey](https://mail.google.com/mail/u/0/#inbox/FMfcgxmXKmkCGqSQkpPRbBrSKWcsbCpr)
3. Inscription EAN
   1. Maj linked in
   2. [aquent](https://aquent.com/find-work)
   3. [..](https://developers.turing.com/welcome?token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1aWQiOjEyMTE4NDAsImxhbmRpbmciOnRydWUsImVtYWlsIjoibWFzYW11bmUuY29kZUBnbWFpbC5jb20iLCJyb2xlX2lkIjozLCJuYW1lIjoiTWF4aW1lIENoZXZhc3NvbiIsImlhdCI6MTY5MjA2Nzg3MSwiZXhwIjoxNjk3MjUxODcxfQ.T-JQB-1GqZ1xOcrHjrOVphtvJwF2Fc-yh0nJ_4KilJg)
   4. [hey](https://www.cominjob.com/candidat/)
   5. [hoy](https://www.ouiboss.com/)
   6. [prout](https://www.freelance-informatique.fr/)
   7. Inscription [crème de la crème](https://mail.google.com/mail/u/0/#inbox/FMfcgzGqQmNcddHDMfMMGTKJmgzNsvbd)
   8. Inscription Jean-Paul.io
   9. [odoo](https://www.odoo.com/fr_FR/jobs)
   10. [capgemini](https://www.linkedin.com/safety/go?url=https%3A%2F%2Ffr.capgemini.talentnet.community%2F&trk=flagship-messaging-web&messageThreadUrn=urn%3Ali%3AmessagingThread%3A2-MjdmZGZlYjgtZjIxNy00ZDM0LTg2ODYtMzIyYzMwNzcxMzUzXzAxMg%3D%3D&lipi=urn%3Ali%3Apage%3Amessaging_thread%3B984fd009-b4db-44e3-b159-e504a3614444)
   11. [Andela](https://client.andela.com/)
   12. [JS / Easypartner](https://forms.easypartner.fr/t/rpxghfLTNFus?firstname=Maxime&lastname=CHEVASSON&email=masamune.code@gmail.com)
4. [Malt PER](https://resources.malt.com/fr/freelances/articles-freelance/reduction-dimpots-avez-vous-pense-a-cette-solution/)
5. Veille
   1. [Arrêt maladie : les démarches du travailleur indépendant](https://www.ameli.fr/assure/droits-demarches/maladie-accident-hospitalisation/arret-travail-maladie/arret-travail-maladie-independants)
   2. 💥 CPF [Prise en charge des formations des travailleurs indépendants](https://entreprendre.service-public.fr/vosdroits/F31148)
      1. CPF > Non périssable > ~2k€
   3. [Quand prendre sa retraite ?](https://www.lassuranceretraite.fr/portail-info/home/actif/travailleur-independant/depart-retraite/inde-quand-retraite.html)

---

## 💪 Perso

### 🌱 later aussi

1. 🔍 Champignon Lingzhi contre la fatigue & insomnie > Y'en a à grand frais !
2. 🔍 Régime
    1. PORK PANKO low carb !
    2. [Low carb](https://www.dietdoctor.com/low-carb) / keto
       1. Most fruits and fruit juice / **Although low-sugar berries — such as blackberries, raspberries, and strawberries — are ok in small to moderate amounts.**
    3. Keto wheat flour > farine avec prot ? [hey](https://www.youtube.com/watch?v=g2fTYDftlCg)
    4. Non fat ricotta cheese / provolone cheese
3. Bouffe mayzon
    1. [MSG maison](https://www.youtube.com/watch?v=sE3dYCphy2M)
    2. [Gochuan mayson](https://www.youtube.com/watch?v=GyzWB5wh4Yw)
    3. [Vinaigres](https://www.youtube.com/watch?v=V9nfVu9zGxk)
    4. [Pickles](https://www.youtube.com/watch?v=LBvr0K-6NIY)
    5. [4 recettes](https://www.youtube.com/watch?v=WZS07jU4U50) Moutarde fermentée / Huile origan / Sésame tahini / Cashew miso
4. Musiques taf & portable
5. Peinture Chtulu
    1. [How to paint Extreme Light Sources - OSL tutorial](https://www.youtube.com/watch?v=c48UiPSBfcg)
    2. [INDESTRUCTIBLE Gaming Bases - Quick & Easy](https://www.youtube.com/watch?v=tRFfsAG-Yf8)
    3. Green gold pour le [grand ancien](https://www.youtube.com/watch?v=AgJqjIMd6k8)

---

### Priorisation

Ordonner puis ranger dans le flux. Doit rester vide.

---

---

Tout est priorisé :)

---
