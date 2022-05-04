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

## 🚀 Priorisation, simple ⏩

Indiquer ici les *tâches à effectuer en priorité*

- Si besoin de focus, mettre une ou 2 tâches ici.
- Ne pas tout fourrer ici, *respecter la priorisation*, sinon tout est fait à l'arrache

Taf

1. 💥 21/05/2021 > Heberg picard > Basculer sur nouveau serveur & annuler

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
- ✅ Déclaration Auto entrepreneur
  - ⏳ Mai 2022
- ✅ Vérifier impôts sur espace / Dernière vérif 15/08/2021
  - ✅ Perso  / ✅ 04/05/22
  - ✅ Pro    / ✅ 04/05/22 (CFE réglé le 17/11/2021)
- ✅ Vérifier messages [Ameli](https://assure.ameli.fr/)
- ⏳ Maj locales / Environnement de dev / Dernière maj le 01/06/21
  - ✅ CHKDSK / Besoin de param `/f` ou [ne répare pas](https://docs.microsoft.com/fr-fr/windows-server/administration/windows-commands/chkdsk), `/r` également
    1. Invite de commande ou Powershell **en admin**
    2. `chkdsk c: /f /r` (et en fonction de vos disques.. && `chkdsk d: /f /r`, etc.)
    3. `>Blah blah besoin de redémarrer O/n` >> `O`
    4. Redémarrer / Attendre 5 ans et demi sauf si t'as un SSD/Nvme
  - ✅ Windaube
    - ✅ Update alakon
    - ✅ [.net](https://dotnet.microsoft.com/download) > Runtime
    - ✅ Panneau de conf > "Fichiers temporaires" > "Fichiers temporaires" (dans les catégories) > Supprimer
  - ✅ Drivers > [detection auto](https://www.touslesdrivers.com/index.php?v_page=29) > Lancer éxécutable, ça ouvre une page recap, et suivre liens dl
  - ✅ Firmware SSDs / Dépend du constructeur > Voir site officiel, avec un peu de chance logiciel auto alakon
    - (Mon ancien MSI) > [Sandisk ultra II](https://kb.sandisk.com/app/answers/detail/a_id/6053/~/ultra-3d-%7C-sandisk-ssd-plus-%28ssd%29-support-information)
      - Lancer (Sandisk) "Dashboard" / Firmware update automatique, et il préveitn avant. Nice
    - ✅ Dell support assist
    - ✅ Alienware update
  - ✅ Docker desktop (tray > icône > RC > Check for updates) / Attention, besoin de redémarrer a la main pour installation
  - ✅ Logiciels alakon
    - ✅ Ouvrir VScode > Auto update plugins etc.
    - ~~Filezilla~~ ✅ WinSCP, ✅ OBS, ✅ VLC, ESET, [Xnview classic (Pas MP)](https://www.xnview.com/fr/xnview/#downloads)
    - ✅ Powershell [sans prise de tête](https://aka.ms/powershell-release?tag=stable) > ~`PowerShell-VERSION-win-x64.msi`.
      - ( [Doc](https://docs.microsoft.com/fr-fr/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-7.1) )
    - ✅ Nvidia driver
  - ✅ Supprimer les fichiers temporaires
    - Exec > `temp` // Devrait ouvrir `~c:Windows\Temp`
    - Supprimer tout
  - ✅ WSL
    - Version Ubuntu
      - Si majeure, ré-effectuer [install-dev-env](https://github.com/youpiwaza/install-dev-env)
    - Packages & terminal

```bash
omz update
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade && sudo apt -y autoremove
```

- ⏳ Maj serveur, script maintenance
  - `98-maintenance.yml` & `sudo apt -y update && sudo apt --fix-broken install && sudo apt -y upgrade && sudo apt -y autoremove` & reboot si besoin
  - Maj Lapie HMAC
- ⏳ Maj budget couple
- ⏳ Serveur > Maj images
  - Maria DB
  - Nginx
  - WP
  - à compléter
- ✅ Téléphone
  - ✅ Maj de la base
  - ✅ Maj des applications
  - ⏳ Tous les 6 mois > reset usine
- ✅ Compléments alimentaires
  - ✅ Huile de foie de morue
  - ✅ Choline Inositol
  - ✅ Trucs foie/reins
  - ✅ Ginseng
  - ✅ Mix vitamine
  - ✅ Doc > vitamine D tous les 6 mois
- ✅ Tout est Versionné, pas de WIP qui traîne

---

## ⏳ En attente

1. ⏳ Bouchons oreilles thomann
   1. 1 semaine stock + délai livraison
2. ⏳ Acheter etiqueteuse [Dymo](https://www.google.com/search?q=Dymo&oq=Dymo&aqs=chrome..69i57.330j0j1&sourceid=chrome&ie=UTF-8)
   1. check en mai/juin ou pas lol
3. ⏳ Couteaux > acheter guide, pierres++ & cuir
   1. Libraison 4 & 5 mai

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

1. slurp cours [3wa](https://e.3wa.fr/user/profile.php?id=2257)
2. install-dev-env > docker-compose pour les principales technos : js & phpay
   1. Nginx + conteneur de gestion de conteneurs
3. 🔍 [tmux](https://nickjanetakis.com/blog/who-else-wants-to-boost-their-productivity-with-tmux)
4. 🔍 [keys remap](https://nickjanetakis.com/blog/remap-and-set-global-hotkeys-on-windows-10-with-auto-hotkey)

---

### Cryptor

⏳💩 Attente paiement avant reprise

🔗 Cf. [Statuts](https://docs.google.com/spreadsheets/d/1nvaJ1uGWcTgfAO7ej4-Bi0ReuN7Xmgou5HzcQ3qqLXo/edit#gid=1341993327)

---

### Serveur

1. ✅ Récupérer les données de l'ancien pc & mieux versionner
2. ✅ Réinstaller la connexion ssh + tests
3. 🚀 Relire les rôles 10 & 20
   1. `ansible-install-web-server\ansible\100---hello--masamune--fr----README--generated.md` > confusion entre nginx et wp > a cleaner (variable techno utilisée ou chp)
4. ⏳ Backups sites clients
   1. ✅ sophie berberian
   2. 💥 Régénerer rôles afin d'avoir les playbooks de sauvegarde
      1. 🚀 Récupération des playbooks actuellement utilisés & vérifications avant
         1. cf. `ansible-install-web-server\commandes-backup-volumes-a-la-maing_secret.md`
         2. cf. `ansible-install-web-server\ansible\tmp\_old`
         3. cf. `ansible-install-web-server\ansible\roles\stack-web-nginx--generate-playbooks\vars\clients\lapie\champagne-didier-lapie--com\`
         4. `ansible-install-web-server\ansible\roles\stack-web-wordpress--generate-playbooks\vars\clients`
      2. Monter les rôles générés sur les devs des clients
      3. champagne didier lapie
      4. ald infographie
      5. Virer (sous)dossiers alakon
         1. /tmp/old, etc.
         2. ansible-install-web-server/ansible/roles/stack-web-nginx--generate-playbooks/vars
         3. ansible-install-web-server/ansible/roles/stack-web-wordpress--generate-playbooks/vars
5. ⏳ Email clients interruption de service
   1. ✅ template
6. Mettre à jour le serveur
   1. Forcer redémarrage > 52
   2. Maintenance > 98
7. Re-prioriser les tâches restantes du serveur
8. 💩 KO role > sftp-create-user
9. 💩 Renommer forge a nginx en forge tutum, puis faire un projet dédié nginx
10. ⏳ Lapie HMAC auto
11. Si tout est bon sur repo secret > virer `/clients` qui est redondant
12. Passage à ubuntu 22
13. Ubuntu 22 sur dockerhub
14. Lint done : ansible-install-web-server > README.MD
15. [WP + nginx](https://wordpress.org/support/article/nginx/)
16. ansible template, au lieu de remplacer variables > [block_start_string](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/template_module.html#parameter-block_start_string)
17. Ansible convenience
    1. Clean templating, variable [deprecated ansible_managed](https://docs.ansible.com/ansible/2.4/intro_configuration.html#ansible-managed)
        1. [?](https://docs.ansible.com/ansible/latest/reference_appendices/config.html#default-managed-str)
    2. [ansible prompt](https://docs.ansible.com/ansible/latest/user_guide/playbooks_prompts.html)
18. Opti script maintenance
    1. Ajouter maj OMZ ZSH
19. Installer webmin plutot que grafana & autres
20. Wordpress dev prod > réutiliser /generated/var files
21. Faire une grosse repasse sur les index de projet il manque plein de vars
22. Conteur **netdata** a la place de grafana
23. Génération d'un nouveau site OU wp > doc identifiant à la racine (actuellement uniquement dans /generated/)
24. wp > identifiants > ajouter url wp-admin
25. BUG: génération des fichiers de sites > prefixe `200-` pas utilisé partout
26. 🚀 Bind volumes pour les fichiers /www des sites, sur les sftp créés
    1. A la mano voir si ça marche, sinon se pendre
    2. Automatiser
27. `/home/singed_the_docker_peon_9f3eqk4s9/configs/masamune/hello--masamune--fr` wtf is that
28. harmoniser builder guy > tout THE_BUiLDER_GUY, idem autres XXX_GUY
29. Tutum > remplacer par nginx
    1. Faire tourner déjà ca serait bien, go ctrl + f "curated"
    2. Utiliser vars d'environnement pour refaire un tutum mayzon: image + nom conteneur
    3. Serveur normal & serveur php basique pour les sites non wp
    4. Opti [Nginx](https://hub.docker.com/_/nginx) / test-nginx.masamune.fr
       1. 🔍 [Video configuration](https://www.youtube.com/watch?v=C5kMgshNc6g)
       2. Tune server for [nginx performance](https://www.nginx.com/blog/10-tips-for-10x-application-performance/)
       3. [+1](https://blog.monitis.com/blog/6-best-practices-for-optimizing-your-nginx-performance/)
30. Bitnami
    1. [Github issues](https://github.com/bitnami/bitnami-docker-mysql/issues/79#issuecomment-545477842) > Variable d'env afin d'augmenter le debug des conteneurs bitnami ! >> raisons explicites sur le problème de boot du conteneur
    2. Gestion notes dans ansible-install-web-server/ansible/203-setup-wordpress-lapie_secret.yml
    3. Testay avec surcharge de conf via config: voir si ca boot avec la bonne conf
    4. Lourder si serveurs web classique stabilité 100%, +1 speed
    5. Activer modules php
    6. Http 2/3
31. Gestion des mails propre
    1. Connexion au serveur SMPT du serveur ? cf. utils-emails
    2. [Conteneur postfix ?](https://hub.docker.com/_/postfixadmin)
    3. Ajout SPF/DKIM/DMARC
    4. Maj lapie & nonore
32. Maj conteneur bitnami/wordpress
33. Cleaner / Relancer clients actuels
    1. Lapie
       1. Cleaner au niveau du serveur dashed-uri > .com ou .fr
    2. Nonore
       1. (wp généré et lancement depuis ansible), Pour le moment c'est un yml lancé a l'arrache sur le serveur
    3. Backups volumes
       1. Maj ansible-install-web-server/commandes-backup-volumes-a-la-maing_secret.md (dashed notation)
       2. (normalement d'ici la les roles de backups seront générés auto :3)
       3. Backup
34. Migration serveur
    1. Lister
       1. Technos
       2. 📌📌📌📌📌📌📌 Fichiers
       3. BDD / Exports WordPress
       4. Basculer

#### Suite Serveur / post migration

1. Gestion des backups
    1. Ajout au CRON
    2. Envoi vers serveur de backup + rotation/sauvegarde incrémentielle
2. Mise en place d'une admin SQL > [phpmyadmin](https://hub.docker.com/_/phpmyadmin)
    1. Objectif 1 : Go nginx sur pma-test-wordpress.masamune.fr
        1. 🚀 .yml indépendant
        2. .yml de test-wordpress
    2. Objectif 2 : Go pma sur pma-test-wordpress.masamune.fr
       1. ^ Check DNS
3. Monitoring > MOD: 4-setup-core-services.yml
    1. Alternative ? [traefik pilot](https://doc.traefik.io/traefik-pilot/)
    2. Alerte si CPU/RAM > 75%
    3. Alerte si space disque libre < 20%
    4. Checker ce qui prend de la place sur le disque ~80Go ? 13% de 450 > `docker system df -v` ; cf. backup des volumes
4. Prévoir dev & prod > 1 seul script mais url change, même users & pass
    1. Utiliser docker-compose.override.yml ? [Bonnes pratiques docker/compose](https://nickjanetakis.com/blog/best-practices-around-production-ready-web-apps-with-docker-compose)
       1. Variables d'environnement dans DC
    2. Check ansible > vars d'environnement afin de maj dev. ou prod
    3. Gestion dev/prod : 1 seul fichier
    4. ENV vars ++
    5. Volumes en fonction de l'environnement ¤_¤
5. Tester conteneurs de serveurs (facilité/stabilité/vitesse/http3)
    1. Need modules de cache php activés
    2. HTTP 2/3 serait un vrai plus
    3. [Apache](https://hub.docker.com/_/httpd) / test-httpd.masamune.fr
    4. [Caddy](https://hub.docker.com/_/caddy) / test-caddy.masamune.fr
    5. Litespeed : [open](https://hub.docker.com/r/litespeedtech/openlitespeed) / [payant ?](https://hub.docker.com/r/litespeedtech/litespeed)
       1. 2-3 trucs/plugins a regarder en plus pour WP : [doc](https://www.litespeedtech.com/open-source) & [site dédié](https://lscache.io/)
       2. test-litespeed.masamune.fr
    6. 🌱 Chaque serveur > Tester WP (install via wp-cli ?)

---

### Lapie > Finaliser

1. Cleaner github dedié > client/url-site/
2. Lapie > Ranger chartes graphiques & lapie-web
3. Charte graphique > Faire les TODOs
4. 🚚(shame) > Lapie kek.php (Crédit agricole > génération d'un fichier kek.php à la racine lors de l'insertion de clé HMAC > détruit au reboot du conteneur)
5. Lapie, retours SEO
6. Lapie > 🚚([Statut](https://docs.google.com/spreadsheets/d/1zZUT0F4XMQyVAFbP7ihACnRz10pmog5KoYlcaiXOGIk/edit#gid=0))
7. ~Lapie > Maj traefik pour redirection www. > faire des tests alakon sur NDD masa avant, cf. critique
      1. Maj Ansible
8. 🚚(shame) Accès fichiers bloqués conteneur bitnamiwp, modules php, passer en http2/3

---

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

1. Trouver logiciel budget couple
2. 🚀 Musiques taf & portable
3. ✅ concert 10/06 maximum the hormone
      1. 🚀 trains, et utiliser [reductions](https://mail.google.com/mail/u/0/#inbox/KtbxLxgZZVNcfFNSbtrStGMpWXmfCKPsJB)
4. Blog groupe metal que j'aime bieng ou pas en concert
5. Films
   1. Ciné
      1. Nick cage
      2. Dernier Cronenberg
      3. Everything everywhere all at once
   2. death of dick long
6. Export photos tel & maj drive
7. Peinture Chtulu
    1. [How to paint Extreme Light Sources - OSL tutorial](https://www.youtube.com/watch?v=c48UiPSBfcg)
    2. [INDESTRUCTIBLE Gaming Bases - Quick & Easy](https://www.youtube.com/watch?v=tRFfsAG-Yf8)
    3. Green gold pour le [grand ancien](https://www.youtube.com/watch?v=AgJqjIMd6k8)
8. [Patinoire](https://mail.google.com/mail/u/0/#inbox/FMfcgzGmvLQjSdlzHqNgpnCFgHjXWZlW)
9. Pourrir la bred sur les réseaux
10. Retrouver Permis conduire
11. DL vidéos WTF youtoob
12. [Changement propriétaire chatte](https://mail.google.com/mail/u/0/#inbox/FMfcgzGllCcNJCZHqcjqlkNJhlNFzwZC)
13. Faire article réparation/optimisation de pc
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
