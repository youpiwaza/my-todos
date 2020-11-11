# Shame / Vider la tête sans rien oublier

## Rangement

- Ranger notes-install... > Séparer Ansible de Docker de Serveur

## idées accès fichiers bloqués conteneur bitnamiwp

Tant que j'y pense, pour modifier les fichiers alakon du wp

- Se connecter au conteneur en forcant un utilisateur++ ? mais pas viable
- Sinon créer un (ou plusieurs) volume/s dédiés aux modifications spécifiques (ex racine du site servi pr .htaccess, robots.txt, etc.)
  - Voir si possibilité de conflits si plusieurs volumes tapent sur les mêmes fichiers d'un conteneur....
    - A priori non, le volume de base tape sur wp-config & wp-content, pas sur les fichiers serveurs, donc pas de soucis

- [Doc maj conteneur](https://onepagezen.com/add-expires-headers-wordpress-bitnami/)

Note : en passant par volume & connexion via conteneur anonyme > connecté en tant que root, avec lecture des bons droits (possibilité de chown derrière )

```bash
docker run \
   -it \
   --mount \
      source=client--dev-champagne-didier-lapie-com--wordpress--files,target=/home \
   --rm \
   --workdir /home \
   alpine \
   /bin/ash

> /home # whoami
**root**

> /home # ls -la
total 20
drwxrwxr-x    3 root     root          4096 Jun 23 13:19 .
drwxr-xr-x    1 root     root          4096 Nov 11 15:11 ..
-rw-r--r--    1 **1001**     root             0 Jun 23 13:14 .initialized
-rw-r--r--    1 1001     root             0 Nov  9 17:57 .restored
-r--r-----    1 1001     root          4201 Jun 23 13:54 wp-config.php
drwxr-xr-x   14 1001     root          4096 Nov  3 15:42 wp-content
```

## Shame

1. Choix du serveur web par défaut
   1. Docs
      - [Caddy](https://caddyserver.com/) vs [Nginx](https://www.nginx.com/)
        - [stackshare](https://stackshare.io/stackups/caddy-vs-nginx)
        - [rex](https://medium.com/@torch2424/my-experience-of-switching-from-nginx-to-caddy-79bc8cd627c0)
          - Caddy
            - HTTPS automatique
            - Configuration réduite et plus simple
            - Moins bonnes performances
      - NEED HTTP3 > Nginx (patch) / Caddy / Litespeed
   2. ♻️(tests) Mettre en place un nginx hello world sur un DNS, gestion du reverse proxy via traefik
      1. lel
   3. [Nginx](https://hub.docker.com/_/nginx)
      1. Sans reverse proxy ni dns ni style ni js > 1er affichage [80-120ms], suivants [30-40ms, pics a 60ms]
   4. +1 [Caddy](https://hub.docker.com/r/yobasystems/alpine-caddy/)
      1. Sans reverse proxy ni dns ni style ni js > 1er affichage [70-120ms], suivants [35-45ms, pics a 70ms]
   5. 📌 Test des performances > Choix
      1. Si choix Nginx Mettre en place HTTPS Automatique via Let's Encrypt
      2. Edit: HTTPS mis en place via Traefik
   6. 💥 /!\ Attention pour bdd et contenus, utiliser [volumes NOMMÉS pour Dstack](https://docs.docker.com/compose/compose-file/#volumes-for-services-swarms-and-stack-files), ou DESTRUCTION lors de la fin du service (si V anonyme)

## Prio

- [Abo litige](https://www.economie.gouv.fr/mediation-conso/vous-etes-professionnel)

## Environnement de dev

- [WLS 2](https://dev.to/twiddlewakka/20x-faster-speeds-by-updating-to-the-new-wsl-2-a-user-s-installation-guide-57n4)
- [Tara / Alternative Jira](https://www.blogdumoderateur.com/tara-outil-gestion-projet/)
- [Sanitize Ansible](https://docs.ansible.com/ansible/2.3/dev_guide/testing_sanity.html)
- Automatiser l'installation de l'environnement de developpement VIA projet install-dev-env
  - Full WSL
  - Bash > Installation d'ansible
  - Ansible > Mise en place du terminal + différentes conneries (tmux, zsh, etc.)
  - DCompose dédié pour image Ansible et tests des scripts sur image ubuntu, cf. [cocadmin](https://www.youtube.com/watch?v=yqLPUOsy-8M)
  - Installation et configuration de Docker
- Possibilité d'en faire un conteneur ? Ex: Alpine > avec interface graphique
- Docker GUI / [Kitematic](https://kitematic.com/) > Docker GUI
- [Packer](https://www.packer.io/) / Image build/vm/container automation
- Images basiques dédiées
  - Serveur PHP (nginx ou apache)
  - Serveur Node
  - Docker GUI [Portainer](https://blog.ippon.tech/tips-and-reminders-for-using-docker-daily/#tip3portainerftw)

## Divers

- Mettre en place l'envoi d'emails > 1 conteneur par site
- Oh my zsh > plugins docker++
- [Pimper vim](https://github.com/amix/vimrc) > awesome vim (fonts, etc.)
- [Pimper terminal avec tmux](https://www.grafikart.fr/tutoriels/pimp-my-shell-750) // zsh + omz faits
- OVH manager > Cleaner sous domaines persos

## Setup serveur

- 🌱 Importer des variables depuis un repo privé
- Si zsh déjà installé, l'utiliser (afin de ne pas le virer en cas de reinstallation) (etape 2 re-création d'users)
- Mails
  - Changer l'expéditeur > jax_the_mail_guy_WHATAVER@masamune.fr
  - Maj expediteur de fail2ban (rechercher 'fail2ban_sender')
  - Tester envoi
  - Tester envoi fail2ban
  - [Tester spam](https://www.mail-tester.com/)
- 🌱 [Backup via rsync](https://www.grafikart.fr/tutoriels/rsync-1012)
- Mise en place des CRONs
  - Backups sites !
  - [docker system prune -f](https://docs.docker.com/config/pruning/)
  - package update > upgrade > auto remove > auto clean
  - auditd once a week auto ? mail si problem
  - docker > [Rotate swarm CA certificates](https://docs.docker.com/engine/swarm/how-swarm-mode-works/pki/)
    - Usefull wehn having multiple managers/workers
  - Traefik [log rotation](https://docs.traefik.io/observability/logs/#log-rotation)
    - in named volumes "core-traefik-logs" > /home/logs/*.log
- [Customisable theme built to enhance the experience of browsing web directories](https://github.com/oupala/apaxy)
- Ansible Docker tests > if fail, remove test related containers/compose/services
- ♻️ Client FTP qui tape sur le même volume [Go](https://forums.docker.com/t/shared-web-hosting-with-docker-best-practices/7893/4)
- Traefik reverse proxy > Configure containers healthchecks
  - cf. server-related-tutorials/01-docker/04-my-tests/09-traefik-curated/03-curated-traefik-swarm-w-proxy-container/README.md
- [docker compose curated example](https://github.com/youpiwaza/docker-compose-curated-example/blob/master/docker-compose.yml)
  - Utiliser config plutôt que volumes
- [Bret fisher security recos](https://github.com/BretFisher/ama/issues/17)
- [D ELK](https://github.com/deviantony/docker-elk)

### Images docker

- Linter [hadolint](https://github.com/hadolint/hadolint) + [ext vscode](https://marketplace.visualstudio.com/items?itemName=exiasr.hadolint)
- [Docker / How to Improve your Docker Image Builds](https://www.youtube.com/watch?v=npC0W2CW_as)
- [Best practices for writing Dockerfiles](https://docs.docker.com/develop/develop-images/dockerfile_best-practices/)
- docker > client ftp pour les sites client : [ftp](https://www.grafikart.fr/tutoriels/proftpd-755) ?
- nginx > Prevent Flood/DDOS avec la configuration, [tuto grafikart](https://www.grafikart.fr/tutoriels/flood-ddos-fail2ban-884)
  - ✅ Aussi via docker
    - http://dockerlabs.collabnix.com/advanced/security/cgroups/#step-6-preventing-a-fork-bomb
    - --pids-limit 200
- [Analyser les configurations](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-9---use-static-analysis-tools)
  - Soft qui identifie les failles sécurités au build et lors de l'execution, avec un plan gratuit [Snyk](https://snyk.io/)

## Ansible

- optimisation, utilisation systématique de changed
  - tâche 1 > `register: resultat`
  - tâche 2 dépendante : `when: resultat.changed`
- validate sur templates
  - [Iptables](https://www.grafikart.fr/tutoriels/iptables-694)

## Done
