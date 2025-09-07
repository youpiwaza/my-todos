# Taf en cours

- Recup photos facebook

## Légende

- 🚀 En cours / **1 MAX A LA FOIS**
- ✅ Terminé
- ⏩ Suite
- 🚧 WIP / Work In Progress / Entamé, pas terminé
- 📌 A tester / Recettage
- 🐛 bug
- 🔍 Lecture/Vidéos
- 🌱 Plus tard, besoin dépendance ou flemme sur le coup
- ♻️ Récurrent / Refacto
- 🚚 Contenus/notes dans les autres fichiers TODO
- 💩 KO
- ⏳ en attente
- 🤏 Petite partie
- 📝 Doc
- 📧 email envoyé/à envoyer
- ✨ Rien à toucher, déjà en place
- 👪 Réunion ou call
- ❌ Nope
- 💾 BDD
- 👀 voir
- 🎯 objectifs
- ❓❔ Question / Question répondue
- 👨‍💻 Notes dev
  - 👷 Exemple / Note pour aider les autres devs
- 🚨 Attention
- ⚡️🐌 Optimisation / Lenteur
- 🧠 Réflexions / Algos
  - 🔀 Alternative / Formattage
- ⏱️ Benchmarks OU tâche Avec estimations de temps
  - ➕ Taf en plus / Non compté dans l'estimation
- 💡📅🔢📝⌚ Types > Boolean / Date / Number / String / Time
- 👴⚰️ Obsolete / Dead code
- ⚗️ Filter / reduce
- 🔮 Anticiper les besoins futurs
- 🔙 Revert changes / Return type
- 🧰 Toolbox / utility
- 👌 Cleaner / ajouter des types
- 🧹 Cleaner le code, virer les console.log
- ⛓️ Contraintes
- 🔗 Relation
- 🛣️ Création de routes / roadmaps
- 📜 Gestion de l'historique
- 🧮 Inventorier
- ✂️ Découper
- 🔭 Scope
- 👥 Dédoublonner
- 👶💪🤮 Facile / Pas facile
- 🤖 Automatique / généré
- 💯 Résultat / Retour / Complété

---

## 🧠⏫ Raccourcis & process à intégrer au flow

- 🤯 Plugin VSCode pour WSL
- Dactylo le midi > [typing study](https://www.typingstudy.com/fr/lesson/3/part/8)

---

## 🚀 Priorisation, simple

hey

---

## Sinon, priorisation classique

1. ♻️ Tâches récurrentes
2. 🚧 Tâches WIP
3. 💥 Tâches critiques
4. ⚡️ Tâches rapides
5. ⏳ Tâches en attente
6. ⏳🌱 Vérifications sur la longueur
7. 🎯 A prioriser (quick dump)

---

## ♻️ Tâches récurrentes ♻️

Tâches à *vérifier au moins une fois par semaine*, afin d'éviter un bordel plus tard/exponentiel

- 💩 Déplacer les TODO 🌱 dans _TODO_shame.md
- ⏳ Shame TODOs : Extraire ici (## Shame) les emplois du temps stockés dans (Si possible description + lien.)
  - ⏳ mails,
  - ⏳ edt portable,
  - ⏳ favoris,
  - ⏳ bureau.
- ⏳ Nettoyer le fichier __TODO
  - ⏳ Status
  - ⏳ Ce fichier > ### Shame 💥 Cleaner pour vrai les trucs ou je ne passe jamais
    - ⏳ Ranger dans fichiers TODO correspondant
      - ⏳ Prioriser
- ⏳ Virer ce qui traine
  - ⏳ sur le bureau
  - ⏳ dans le dossier _shame du bureau
  - ⏳ Vider corbeille
  - ⏳ Vider téléchargements
  - ⏳ Dans les mails
- ⏳ Déplacer veille onglets dans TODO_veille
- ⏳ Veille / Un truc par semaine, genre le vendredi aprem, a githuber
- //
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
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade && sudo apt -y clean && sudo apt -y autoremove && docker system prune -af && sudo npm install -g npm@latest && sudo npm install -f --global yarn && pnpm add -g pnpm && bun upgrade --canary && sudo sh -c "/usr/bin/echo 3 > /proc/sys/vm/drop_caches" && swapoff -a && swapon -a && printf '\n%s\n' 'Ram-cache and Swap Cleared'
```

- High usage CPU & maintenance > [yay](https://fr.drivereasy.com/connaissances/resolu-wmiprvse-exe-haute-utilisation-cpu-sous-windows-10/)

cmd as admin

```bash
sfc /scannow
Dism /Online /Cleanup-Image /CheckHealth
Dism /Online /Cleanup-Image /ScanHealth
Dism /Online /Cleanup-Image /RestoreHealth
```

Restart pc

---

- ⏳ Téléphone
  - ⏳ Maj de la base
  - ⏳ Maj des applications
  - ⏳ Tous les 6 mois > reset usine
- ~⏳ Compléments alimentaires
  - ⏳ Huile de foie de morue
  - ⏳ Choline Inositol
  - ⏳ Doc > vitamine D tous les 6 mois
  - ⏳♻️ Acheter flotte > magnésium

---
---
---

## 🚧 WIP

Si travail en cours, indiquer les *notes & liens* ici

Rieng

---

## 💥 Tâches critiques

Bug clients majeurs, interruptions de service, etc.

Rieng

---

## ⚡️ Tâches rapides ✨

Indiquer ici les *tâches en dehors du flux général* (urgences, corrections process, trucs qui perturbent et doivent être fait, tâches ultra rapides, etc.)

Rieng

---

## ⏳ En attente

rieng

---

### ⏳🌱 Vérifications sur la longueur

rieng

---

## 🎯 A prioriser (quick dump)

Ordonner puis ranger dans le flux. Doit rester vide.

---

Tout est priorisé :)

---





PAS clean v


















---

1. blog
  1. [99 /  Bonus / Outils du Dev](https://docs.google.com/presentation/d/10XK2uOq3G0MnlsokNBBqV7VPkTIGprrhRxHnnX4Hrdo/edit#slide=id.g20f9d5d5cf0_0_0)
2. Ranger doc robots.txt dans un article de blog
  1. [google](https://developers.google.com/search/docs/crawling-indexing/robots/robots_txt?hl=fr)
  2. [bing](https://www.bing.com/webmasters/help/how-to-create-a-robots-txt-file-cb7c31ec)

---


---

### Perso 2

1. 👨‍⚕️ RDV dermato
2. 🍔 [Croissants high hydration dow](https://www.youtube.com/watch?v=GSlBVCbgFhE)

---


---

#### 🌱 Moins urgent

1. Toutes les musiques de salvatore ganacci
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
4. Peinture Chtulu
    1. [How to paint Extreme Light Sources - OSL tutorial](https://www.youtube.com/watch?v=c48UiPSBfcg)
    2. [INDESTRUCTIBLE Gaming Bases - Quick & Easy](https://www.youtube.com/watch?v=tRFfsAG-Yf8)
    3. Green gold pour le [grand ancien](https://www.youtube.com/watch?v=AgJqjIMd6k8)

---

