# Taf en cours

Légende :

- 🚀  En cours / **1 MAX A LA FOIS**
- ✅  Terminé
- ⏩  Suite
- 📌  A tester
- ♻️  Contenus/notes dans TODO_details_shame.md
- 🔍  Lecture/Vidéos
- 🌱  TODO
- 🚧  WIP / Work In Progress
- 💩  KO

**Tâches récurrentes** :

- Déplacer les terminés ✅ à chaque début de semaine dans README.
- Déplacer les TODO 🌱 dans _TODO_shame.md

## Priorisation, simple

1. Installation de docker
   1. Mettre en place la sécurité docker en vérifiant que tout roule toujours
      1. 🔍 Docs
         - ✅ iptables firewall > docker [needs update](https://github.com/nickjj/ansible-iptables/blob/master/tasks/main.yml)
         - ✅ [Docker Post-installation steps for Linux](https://docs.docker.com/install/linux/linux-postinstall/)
         - ✅ [Run your app in production](https://docs.docker.com/get-started/orchestration/)
           - 🚀 [Docker security](https://docs.docker.com/engine/security/security/)
         - ✅ Security > capabilites. [Dedicated article](https://opensource.com/business/15/3/docker-security-tuning) as ansible official doc sucks
           - ✅ [Docker doc on capabilities](https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities) defauts & dispos
           - ✅ [Docker and permission management](https://blog.ippon.tech/docker-and-permission-management/)
           - ✅ [Docker security basics](https://innablr.com.au/blog/docker-security-basics/)
      2. Docker Post-installation steps for Linux
         1. ✅ [Manage Docker as a non-root user](https://docs.docker.com/install/linux/linux-postinstall/#manage-docker-as-a-non-root-user)
         2. ✅ Configure Docker to start on boot
         3. ✅ Proper docker [logs](https://docs.docker.com/config/containers/logging/) [configuration](https://docs.docker.com/config/containers/logging/configure/)
            1. 🔍✅ Docs
               - ✅ [Sponso / Docker logging best practices](https://www.datadoghq.com/blog/docker-logging/)
                 - Reco: json-log default driver, avec quelques options + configurer logs par défaut + UI datadog (eq. grafana)
            2. 🔍✅ Choix : Grafana (cf. [docker swarm rocks > swarmprom](https://dockerswarm.rocks/swarmprom/) )
            3. ✅ Spécifier une [taille max](https://docs.docker.com/config/containers/logging/configure/#configure-the-default-logging-driver)
               1. ✅ Note: Le fichier /etc/docker/daemon.json n'existe pas par défaut.
               2. ✅ Note: docker a **besoin de restart** pour prendre en compte la nouvelle configuration des logs
      3. 🚀 Run your app in production
         1. 🚧🔍 MAJ `ansible/roles/docker-installation/tasks/run-your-app-in-production.yml`
         2. ✅ Modification de la conf du *docker daemon*
            1. ✅ Template (json) + doc .MD
         3. 🔍✅ [Ubuntu server](https://help.ubuntu.com/lts/serverguide/serverguide.pdf)
         4. Remove *the_docker_peon* privileges, so he can access only his own `/home`
            1. ✅ [Ubuntu doc / Restrict /home_da_user access to only himself](https://help.ubuntu.com/lts/serverguide/serverguide.pdf#page=188)
            2. 🚀 SSH prison ?
         5. ⏩ Add restriction to docker volumes (via *the_docker_guy* ?) > volumes only mounted in *the_docker_peon* `/home`
         6. ⏩ Restrict possibility to create a container from inside a container
         7. ⏩ Use traditional UNIX permission checks to limit access to the control socket
         8. ⏩ Limit docker functions
            1. docker load
            2. docker pull
         9. [Ubuntu user privileges list](https://wiki.ubuntu.com/Security/Privileges)
         10. ✅ AppArmor
             1. 🔍✅ Docs
                1. [Ubuntu / AppArmor](https://help.ubuntu.com/lts/serverguide/serverguide.pdf#page=200)
                2. [AppArmor](https://apparmor.net/) & [Main commands](https://gitlab.com/apparmor/apparmor/-/wikis/Documentation)
             2. ✅ Install
             3. ✅ Load profile/s
                1. ✅ Nginx example profile load
             4. ✅ Apply to docker daemon / already done by docker
             5. 🔍✅ ~~[App armor recommandations & profiles](https://www.nccgroup.trust/uk/our-research/abusing-privileged-and-unprivileged-linux-containers/)~~
      4. grsec
      5. egress
      6. ✅ [Docker_Security_Cheat_Sheet.md](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet)
      7. [Ubuntu CVE / Common Vulnerabilities and Exposures](https://www.google.com/search?q=ubuntu+CVEs)md#rule-10---set-the-logging-level-to-at-least-info)
      8. Check TODO_shame for security stuff
      9. Close this fucking topic
2. Installer les containers de l'architecture de base via ansible
   1. Reverse Proxy
      1. Installation de [traefik pour Docker](https://docs.traefik.io/providers/docker/)
         1. Besoin de l'accès a la socket ! (même via un conteneur proxy)
         2. Ou [Nginx](https://hub.docker.com/r/jwilder/nginx-proxy/) ? / [proxy_pass](https://medium.com/@mannycodes/create-an-nginx-reverse-proxy-with-docker-a1c0aa9078f1)
         3. Exemple avec conf dans un container alakon avec un label traefik ?
   2. Test avec 2 urls pour 2 sites
3. Installation du Monitoring
   1. 🔍 Docs
      - [Docker swarm rocks > monitoring w. swarprom](https://dockerswarm.rocks/swarmprom/)
        - [Docker / Prometheus setup](https://docs.docker.com/config/daemon/prometheus/)
        - [Swarmprom - Prometheus Monitoring for Docker Swarm](https://www.weave.works/blog/swarmprom-prometheus-monitoring-for-docker-swarm)
   2. UI pour afficher les logs docker de chaque service (~eq datadog)
4. Choix du serveur web par défaut
   1. Docs
      - [Caddy](https://caddyserver.com/) vs [Nginx](https://www.nginx.com/)
        - [stackshare](https://stackshare.io/stackups/caddy-vs-nginx)
        - [rex](https://medium.com/@torch2424/my-experience-of-switching-from-nginx-to-caddy-79bc8cd627c0)
          - Caddy
            - HTTPS automatique
            - Configuration réduite et plus simple
            - Moins bonnes performances
   2. ♻️(tests) Mettre en place un nginx hello world sur un DNS, gestion du reverse proxy via traefik
   3. [Nginx](https://hub.docker.com/_/nginx)
      1. Sans reverse proxy ni dns ni style ni js > 1er affichage [80-120ms], suivants [30-40ms, pics a 60ms]
   4. +1 [Caddy](https://hub.docker.com/r/yobasystems/alpine-caddy/)
      1. Sans reverse proxy ni dns ni style ni js > 1er affichage [70-120ms], suivants [35-45ms, pics a 70ms]
   5. 📌 Test des performances > Choix
      1. Si choix Nginx Mettre en place HTTPS Automatique via Let's Encrypt

## 🚧 WIP 🚧

Faire plusieurs templates ansible (un de chaque pour lancer docker container/compose/swarm) comportant les attributs suivants

[cocadmin / templates yaml](https://www.youtube.com/watch?v=7gmW6vxgsRQ)

- [Forcer l'utilisateur](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-2---set-a-user)
- [capabilities drop all, puis autoriser celles nécessaires](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-3---limit-capabilities-grant-only-specific-capabilities-needed-by-a-container)
  - [Docker doc on capabilities](https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities)
  - [Docker security tuning](https://opensource.com/business/15/3/docker-security-tuning)
    - De manière générale, à l'intérieur du conteneur, pas droits pour ssh, cron, logs, hardware, network
- [No new privileges flag](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-4---add-no-new-privileges-flag)
- [AppArmor > Profil de sécurité](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-6---use-linux-security-module-seccomp-apparmor-or-selinux)
  - Generated new profile with [apparmor tools](https://github.com/docker/labs/tree/master/security/apparmor#step-5-extra-for-experts)
  - Load them thanks to `/ansible/roles/security-apparmor/tasks/main.yml`
  - Use with `docker run --security-opt "apparmor=docker-nginx"` where docker-nginx is the wanted profile
- [read-only flag](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-8---set-filesystem-and-volumes-to-read-only)
  - Également sur les volumes (ex: un front qui va taper dans la bdd)
- [Ajouter des labels](https://docs.docker.com/config/labels-custom-metadata/)
- Start containers automatically
- Resources allocations

## Priorisation, détails tâche courante

1. Refacto variables
   1. Tout mettre dans */defaults/main.yml
   2. Fichier à la racine avec valeurs par défaut, toutes commentées
      1. ~conflits noms identiques
   3. Chargement de mes variables réelles depuis repo privé
2. Lint users
   1. Replace {{ users.0.name }} & {{ users.2.name }} par les vrais users
      1. Rechercher {{ users. et {{users.
   2. Créer liste dynamique populée à partir des utilisateurs dédiés
   3. ansible\roles\docker-installation\templates\etc-docker-daemon-json.j2
3. Ubuntu reco : Canonical Livepatch is available for installation.
    - Reduce system reboots and improve kernel security. [Activate at](https://ubuntu.com/livepatch)

## Tests

hey
