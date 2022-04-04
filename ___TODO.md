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
- ✅🧠 Copier coller historique > Activer l'hitorique
  - *windows + V*
- Tétrachiée de nouveaux plugins VSCode
  - ✅ Better comments
  - Bookmarks
  - 🚀🧠 changeCase
    - *Ctrl Shift X* > Choisir
    - *Ctrl Shift W* > Inverser
  - Code spell checker
  - TO DO Tree
  - 🧠 "Toggle quotes"
    - *Ctrl + ²*, curseur après la première de la paire de quotes à changer
  - polacode > joli print de code

## 🚀 Priorisation, simple ⏩

Indiquer ici les *tâches à effectuer en priorité*

- Si besoin de focus, mettre une ou 2 tâches ici.

1. ✅ Lapie > Changer image accueil > ratafia

Courant, puis taf

1. 🚀 Versionner TODOs
2. Virer Done
3. Versionner TODOs
4. Devis & factures PB Modélisme
5. Tâches récurrentes
6. 💥 Cleaner TODOs
   1. Versionner TODOs
7. Réinstaller environnement de dev sur nouveau pc
   1. WSL
   2. Docker desktop

Trucs **persos**

1. ✅ Régulariser impots janvier 2022 pour décembre 2021
   1. ✅ Demande de régularisation
   2. ✅ Virement ponctuel de régularisation
   3. ✅ Confirmation prise en compte
   4. ✅ Confirmation pas de frais de retard
2. ⏳⏳ Changement de banque
   1. ✅ Ouverture de compte
   2. ✅ CB
   3. ✅ Provisionner
   4. ✅ Transfert des opérations courantes & soldes restants
   5. ✅ Message à l'ancienne banque pour résiliation
      1. ✅ Envoi lettre recommandée, en attente de bonne reception, envoyé le 04/03/2022
   6. ✅ Dernière facture 26D > Transmettre nouveau RIB
   7. ✅ Paiement AE
   8. ✅ Maj factures AE
   9. ✅ Maj bankin
   10. ✅ Récupérer IBANs enregistrés
   11. ✅ Maj amazon
   12. ✅ Maj Paypal
   13. ✅ Maj paiement le bon coin
   14. ✅ Analyser opérations en cours sur compte courant BRED et tout flinguer !!!
       1. ✅ Assurance Alan
       2. ✅ Popa
       3. ✅ Deliveroo
       4. ✅ Abo piscine
       5. ✅ Forfait tel sosh
       6. ✅ Urssaff
       7. ✅ OVH / via paypal
       8. ✅ SYS / via paypal
       9. ✅ Ameli : Vérifier ou refaire, service indisponible -_-
       10. ✅ Impôts
           1. ✅👤 Perso / Pas d'IBAN ou de mandat pour le moment
           2. ✅💩💩💩 Pro / Compte courant boursorama, à passer sur compte pro quand créé, cf ci-dessous
   15. ✅💩💩💩 Retour de l'autre connard > souscription à une autorisation de découvert au lieu de résiliation
       1. ✅  YAVAI PAS BESOIN LAUL
   16. ⏳ Vérifier clôture encore reportée par l'autre sac a merde
3. 💩 Compte Pro boursorama / C'est mort, whatever
4. ✅ Remplacement tireuse à bière
   1. ✅ Laver, étiquettes, paquet
   2. ✅ Renvoyer à SB via mondial relay
   3. ✅ Reçu & good
