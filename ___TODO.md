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

Taf

1. Envoyer mail clients maj serveur & possibles interuptions de services
2. ✅ Clôture cryptor
   1. ✅ Boilerplate rupture de contrat
   2. ✅ Doc de fin de contrat a signer + signature electronique
      1. ⏳ Signature
   3. ✅ Facture
      1. ⏳ Règlement
3. Environnement de dev local clean
   1. Gestion de containers via portainer (actuellement en extension sur docker desktop)
4. 💥 21/05/2021 > Heberg picard > Basculer sur nouveau serveur & annuler

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
- ✅ Déclaration Auto entrepreneur
  - ⏳ Mai 2022
- ✅ Vérifier impôts sur espace / Dernière vérif 15/08/2021
  - ✅ Perso  / ✅ 23/05/22
  - ✅ Pro    / ✅ 23/05/22 (CFE réglé le 17/11/2021)
- ✅ Vérifier messages [Ameli](https://assure.ameli.fr/)
- ✅ Maj locales / Environnement de dev / Dernière maj le 01/06/21
  - ⏩ CHKDSK / Besoin de param `/f` ou [ne répare pas](https://docs.microsoft.com/fr-fr/windows-server/administration/windows-commands/chkdsk), `/r` également
    1. Invite de commande ou Powershell **en admin**
    2. `chkdsk c: /f /r` (et en fonction de vos disques.. && `chkdsk d: /f /r`, etc.)
    3. `>Blah blah besoin de redémarrer O/n` >> `O`
    4. Redémarrer / Attendre 5 ans et demi sauf si t'as un SSD/Nvme
  - ✅ Windaube
    - ✅ Update alakon
    - ⏳ [.net](https://dotnet.microsoft.com/download) > Runtime
    - ⏳ Panneau de conf > "Fichiers temporaires" > "Fichiers temporaires" (dans les catégories) > Supprimer
  - ✅ Drivers > [detection auto](https://www.touslesdrivers.com/index.php?v_page=29) > Lancer éxécutable, ça ouvre une page recap, et suivre liens dl
  - ✅ Firmware SSDs / Dépend du constructeur > Voir site officiel, avec un peu de chance logiciel auto alakon
    - ✅ Dell support assist
    - ✅ Alienware update
  - ✅ Docker desktop (tray > icône > RC > Check for updates) / Attention, besoin de redémarrer a la main pour installation
  - ⏳ Logiciels alakon
    - ✅ Ouvrir VScode > Auto update plugins etc.
    - ~~Filezilla~~ ✅ WinSCP, ✅ OBS, ✅ VLC, ESET, [Xnview classic (Pas MP)](https://www.xnview.com/fr/xnview/#downloads)
    - ⏳ Powershell [sans prise de tête](https://aka.ms/powershell-release?tag=stable) > ~`PowerShell-VERSION-win-x64.msi`.
      - ( [Doc](https://docs.microsoft.com/fr-fr/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-7.1) )
    - ✅ Nvidia driver
  - ✅ Supprimer les fichiers temporaires
    - Exec > `temp` // Devrait ouvrir `~c:Windows\Temp`
    - Supprimer tout, Ignorer ceux utilisés
  - ⏳ WSL
    - Version Ubuntu
      - Si majeure, ré-effectuer [install-dev-env](https://github.com/youpiwaza/install-dev-env)
    - Packages & terminal

```bash
omz update
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade && sudo apt -y autoremove && docker system prune -af
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
- ⏳ Téléphone
  - ⏳ Maj de la base
  - ⏳ Maj des applications
  - ⏳ Tous les 6 mois > reset usine
- ✅ Compléments alimentaires
  - ✅ Huile de foie de morue
  - ✅ Choline Inositol
  - ✅ Trucs foie/reins
  - ✅ Ginseng / "Super ginko"
    - ⏳ Attente livraison
  - ✅ Mix vitamine
  - ✅ Doc > vitamine D tous les 6 mois
- ⏳ Tout est Versionné, pas de WIP qui traîne

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

1. slurp cours [3wa](https://e.3wa.fr/user/profile.php?id=2257)
2. install-dev-env > docker-compose pour les principales technos : js & phpay
   1. Nginx + conteneur de gestion de conteneurs
3. 🔍 [tmux](https://nickjanetakis.com/blog/who-else-wants-to-boost-their-productivity-with-tmux)
4. 🔍 [keys remap](https://nickjanetakis.com/blog/remap-and-set-global-hotkeys-on-windows-10-with-auto-hotkey)

---

### Serveur

#### 🚀 Terminer les bases (sftp, adminer, mails) + dev/prod + Lapie secrets

1. 🚀 Rôle accès sftp
   1. 📌 Tests
      1. 🔍 Image serveur sftp avec volumes & clés ssh [atmoz](https://hub.docker.com/r/atmoz/sftp)
      2. ✅ Test sans volume
      3. 🚀 Test avec volume bind
      4. Test avec volume bind + named volume
2. Rôle accès bdd
   1. adminer, cf. cryptor
3. Gestion des mails propre
    1. Connexion au serveur SMPT du serveur ? cf. utils-emails
    2. [Conteneur postfix ?](https://hub.docker.com/_/postfixadmin)
    3. Ajout SPF/DKIM/DMARC
    4. Maj lapie & nonore
4. Prévoir dev & prod > 1 seul script mais url change, même users & pass
    1. Réutiliser `/generated/vars` files ? (WP)
    2. Utiliser docker-compose.override.yml ? [Bonnes pratiques docker/compose](https://nickjanetakis.com/blog/best-practices-around-production-ready-web-apps-with-docker-compose)
       1. Variables d'environnement dans DC
    3. Check ansible > vars d'environnement afin de maj dev. ou prod
    4. Gestion dev/prod : 1 seul fichier
    5. ENV vars ++
    6. Volumes en fonction de l'environnement ¤_¤
5. ⏳ Lapie HMAC auto
    1. Lapie kek.php (Crédit agricole > génération d'un fichier kek.php à la racine lors de l'insertion de clé HMAC > détruit au reboot du conteneur)

#### Régénérer les clients existants

##### Sophie berberian

1. ✅ Créer un fichier de forge dédié dev, avec le bon chemin vers leurs variables
2. ✅ Génerer rôle dev
3. Mettre en place le dev afin de vérifier le bon fonctionnement
   1. Backup prod en local
   2. Injection sur dev host
4. Créer un fichier de forge dédié prod, avec le bon chemin vers leurs variables
5. Générer rôle prod
   1. Backup host & local
   2. Migrer la prod
6. Maj secrets

##### Champagne didier lapie

📝👴 *Cleaner au niveau du serveur dashed-uri > .com ou .fr*

💾👴 *Sauvegarde wp db & files faites à partir de backup à la main, stockés sur serveur dans /home/THE_DOCKER_GUY/backups/volumes/2022_temp_backups_anciens_yml_avant_normalisation
et téléchargées dans C:\Users\masam\Documents\_dev\Backups serveurs*

👷 Faire attention aux noms de volumes

🧠 Backup a la main avec les anciennes commandes puis regen stack puis injection en modifiant les noms d'archives injectées

1. Créer un fichier de forge dédié dev, avec le bon chemin vers leurs variables
   1. 💥 Réutiliser fichiers de variables (à rajouter en amont dans /generated)
      1. `C:\Users\masam\Documents\_dev\Backups serveurs\lapie old access and yml`
   2. 💥 Maj les ressources allouées aux WordPress
2. Génerer rôle dev
3. Mettre en place le dev afin de vérifier le bon fonctionnement
   1. Backup host & local
4. Créer un fichier de forge dédié prod, avec le bon chemin vers leurs variables
5. Générer rôle prod
   1. Backup host & local
   2. Migrer la prod
6. Maj secrets
   1. ranger cle hmac pour e commerce (en local uniquement pour le moment)

##### ALD infographie

📝👴 *(wp généré et lancement depuis ansible), Pour le moment c'est un yml lancé a l'arrache sur le serveur*

💾👴 *Sauvegarde wp db & files faites à partir de backup à la main, stockés sur serveur dans /home/THE_DOCKER_GUY/backups/volumes/2022_temp_backups_anciens_yml_avant_normalisation
et téléchargées dans C:\Users\masam\Documents\_dev\Backups serveurs*

👷 Faire attention aux noms de volumes

🧠 Backup a la main avec les anciennes commandes puis regen stack puis injection en modifiant les noms d'archives injectées

1. ALD infographie / nonore > .yml stocké uniquement sur serveur !
   1. Faire diff avec `C:\Users\masam\Documents\_dev\Backups serveurs\nonore old yml`
2. Créer un fichier de forge dédié dev, avec le bon chemin vers leurs variables
3. Génerer rôle dev
4. Mettre en place le dev afin de vérifier le bon fonctionnement
   1. Backup host & local
5. Créer un fichier de forge dédié prod, avec le bon chemin vers leurs variables
6. Générer rôle prod
   1. Backup host & local
   2. Migrer la prod
7. Maj secrets

#### Faire la mise à jour du serveur vers ubuntu 22

1. Backups sites clients
   1. sophie berberian
   2. champagne didier lapie
   3. ald infographie
2. ⏳ Email clients interruption de service
    1. ✅ template
3. Mettre à jour le serveur
    1. Forcer redémarrage > 52
    2. Maintenance > 98
4. Vérifications sites clients toujours en place
   1. Restaurer backup si besoin

#### Faire la mise à jour des wordpress

📌 Possibilité de tester sur le dev avant

1. sophie berberian
2. champagne didier lapie
3. ald infographie

#### Passer Tutum en Nginx + php basique

1. Renommer forge a nginx en forge tutum, puis faire un playbook dédié nginx
    1. Faire conteneur en local pour tester installation & configuration simple
       1. Récupérer config faite pour cryptor
    2. Serveur normal & serveur php basique pour les sites non wp
    3. Opti [Nginx](https://hub.docker.com/_/nginx) / test-nginx.masamune.fr
       1. 🔍 [Video configuration](https://www.youtube.com/watch?v=C5kMgshNc6g)
       2. Tune server for [nginx performance](https://www.nginx.com/blog/10-tips-for-10x-application-performance/)
       3. [+1](https://blog.monitis.com/blog/6-best-practices-for-optimizing-your-nginx-performance/)

#### Installer le monitoring

Commencer via 99 crafts puis MOD: 4-setup-core-services.yml

1. Installer webmin ou **netdata** plutot que grafana & autres
   1. Swarm WebUi Portainer
      1. [doc](https://portainer.readthedocs.io/en/stable/deployment.html)
      2. [DS rocks](https://dockerswarm.rocks/portainer/)
   2. Tester en local
2. Alerte si CPU/RAM > 75%
3. Alerte si space disque libre < 20%

#### Migrer ancien serveur

1. Migration de l'ancien serveur, pour chaque client hébergé, lister
    1. Technos
    2. 📌📌📌📌📌📌📌 Fichiers
    3. BDD / Exports WordPress
    4. Basculer

#### Cleaner avant de poursuivre le projet

1. Tester Nginx + WordPress, sans bitnami, [cf.](https://wordpress.org/support/article/nginx/)
   1. Voir pour virer bitnami en vrai c'est juste pas clair au niveau de la gestion
   2. Voir pour ajouter REDIS > meilleures perfs si grosses données ? existe en image docker
2. ansible template, au lieu de remplacer variables > [block_start_string](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/template_module.html#parameter-block_start_string)
3. Opti script maintenance
    1. Ajouter maj OMZ ZSH
4. wp > identifiants > ajouter url wp-admin
5. `/home/singed_the_docker_peon_9f3eqk4s9/configs/masamune/hello--masamune--fr` wtf is that
6. Process récurrent de Maj des images clients

#### Suite Serveur / post migration

1. Activer le [Debug Mode de docker](https://docs.docker.com/engine/reference/commandline/dockerd/#daemon-configuration-file)
2. ⏳📌 `/var/log/auth.log` > [audit: backlog limit exceeded](https://aws.amazon.com/fr/premiumsupport/knowledge-center/troubleshoot-audit-backlog-errors-ec2/)
   1. Augmentation de la valeur de 1280 à 8192 via `sudo nano /etc/audit/rules.d/audit.rules PUIS sudo service auditd restart VERIF sudo auditctl -s`
   2. Maj de `/roles/docker-installation/tasks/docker-bench-security.yml` &`/roles/docker-installation/templates/auditd-audit.rules.j2`
3. Gestion des backups
    1. Ajout au CRON
    2. Envoi vers serveur de backup + rotation/sauvegarde incrémentielle
4. Checker ce qui prend de la place sur le disque ~80Go ? 13% de 450 > `docker system df -v` ; cf. backup des volumes
   1. 💥 Tâche ponctuelle clean logs (en attendant automatisation > traefik.log > 200514-traefik.log)
5. Ansible convenience
    1. Clean templating, variable [deprecated ansible_managed](https://docs.ansible.com/ansible/2.4/intro_configuration.html#ansible-managed)
        1. [?](https://docs.ansible.com/ansible/latest/reference_appendices/config.html#default-managed-str)
    2. [ansible prompt](https://docs.ansible.com/ansible/latest/user_guide/playbooks_prompts.html)
6. Containers [Healtcheck](https://blog.sixeyed.com/docker-healthchecks-why-not-to-use-curl-or-iwr/)
7. Pagespeed optimisations w. vanilla websites
8. Tester conteneurs de serveurs (facilité/stabilité/vitesse/http3)
    1. Need modules de cache php activés
    2. Nginx
    3. [Apache](https://hub.docker.com/_/httpd) / test-httpd.masamune.fr
    4. [Caddy](https://hub.docker.com/_/caddy) / test-caddy.masamune.fr
    5. Litespeed : [open](https://hub.docker.com/r/litespeedtech/openlitespeed) / [payant ?](https://hub.docker.com/r/litespeedtech/litespeed)
       1. 2-3 trucs/plugins a regarder en plus pour WP : [doc](https://www.litespeedtech.com/open-source) & [site dédié](https://lscache.io/)
       2. test-litespeed.masamune.fr
    6. 🌱 Chaque serveur > Tester WP (install via wp-cli ?)
9. [Varnish cache](https://varnish-cache.org/)
10. Docker certification [175€](https://success.docker.com/certification)
11. Veille securité
    1. [Docker Production Best Practices from Bret Fisher at DockerCon](https://www.youtube.com/watch?v=V4f_sHTzvCI)
    2. [Container security free pdf](http://containersecurity.tech/)

---

### Lapie > Finaliser

1. Cleaner github dedié > client/url-site/
2. Lapie > Ranger chartes graphiques & lapie-web
3. Charte graphique > Faire les TODOs
4. Lapie, retours SEO
5. Lapie > [Statut](https://docs.google.com/spreadsheets/d/1zZUT0F4XMQyVAFbP7ihACnRz10pmog5KoYlcaiXOGIk/edit#gid=0)
6. ~Lapie > Maj traefik pour redirection www. > faire des tests alakon sur NDD masa avant, cf. critique
      1. Maj Ansible

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
9. Retrouver Permis conduire
10. DL vidéos WTF youtoob
11. [Changement propriétaire chatte](https://mail.google.com/mail/u/0/#inbox/FMfcgzGllCcNJCZHqcjqlkNJhlNFzwZC)
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
