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
   1. (Déjà fait)
   2. 🔍✅ Docs
      1. [Reco ansible](https://www.ansible.com/blog/six-ways-ansible-makes-docker-compose-better)
      2. [Ansible docker guide](https://docs.ansible.com/ansible/latest/scenario_guides/guide_docker.html)
      3. [Ansible docker_image module](https://docs.ansible.com/ansible/latest/modules/docker_image_module.html)
      4. [Ansible docker_container module](https://docs.ansible.com/ansible/latest/modules/docker_container_module.html)
      5. [Ansible docker_compose module](https://docs.ansible.com/ansible/latest/modules/docker_compose_module.html), également utilisé pour swarm
   3. Utiliser Docker compose & swarm pour faire la même chose
      1. ✅ Installation des [plugins recommandés](https://docs.ansible.com/ansible/latest/modules/docker_compose_module.html#requirements)
      2. ✅ Faire tourner un projet compose
         1. 🚀🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧🚧Nope, ça down pas
      3. Faire tourner des services via swarm
         1. 🔍 Docs ansible
            - [Créer un swarm](https://docs.ansible.com/ansible/latest/modules/docker_swarm_module.html)
            - [Gérer les services](https://docs.ansible.com/ansible/latest/modules/docker_swarm_service_module.html)
   4. Mettre en place la sécurité docker en vérifiant que tout roule toujours
      1. 🔍 Docs
         - 🚧 iptables firewall > docker [needs update](https://github.com/nickjj/ansible-iptables/blob/master/tasks/main.yml)
         - [Docker Post-installation steps for Linux](https://docs.docker.com/install/linux/linux-postinstall/)
         - [Run your app in production](https://docs.docker.com/get-started/orchestration/)
         - [Docker security](https://docs.docker.com/engine/security/security/)
         - Security > capabilites. [Dedicated article](https://opensource.com/business/15/3/docker-security-tuning) as ansible official doc sucks
         - [Docker doc on capabilities](https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities) defauts & dispos
         - Utilisateur dédié pour docker / *the_docker_guy*
         - SELinux + automatiser
   5. ♻️ Images optimisées
   6. ♻️ Images saines
2. Installer les containers de l'architecture de base via ansible
   1. Installation de traefik
   2. Test avec 2 urls pour 2 sites
3. Installation du Monitoring
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

hey

## Priorisation, détails tâche courante

1. Refacto cookbooks > 1 rôle pour chaque tâche, ne pas grouper (préfixer rôles, ex: *security-noRootPw*)

## Tests

hey