5. 🚀 Musiques taf & portable
6. Paiement syndic
7. Retrouver Permis conduire
8. Maj document de base CdC à partir de celui de PB Modelisme
9. DL vidéos WTF youtoob
10. Changement propriétaire chatte
11. Faire article réparation/optimisation de pc
    1. [hey](https://www.drivereasy.com/knowledge/100-disk-usage-windows-10-fixed/)
    2. [hoy](https://www.makeuseof.com/tips-fix-100-disk-usage-improve-windows-performance/)
12. Faire article maintenance PC
13. double authentification OVH manager
14. Mettre à jour CV !
15. Rdv médecins
    1. Ophtalmo
    2. Cardiolog0ue
    3. Oreillologiste
16. CPF > Langage des signes / Amazon AWS / Jenkins git hooks
17. !site perso > cours particuliers code > 50€ heure (+, compter impôts)

Trucs **taf**

1. slurp cours [3wa](https://e.3wa.fr/user/profile.php?id=2257)

Trucs pour la **migration du serveur**

1. Installer webmin plutot que grafana & autres
2. Wordpress dev prod > réutiliser /generated/var files
3. Faire une grosse repasse sur les index de projet il manque plein de vars
4. Conteur netdata a la place de grafana
5. Génération d'un nouveau site OU wp > doc identifiant à la racine (actuellement uniquement dans /generated/)
6. wp > identifiants > ajouter url wp-admin
7. BUG: génération des fichiers de sites > prefixe `200-` pas utilisé partout
8. 🚀 Bind volumes pour les fichiers /www des sites, sur les sftp créés
   1. A la mano voir si ça marche, sinon se pendre
   2. Automatiser
9. `/home/singed_the_docker_peon_9f3eqk4s9/configs/masamune/hello--masamune--fr` wtf is that
10. harmoniser builder guy > tout THE_BUiLDER_GUY, idem autres XXX_GUY
11. Tutum > remplacer par nginx
    1. Faire tourner déjà ca serait bien, go ctrl + f "curated"
    2. Utiliser vars d'environnement pour refaire un tutum mayzon: image + nom conteneur
    3. Serveur normal & serveur php basique pour les sites non wp
    4. Opti [Nginx](https://hub.docker.com/_/nginx) / test-nginx.masamune.fr
       1. 🔍 [Video configuration](https://www.youtube.com/watch?v=C5kMgshNc6g)
       2. Tune server for [nginx performance](https://www.nginx.com/blog/10-tips-for-10x-application-performance/)
       3. [+1](https://blog.monitis.com/blog/6-best-practices-for-optimizing-your-nginx-performance/)
12. Bitnami
    1. [Github issues](https://github.com/bitnami/bitnami-docker-mysql/issues/79#issuecomment-545477842) > Variable d'env afin d'augmenter le debug des conteneurs bitnami ! >> raisons explicites sur le problème de boot du conteneur
    2. Gestion notes dans ansible-install-web-server/ansible/203-setup-wordpress-lapie_secret.yml
    3. Testay avec surcharge de conf via config: voir si ca boot avec la bonne conf
    4. Lourder si serveurs web classique stabilité 100%, +1 speed
    5. Activer modules php
    6. Http 2/3
13. Gestion des mails propre
    1. Connexion au serveur SMPT du serveur ? cf. utils-emails
    2. [Conteneur postfix ?](https://hub.docker.com/_/postfixadmin)
    3. Ajout SPF/DKIM/DMARC
    4. Maj lapie & nonore
14. Maj conteneur bitnami/wordpress
15. Cleaner / Relancer clients actuels
    1. Lapie
       1. Cleaner au niveau du serveur dashed-uri > .com ou .fr
    2. Nonore
       1. (wp généré et lancement depuis ansible), Pour le moment c'est un yml lancé a l'arrache sur le serveur
    3. Backups volumes
       1. Maj ansible-install-web-server/commandes-backup-volumes-a-la-maing_secret.md (dashed notation)
       2. (normalement d'ici la les roles de backups seront générés auto :3)
       3. Backup
16. Migration serveur
    1. Lister
       1. Technos
       2. 📌📌📌📌📌📌📌 Fichiers
       3. BDD / Exports WordPress
       4. Basculer

Suite **Serveur** post migration

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
    1. ✅ NDDs
       1. Need modules de cache php activés
       2. HTTP 2/3 serait un vrai plus
    2. [Apache](https://hub.docker.com/_/httpd) / test-httpd.masamune.fr
    3. [Caddy](https://hub.docker.com/_/caddy) / test-caddy.masamune.fr
    4. Litespeed : [open](https://hub.docker.com/r/litespeedtech/openlitespeed) / [payant ?](https://hub.docker.com/r/litespeedtech/litespeed)
       1. 2-3 trucs/plugins a regarder en plus pour WP : [doc](https://www.litespeedtech.com/open-source) & [site dédié](https://lscache.io/)
       2. test-litespeed.masamune.fr
    5. 🌱 Chaque serveur > Tester WP (install via wp-cli ?)

### Sinon, priorisation classique

1. Tâches récurrentes
2. Tâches en attente
3. Tâches critiques
4. Tâches WIP
5. Tâches rapides
6. Autres fichiers TODO

## ♻️ Tâches récurrentes ♻️

Tâches à *vérifier au moins une fois par semaine*, afin d'éviter un bordel plus tard/exponentiel

- ⏳Déplacer les terminés ✅ à chaque début de semaine dans done.md
- 💩 Déplacer les TODO 🌱 dans _TODO_shame.md
- ⏳ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur ⏳ mails, ⏳ edt portable, ⏳ favoris, ⏳ bureau. Si possible description + lien.
- ⏳ Nettoyer le fichier __TODO
  - ⏳ Status
  - ⏳ Ce fichier > ### Shame
    - ⏳ Ranger dans fichiers TODO correspondant
    - ⏳ Prioriser
- ⏳ Virer ce qui traine
  - ⏳ sur le bureau
  - 💩 dans le dossier _shame du bureau
  - 💩 Lel (local)/Mes documents/_dev/_shame
  - ⏳ Vider corbeille
  - ⏳ Vider téléchargements
  - ⏳ Dans les mails
- ⏳ Déplacer veille onglets dans TODO_veille
- 💩 Ranger DD boulot
- 💩 Lel Veille / Un truc par semaine, genre le vendredi aprem, a githuber
- ✅ Déclaration Auto entrepreneur
  - ✅ Mars 2022
- ⏳ Vérifier impôts sur espace / Dernière vérif 15/08/2021
  - ⏳ Perso / ✅ 16/03/22
  - ⏳ Pro / ✅ 16/03/22 (CFE réglé le 17/11/2021)
- ⏳ Maj locales / Environnement de dev / Dernière maj le 01/06/21
  - ⏳ CHKDSK / Besoin de param `/f` ou [ne répare pas](https://docs.microsoft.com/fr-fr/windows-server/administration/windows-commands/chkdsk)
  - `/r` ?
    1. Invite de commande ou Powershell **en admin**
    2. `chkdsk c: /f /r` (et en fonction de vos disques.. && `chkdsk d: /f /r`, etc.)
    3. `>Blah blah besoin de redémarrer O/n` >> `O`
    4. Redémarrer / Attendre 5 ans et demi sauf si t'as un SSD
  - ⏳ Windaube update
    - [.net](https://dotnet.microsoft.com/download)
    - Panneau de conf > "Fichiers temporaires" > "Fichiers temporaires" (dans les catégories) > Supprimer
  - ⏳ Drivers > [detection auto](https://www.touslesdrivers.com/index.php?v_page=29) > Lancer éxécutable, ça ouvre une page recap, et suivre liens dl
  - ⏳ Firmware SSDs / Dépend du constructeur > Voir site officiel, avec un peu de chance logiciel auto alakon
    - [Sandisk ultra II](https://kb.sandisk.com/app/answers/detail/a_id/6053/~/ultra-3d-%7C-sandisk-ssd-plus-%28ssd%29-support-information)
    - Lancer (Sandisk) "Dashboard" / Firmware update automatique, et il préveitn avant. Nice
  - ⏳ Docker desktop (tray > icône > RC > Check for updates) / Attention, besoin de redémarrer a la main pour installation
  - ⏳ Logiciels alakon
    - Ouvrir VScode > Auto update plugins etc.
    - ~~Filezilla~~ WinSCP, OBS, VLC, ESET, [Xnview classic (Pas MP)](https://www.xnview.com/fr/xnview/#downloads)
    - Powershell [sans prise de tête](https://aka.ms/powershell-release?tag=stable) > ~`PowerShell-VERSION-win-x64.msi`.
    - Nvidia driver
      - ( [Doc](https://docs.microsoft.com/fr-fr/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-7.1) )
  - ⏳ Supprimer les fichiers temporaires
    - Exec > `temp` // Devrait ouvrir `~c:Windows\Temp`
    - Supprimer tout
  - ⏳ WSL
    - Version Ubuntu
      - Si majeure, ré-effectuer [install-dev-env](https://github.com/youpiwaza/install-dev-env)
    - Packages & terminal

```bash
omz update
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull && sudo apt update && sudo apt --fix-broken install && sudo apt -y upgrade
```

- ⏳ Maj serveur, script maintenance
  - `98-maintenance.yml` & `sudo apt -y update && sudo apt --fix-broken install && sudo apt -y upgrade` & reboot si besoin
  - Maj Lapie HMAC
- ⏳ Tout est Versionné, pas de WIP qui traîne

---

- Maj budget couple

## ⏳ En attente

1. ⏳ Serveur > Maj WP 5.8 / Attente bitnami (5.7.2)
2. Trucs AE
   1. [hey](https://www.cominjob.com/candidat/)
   2. [hoy](https://www.ouiboss.com/)
   3. [prout](https://www.freelance-informatique.fr/)

### ⏳🌱 Vérifications sur la longueur

- 🌱 21/05/2021 > Heberg picard > Basculer sur nouveau serveur & annuler

## 💥 Tâches critiques

Bug clients majeurs, interruptions de service, etc.

## 🚧 WIP 🚧

Si travail en cours, indiquer *les notes* ici

## ⚡️ Tâches rapides ✨

Indiquer ici les *tâches en dehors du flux général* (urgences, corrections process, trucs qui perturbent et doivent être fait, tâches ultra rapides, etc.)

1. Serveur
   1. Lint done : ansible-install-web-server > README.MD
   2. Ansible convenience
       1. Clean templating, variable [deprecated ansible_managed](https://docs.ansible.com/ansible/2.4/intro_configuration.html#ansible-managed)
           1. [?](https://docs.ansible.com/ansible/latest/reference_appendices/config.html#default-managed-str)
       2. [ansible prompt](https://docs.ansible.com/ansible/latest/user_guide/playbooks_prompts.html)
   3. Opti script maintenance
      1. Ajouter maj OMZ ZSH
2. install-dev-env > docker-compose pour les principales technos : js & phpay
3. __TODO_shame.md > serveur
4. 🔍 [tmux](https://nickjanetakis.com/blog/who-else-wants-to-boost-their-productivity-with-tmux)
5. 🔍 [keys remap](https://nickjanetakis.com/blog/remap-and-set-global-hotkeys-on-windows-10-with-auto-hotkey)
6. Lapie > Traitement des tâches en souffrance
   1. Cleaner github dedié > client/url-site/
   2. Lapie > Ranger chartes graphiques & lapie-web
   3. Charte graphique > Faire les TODOs
   4. 🚚(shame) > Lapie kek.php (Crédit agricole > génération d'un fichier kek.php à la racine lors de l'insertion de clé HMAC > détruit au reboot du conteneur)
   5. Lapie, retours SEO
   6. Lapie > 🚚([Statut](https://docs.google.com/spreadsheets/d/1zZUT0F4XMQyVAFbP7ihACnRz10pmog5KoYlcaiXOGIk/edit#gid=0))
   7. ~Lapie > Maj traefik pour redirection www. > faire des tests alakon sur NDD masa avant, cf. critique
       1. Maj Ansible
   8. 🚚(shame) Accès fichiers bloqués conteneur bitnamiwp, modules php, passer en http2/3
7. Relancer impôts pro pour CFE
8. Renvoi doc AE décla 0€ années passées [hey](https://mail.google.com/mail/u/0/#inbox/FMfcgxmXKmkCGqSQkpPRbBrSKWcsbCpr)

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
