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

1. Blog > 📌🐛 Corriger Indexation
2. Perso > Orga anniv pougnoutte
3. Jus

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

- ⏳ Déplacer les terminés ✅ à chaque début de semaine dans done.md
- 💩 Déplacer les TODO 🌱 dans _TODO_shame.md
- ⏳ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur ⏳ mails, ⏳ edt portable, ⏳ favoris, ⏳ bureau. Si possible description + lien.
- ⏳ Nettoyer le fichier __TODO
  - ⏳ Status
  - ⏳ Ce fichier > ### Shame 💥 Cleaner pour vrai les trucs ou je ne passe jamais
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
    - ⏳ Update alakon
    - ⏳ [.net](https://dotnet.microsoft.com/download) > Runtime
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
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade && sudo apt -y clean && sudo apt -y autoremove && docker system prune -af && npm install -g npm@latest
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
      1. 🏭 Appliquer BP
      2. ⏳ En attente de contrat, 1ère partie 1 jour juillet ok, manque 4 jours août
         1. ⏳ Dispo au 1er juiller
         2. Réserver trains
         3. Trouver logement

---

### Masamune

1. OVH Manager > desactiver protection transfert domaine et re-test
2. Checker taf > micro frontend 1500 -2500 / journée
3. ⚡️ [heberg wp](https://wpmudev.com/hosting/#dev-plans)
4. Maj CV
   1. Maj age

### Blog

1. 📌🐛 Corriger Indexation
   1. Introuvable (404)
      1. 378
   2. Autre page avec balise canonique correcte
      1. ~~51~~
      2. 💩 58
         1. `http://blog.masamune.fr/bouffe/recette-mini-burgers/` manque **https** ?
         2. ~/tags/kaput/?query-0-page=1 **tags** au lieu de tag ?
         3. /2013/07/ ptain de date
         4. `/pages-secondaires/blog-template-alternatif/?cst&query-3-page=3` tf is   that // plusieurs
   3. Page en double sans URL canonique sélectionnée par l'utilisateur
      1. 97
   4. Exclue par la balise "noindex"
      1. 66
   5. Page avec redirection
      1. ~~14~~
      2. 💩 16
         1. /tags/adwords/?query-0-page=1 **tags**
         2. `/recette-mini-burgers/mini-burgers-pains-11/`
         3. /tag/veille/ Vérifier si les **tag_ existent toujours**
         4. Pas mal de http alakon à sniper
            1. `http://blog.masamune.fr/3wa-raccourcis/`
         5. `http://blog.masamune.fr/category/divers`
   6. Bloquée par le fichier robots.txt
      1. 1
   7. Explorée, actuellement non indexée
      1. 396
   8. Page en double : Google n'a pas choisi la même URL canonique que l'utilisateur
      1. 77
   9. Détectée, actuellement non indexée
      1. 17
2. [Article blog](https://blog.masamune.fr/wp-admin/post.php?post=192&action=edit)
      1. Juste à compléter, image déjà en place
3. Article blog
   1. Notes jardin
   2. Captures écran > installer & configurer OBS Observer
   3. Logos > Augmenter la taille, nettoyer, crispyyy > tinypng
4. Ranger doc robots.txt dans un article de blog
   1. [google](https://developers.google.com/search/docs/crawling-indexing/robots/robots_txt?hl=fr)
   2. [bing](https://www.bing.com/webmasters/help/how-to-create-a-robots-txt-file-cb7c31ec)

---

### Site vitrine

1. 📱 Vérifier responsive
2. Virer warnings PHP // Page grille projet
3. Maj pages secondaires blog ?
4. CGV
    1. Revoir clause 6 retard de paiement > Cleaner avec celle devis/factures
    2. Rassembler 8 & 13, propriété intelectuelle
    3. Vérifier uniformité et versionner > SST
5. Vérifier permaliens
6. Vérifier console
7. Faire un backup texte / Gros cc contenus textes sur word, par page
    1. images pages > fr--masamune/assets
8. Remplacer images placeholders
    1. Images requises
       1. Accueil
          1. Expertise
          2. Professorat
          3. Quelques chiffres
          4. Etudes
       2. Contact > En visio
9. Repasse prestations ? [hey](https://docs.google.com/document/d/1w88CIdw7LNbKpmFHZbWhWxXU2kAeXVSHKGaAcSUJyfg/edit?pli=1)
10. Toutes les images mises en avant pour les pages
    1. Config partages all in one seo
11. Pages auto
    1. Page de recherche
    2. Page affichage des résultats de recherche
    3. Page cat projet > [hey](https://masamune.fr/categorie-projet/developpeur-web/) avec liens sur la page d'accueil
    4. RGPD > Revoir via génération automatique (google analytics, wp, plugins)

---

### Perso 2

1. Préparer prochaine séance de tatoo
2. Retrouver le correcteur de posture
3. 👨‍⚕️ RDV dermato > Obligé d'appeler
   1. Julie Plee / 03 26 85 42 88
   2. Ziad Reguaï / 03 52 15 08 08
4. 👨‍⚕️ Alan > Faire exos pour le dos > Pas sur le site internet, appli seulement :/
5. Changer les filtres a flotte > Voir si besoin d'en racheter, de mémoire 1
6. Meuble bar > cleaner éclats de la réparation
7. 🍔 [Croissants high hydration dow](https://www.youtube.com/watch?v=GSlBVCbgFhE)
8. Rappeler Gauthier
9. Rappeler Anouk

---

#### 🎂 Orga anniv pougnoutte

1. [Drive](https://drive.google.com/drive/folders/1gjOfZsH-a8l7yWM7sCDSziNkCIQbeWbY?usp=drive_link)
2. ⏳ Liste des invités
   1. ⏳ Attente confirmations
3. Lieux
   1. Trouver gros AirBNB
4. Activités
5. Dépenses
6. Images
7. Espace de discussion
8. OLD
   1. Idées cadeaux
      1. Zaylda
      2. Vélo, a voir en revenant de vacances
      3. Cagnotte permis moto
      4. Robe style médiéval, demander à Mélanie
      5. Machine pour frapper sa propre monnaie (étain), initiales VL (Vigi & Lucifer)
      6. Bouclier armoiries normandie viking (VL)
      7. Machine à coudre
      8. Table air hockey
   2. Redemander date a pougnoutte > mars...
   3. Demander contact & liste invités
   4. Demander si logement déjà vu
   5. Voir pour cagnotte permis moto
   6. Medieval tents

---

#### 🌱 Moins urgent

1. 👨‍⚕️ Alan > évolution offres > [baisser tarifs ?](https://mail.google.com/mail/u/0/#inbox/FMfcgzGsnBhjwhRxzJXXKQRLjbNbRPML)
2. 🏃 Magazine "science des épices" > Voir si toujours dispo ou pdf en ligne
3. OST Ghost in the shell le film
   1. Choper des images d'inspi
   2. Toshop de proposition combler le blanc ?
4. Musiques Hellfest
   1. 1 earth
   2. Architects
   3. Crisix
   4. In flames > dernier album
   5. Pantera
   6. Skynd
5. Organiser une LAN pour les 10 ans de unreal tournament ek dus

---

## 💩 Shame

Parfois, l'entropie.

Emplois du temps stockés sur mail, portable, favoris, bureau.

Extraire ici puis ranger & prioriser. Doit rester vide.

---

### Priorisation

Ordonner puis ranger dans le flux. Doit rester vide.

---

---

Tout est priorisé :)

---
