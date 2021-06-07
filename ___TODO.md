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

## 🚀 Priorisation, simple ⏩

Indiquer ici les *tâches à effectuer en priorité*

- Si besoin de focus, mettre une ou 2 tâches ici.

- ⏳ Date bière élèves

Trucs sur le **Serveur**

1. ✅ Fusionner config dans generate
2. ✅ Plus de dossier /configs, directement dans le dossier client/etc/habituel/
3. ✅ Lint nginx folder & filenames > Renommer '/home/{{ users.3.name }}/configs/webserver/nginx/tutum--customUser-p8080-php--nginx.conf'
   1. ansible-install-web-server\ansible\roles\stack-web-nginx--config\tasks\main.yml
   2. ^ Attention à changer les chemins d'injection dans les .yml également
   3. ansible-install-web-server\nomenclature-and-folder-tree.md
4. ✅ WordPress forge stack > WordPress forge role
   1. ✅ Playbook to generate .yml files: playbook & role 20X-forge---DASHED-URI---wordpress-stack-generated.yml
   2. ✅ Ajuster stack-web-wordpress--generate-stack
5. ✅ Nginx forge stack > WordPress forge role
   1. ✅ Créer fichier de variables de projet
   2. ✅ Adapter generate stack
6. ✅👥 stack-web-nginx--generate > vars comme wordpress
7. ✅ Sur les fichiers générés
   1. ✅ En-tête avec commentaire: "Généré avec ansible + timestamp + ref au fichier original + ref playbook original"
   2. ✅ suffixe extension > ex "README.j2" devient "README.md.j2"
