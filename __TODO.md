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
      1. Automatic security benchmark [Docker bench security](https://github.com/docker/docker-bench-security)
          1. ✅ [Aide pour les correctifs](https://www.digitalocean.com/community/tutorials/how-to-audit-docker-host-security-with-docker-bench-for-security-on-ubuntu-16-04)
          2. ✅ [+1](https://www.digitalocean.com/community/tutorials/7-security-measures-to-protect-your-servers)
          3. ✅ auditd installation & configuration
          4. ✅ Standalone containers recos (docker run)
             1. ✅ [Labels on containers](https://docs.docker.com/engine/reference/commandline/run/#set-metadata-on-container--l---label---label-file)
             2. ✅ [Labels best practices](https://docs.docker.com/config/labels-custom-metadata/)
                1. Authors of third-party tools should prefix each label key with the reverse DNS notation of a domain they own, such as com.example.some-label.
             3. Use label files ? No > Maintenance in 1 place + ansible's docker_container doesn't support
                1. ✅ Client
                2. ✅ Project
                3. ✅ Date
                4. ✅ Type = test/dev/prod
             4. ✅ Label on networks
             5. ✅ Label on volumes
          5. ✅ Check and clean TODO_shame for security stuff
          6. ✅ Via ansible
          7. ✅ Ansible task template > Utiliser [module_defaults](https://docs.ansible.com/ansible/latest/user_guide/playbooks_module_defaults.html)
             1. ✅ cf. server-related-tutorials/02-ansible/13-ansible-task-template-w-module-defaults
          8. ✅ Compose containers recos (docker compose)
          9. 🚀 Via ansible
          10. ⏩ Services recos (docker swarm & docker stack)
          11. ⏩ Via ansible
      2. Close this fucking topic
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

128> Docker certification [175€](https://success.docker.com/certification)

## 🚧 WIP 🚧

Faire plusieurs templates ansible (un de chaque pour lancer docker container/compose/swarm) comportant les attributs suivants

[cocadmin / templates yaml](https://youtu.be/7gmW6vxgsRQ?t=360)

Legend:
✅             / Standalone containers OK
✅✅           / + Standalone Ansible
✅✅✅         / + Compose containers
✅✅✅✅       / + Compose containers Ansible
✅✅✅✅✅     / + Services
✅✅✅✅✅✅   / + Services Ansible

- ✅✅✅ [Forcer l'utilisateur](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-2---set-a-user)
  - [Voir n°2](https://snyk.io/blog/10-docker-image-security-best-practices/)
- ✅✅✅ [No new privileges flag](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-4---add-no-new-privileges-flag)
  - --security-opt=no-new-privileges, [see](https://www.stackrox.com/post/2017/08/hardening-docker-containers-and-hosts-against-vulnerabilities-a-security-toolkit/#restrict-a-container-from-acquiring-new-privileges)
  - Also in daemon.json
- ✅✅✅ [Ajouter des labels](https://docs.docker.com/config/labels-custom-metadata/)
  - ✅✅✅ And to networks
  - ✅✅🚀🚀🚀🚀🚀🚀🚀🚀🚀 And to volumes
- ✅✅✅ Start containers automatically
- ✅✅❌ Resources allocations
  - Memory soft & hard limit, disable swap
  - CPU shares
  - Restrict process (pids limit)
  - *Note: Not available for docker-compose in v3. Only v2 or swarm*
- ✅✅✅ Working directory
- ✅✅✅ Volumes, mounted in /home/the_docker_peon/
  - ✅✅✅ [read-only flag](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-8---set-filesystem-and-volumes-to-read-only)
- ✅✅✅ No vars or ENV > use secrets
- ✅✅✅ Health checks
- ✅✅✅ [capabilities drop all, puis autoriser celles nécessaires](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-3---limit-capabilities-grant-only-specific-capabilities-needed-by-a-container)
  - [Docker doc on capabilities](https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities)
    - deny all “mount” operations;
    - deny access to raw sockets (to prevent packet spoofing);
    - deny access to some filesystem operations, like creating new device nodes, changing the owner of files, or altering attributes (including the immutable flag);
    - deny module loading;
    - and many others.
    - De manière générale, à l'intérieur du conteneur, pas droits pour ssh, cron, logs, hardware, network, NETCAT
  - [Docker security tuning](https://opensource.com/business/15/3/docker-security-tuning)
- ✅✅✅ [AppArmor > Profil de sécurité](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-6---use-linux-security-module-seccomp-apparmor-or-selinux)
  - default docker profile : --security-opt apparmor=docker-default
  - Generated new profile with [apparmor tools](https://github.com/docker/labs/tree/master/security/apparmor#step-5-extra-for-experts)
  - Load them thanks to `/ansible/roles/security-apparmor/tasks/main.yml`
  - Use with `docker run --security-opt "apparmor=docker-nginx"` where docker-nginx is the wanted profile
- ✅✅✅ Seccomp / Utiliser le profile par defaut [seccomp](https://docs.docker.com/engine/security/seccomp/)
  - --security-opt seccomp=/etc/docker/seccomp-profiles/default-docker-profile.json

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

Sécurités SSL/TLS (Transport Layer Security / https) >
   Privilégier TLS 1.3 (le reste **deprecated** a part TLS 1.2)
   Doit être enregistré auprès d'une autorité de confiance > [liste française](https://webgate.ec.europa.eu/tl-browser/#/tl/FR)
   Privilégier les certificats courts (1 a 3 mois) au cas ou le serveur serait compromis (et possibilité de résilier un certif manuellement)
   Favoriser le mutual Auth
   Automatiser avec Let's encrypt

## Tests

hey