8. ✅ ansible > \n KO
9. ✅ Deprecated docker_container explicit default behavior stuff [container_default_behavior: compatibility](https://docs.ansible.com/ansible/latest/collections/community/docker/docker_container_module.html#parameter-container_default_behavior)
   1. ✅ ansible-install-web-server\ansible\roles\core-reverse-proxy-traefik--run\tasks\main.yml
   2. ✅ ansible-install-web-server\ansible\roles\stack-web-nginx--generate
   3. ✅ ansible-install-web-server\ansible\roles\stack-web-nginx--run
10. ✅ BUG: stack-web-nginx--run > can't update due to timestamp in .conf file
11. ✅ Forge playbookS > At the end add a message to start the generated playbook
12. ✅ Maj traefik ?
13. ✅ Clean noms containers (noms services fichiers yml :
    1. OK / test---test-wordpress--masamune--fr_mariadb.1.6u0pzz5paqai596um2b22eu1c
    2. NOK / test---hello-php--masamune--fr---tutum-hello-php_hello-php.1.
14. ✅ Add docker images credits.docs
15. ✅✅✅ Clean cette TODO, enlever les doublons👥
16. 🌱 done.md > ansible-install-web-server README.MD // voir faire un done.md pour le serveur haha, may bien rangé
17. Gestion des backups
    1. Ajout au CRON
    2. Envoi vers serveur de backup + rotation/sauvegarde incrémentielle
18. forge playbookS
    1. Générer des README.md
    2. playbboks supplémentaires
       1. stop stack
       2. uninstall stack (stop + rm volumes)
       3. save volumes ponctuel
          1. Création de l'arborescence, attention au répertoire année courante
       4. Prévoir dev & prod > 1 seul script mais url change, même users & pass
          1. Check ansible > vars d'environnement afin de maj dev. ou prod
          2. [Bonnes pratiques docker/compose](https://nickjanetakis.com/blog/best-practices-around-production-ready-web-apps-with-docker-compose)
          3. Gestion dev/prod : 1 seul fichier
          4. ENV vars ++
          5. Volumes en fonction de l'environnement ¤_¤
       5. Création d'un utilisateur ubuntu pour connexion ssh, qui remplace ftp (clé publique privée, etc.)
          1. Note: Probablement moyen de faire qu'un seul rôle, utilisé dans tous les playbooks webs
          2. Rôle ajout
          3. Rôle suppression
19. Tutum > remplacer par nginx
    1. Faire tourner déjà ca serait bien, go ctrl + f "curated"
    2. Utiliser vars d'environnement pour refaire un tutum mayzon: image + nom conteneur
20. Bitnami
    1. [Github issues](https://github.com/bitnami/bitnami-docker-mysql/issues/79#issuecomment-545477842) > Variable d'env afin d'augmenter le debug des conteneurs bitnami ! >> raisons explicites sur le problème de boot du conteneur
    2. Gestion notes dans ansible-install-web-server/ansible/203-setup-wordpress-lapie_secret.yml
    3. Lourder si serveurs web classique stabilité 100%, +1 speed
    4. Activer modules php
    5. Http 2/3
21. Mise en place d'une admin SQL > [phpmyadmin](https://hub.docker.com/_/phpmyadmin)
    1. Objectif 1 : Go nginx sur pma-test-wordpress.masamune.fr
        1. 🚀 .yml indépendant
        2. .yml de test-wordpress
    2. Objectif 2 : Go pma sur pma-test-wordpress.masamune.fr
       1. ^ Check DNS
22. Monitoring > MOD: 4-setup-core-services.yml
    1. Alternative ? [traefik pilot](https://doc.traefik.io/traefik-pilot/)
    2. Alerte si CPU/RAM > 75%
    3. Alerte si space disque libre < 20%
    4. Checker ce qui prend de la place sur le disque ~80Go ? 13% de 450 > `docker system df -v` ; cf. backup des volumes
23. Gestion des mails propre
    1. Connexion au serveur SMPT du serveur ? cf. utils-emails
    2. [Conteneur postfix ?](https://hub.docker.com/_/postfixadmin)
    3. Ajout SPF/DKIM/DMARC
    4. Maj lapie & nonore
24. Tester conteneurs de serveurs (facilité/stabilité/vitesse/http3)
    1. ✅ NDDs
       1. Need modules de cache php activés
       2. HTTP 2/3 serait un vrai plus
    2. [Apache](https://hub.docker.com/_/httpd) / test-httpd.masamune.fr
    3. [Nginx](https://hub.docker.com/_/nginx) / test-nginx.masamune.fr
       1. Tune server for [nginx performance](https://www.nginx.com/blog/10-tips-for-10x-application-performance/)
       2. [+1](https://blog.monitis.com/blog/6-best-practices-for-optimizing-your-nginx-performance/)
    4. [Caddy](https://hub.docker.com/_/caddy) / test-caddy.masamune.fr
    5. Litespeed : [open](https://hub.docker.com/r/litespeedtech/openlitespeed) / [payant ?](https://hub.docker.com/r/litespeedtech/litespeed)
       1. 2-3 trucs/plugins a regarder en plus pour WP : [doc](https://www.litespeedtech.com/open-source) & [site dédié](https://lscache.io/)
       2. test-litespeed.masamune.fr
    6. 🌱 Chaque serveur > Tester WP (install via wp-cli ?)
25. Cleaner / Relancer clients actuels
    1. Lapie
       1. Cleaner au niveau du serveur dashed-uri > .com ou .fr
    2. Nonore
       1. (wp généré et lancement depuis ansible), Pour le moment c'est un yml lancé a l'arrache sur le serveur
    3. Backups volumes
       1. Maj ansible-install-web-server/commandes-backup-volumes-a-la-maing_secret.md (dashed notation)
       2. (normalement d'ici la les roles de backups seront générés auto :3)
       3. Backup
26. Ansible convenience
    1. Clean templating, variable [deprecated ansible_managed](https://docs.ansible.com/ansible/2.4/intro_configuration.html#ansible-managed)
        1. [?](https://docs.ansible.com/ansible/latest/reference_appendices/config.html#default-managed-str)
    2. [ansible prompt](https://docs.ansible.com/ansible/latest/user_guide/playbooks_prompts.html)

### Sinon, priorisation classique

1. Tâches récurrentes
2. Tâches en attente
3. Tâches critiques
4. Tâches WIP
5. Tâches rapides
6. Autres fichiers TODO

## ♻️ Tâches récurrentes ♻️

Tâches à *vérifier au moins une fois par semaine*, afin d'éviter un bordel plus tard/exponentiel

- ✅ Déplacer les terminés ✅ à chaque début de semaine dans done.md
- 💩 Déplacer les TODO 🌱 dans _TODO_shame.md
- ✅ Shame TODOs : Extraire ici (### Shame) les emplois du temps stockés sur mails, edt portable, favoris, bureau. Si possible description + lien.
- ✅ Nettoyer le fichier __TODO
  - ✅ Status
  - ✅ Ce fichier > ### Shame
    - ✅ Ranger dans fichiers TODO correspondant
    - ✅ Prioriser
- ✅ Virer ce qui traine
  - ✅ sur le bureau
  - 💩 dans le dossier _shame du bureau
  - 💩 Lel (local)/Mes documents/_dev/_shame
  - ✅ Vider corbeille
  - ✅ Vider téléchargements
  - ✅ Dans les mails
- ✅ Déplacer veille onglets dans TODO_veille
- 💩 Ranger DD boulot
- 💩 Lel Veille / Un truc par semaine, genre le vendredi aprem, a githuber
- ✅ Déclaration Auto entrepreneur
- ✅ Vérifier impôts sur espace / Dernière vérif 01/06/2021
  - ✅ Perso
  - ✅ Pro
- ✅ Maj locales / Environnement de dev / Dernière maj le 01/06/21
  - ✅ Windaube update
  - ✅ Docker desktop (tray > icône > RC > Check for updates)
  - ✅ WSL
    - ✅ Version Ubuntu
      - 🚀 Si majeure, ré-effectuer [install-dev-env](https://github.com/youpiwaza/install-dev-env)
    - ✅ Packages & terminal, cf. ci dessous 1 liner
- ✅ Maj serveur, script maintenance
  - ✅ `98-maintenance.yml & sudo apt update && sudo apt -y upgrade & reboot si besoin`
  - ✅ Maj Lapie HMAC
- ✅ Tout est Versionné, pas de WIP qui traîne

```bash
sudo apt update && sudo apt -y upgrade && omz update && git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull
```

## ⏳ En attente

- Perso > Vérifier résilation red sfr une fois repassé chez soshs

### ⏳🌱 Vérifications sur la longueur

- 🌱 Impôts > Pas d'avis de CFE ?
  - Réponse par mail le 26/11/20, CA non transmis pour le moment, avis et prélèvement courant 2021
  - Toujours rien au 01/01/21
  - Toujours rien au 10/02/21
  - Toujours rien au 12/05/21
  - Site KO au 15/05/21 (maintenance ?), toujours KO le 19/05/21
  - Toujours rien au 26/05/21
  - Toujours rien au 01/06/21
- 🌱 21/05/2021 > Commande d'un hébergement ovh dédié aux picards (ovh manager > bare metal ? kimsufi) > rebasculer sur le nouveau serveur quand il sera terminé

## 💥 Tâches critiques

Bug clients majeurs, interruptions de service, etc.

## 🚧 WIP 🚧

Si travail en cours, indiquer *les notes* ici

## ⚡️ Tâches rapides ✨

Indiquer ici les *tâches en dehors du flux général* (urgences, corrections process, trucs qui perturbent et doivent être fait, tâches ultra rapides, etc.)

1. Migrer ancien serveur
   1. Migrer sites une fois serveur choisi
      1. Lister
         1. Technos
         2. 📌📌📌📌📌📌📌 Fichiers
         3. BDD / Exports WordPress
         4. Basculer
2. __TODO_shame.md > serveur
3. 🔍 [tmux](https://nickjanetakis.com/blog/who-else-wants-to-boost-their-productivity-with-tmux)
4. 🔍 [keys remap](https://nickjanetakis.com/blog/remap-and-set-global-hotkeys-on-windows-10-with-auto-hotkey)
5. Lapie > Traitement des tâches en souffrance
   1. Cleaner github dedié > client/url-site/
   2. Lapie > Ranger chartes graphiques & lapie-web
   3. Charte graphique > Faire les TODOs
   4. 🚚(shame) > Lapie kek.php (Crédit agricole > génération d'un fichier kek.php à la racine lors de l'insertion de clé HMAC > détruit au reboot du conteneur)
   5. Lapie, retours SEO
   6. Lapie > 🚚([Statut](https://docs.google.com/spreadsheets/d/1zZUT0F4XMQyVAFbP7ihACnRz10pmog5KoYlcaiXOGIk/edit#gid=0))
   7. ~Lapie > Maj traefik pour redirection www. > faire des tests alakon sur NDD masa avant, cf. critique
       1. Maj Ansible
   8. 🚚(shame) Accès fichiers bloqués conteneur bitnamiwp, modules php, passer en http2/3
6. Relancer impôts pro pour CFE
7. Renvoi doc AE décla 0€ années passées [hey](https://mail.google.com/mail/u/0/#inbox/FMfcgxmXKmkCGqSQkpPRbBrSKWcsbCpr)
8. CPF > Langage des signes / Amazon AWS
9. Cleaner zone DNS masamune.fr

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

Tout est priorisé :)

---
