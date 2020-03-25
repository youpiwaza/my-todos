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
   1. 🔍✅ Docs
      1. [Reco ansible](https://www.ansible.com/blog/six-ways-ansible-makes-docker-compose-better)
      2. [Ansible docker guide](https://docs.ansible.com/ansible/latest/scenario_guides/guide_docker.html)
      3. [Ansible docker_image module](https://docs.ansible.com/ansible/latest/modules/docker_image_module.html)
      4. [Ansible docker_container module](https://docs.ansible.com/ansible/latest/modules/docker_container_module.html)
      5. [Ansible docker_compose module](https://docs.ansible.com/ansible/latest/modules/docker_compose_module.html), également utilisé pour swarm
   2. ✅ Utiliser Docker compose & swarm pour faire la même chose
      1. ✅ Installation des [plugins recommandés](https://docs.ansible.com/ansible/latest/modules/docker_compose_module.html#requirements)
      2. ✅ Faire tourner un projet compose
         1. ✅🐛 **Attention**, si un nom de projet est spécifié au lancement, il doit également être spécifié lors de l'arrêt
      3. Faire tourner des services via swarm
         1. 🔍✅ Docs ansible
            - [Créer un swarm](https://docs.ansible.com/ansible/latest/modules/docker_swarm_module.html)
            - [Gérer les services](https://docs.ansible.com/ansible/latest/modules/docker_swarm_service_module.html)
            - [Docker stack](https://docs.ansible.com/ansible/latest/modules/docker_stack_module.html#examples)
         2. ✅ Initialiser swarm
            1. Conditionnel (pas péter prod avec tests)
         3. ✅ Lancer et tester un service
         4. ✅ Supprimer le swarm
         5. ✅ Idem `docker stack`
   3. 🚀 Mettre en place la sécurité docker en vérifiant que tout roule toujours
      1. 🔍 Docs
         - ✅ iptables firewall > docker [needs update](https://github.com/nickjj/ansible-iptables/blob/master/tasks/main.yml)
         - ✅ [Docker Post-installation steps for Linux](https://docs.docker.com/install/linux/linux-postinstall/)
         - ✅ [Run your app in production](https://docs.docker.com/get-started/orchestration/)
           - 🚀 [Docker security](https://docs.docker.com/engine/security/security/)
         - Security > capabilites. [Dedicated article](https://opensource.com/business/15/3/docker-security-tuning) as ansible official doc sucks
         - [Docker doc on capabilities](https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities) defauts & dispos
         - Utilisateur dédié pour docker / *the_docker_guy* > UNIX cap drop (remove `> cd /`)
      2. Docker Post-installation steps for Linux
         1. ✅ [Manage Docker as a non-root user](https://docs.docker.com/install/linux/linux-postinstall/#manage-docker-as-a-non-root-user)
         2. ✅ Configure Docker to start on boot
         3. ✅ Proper docker [logs](https://docs.docker.com/config/containers/logging/) [configuration](https://docs.docker.com/config/containers/logging/configure/)
            1. 🔍✅ Docs
               - [Sponso / Docker logging best practices](https://www.datadoghq.com/blog/docker-logging/)
                 - Reco: json-log default driver, avec quelques options + configurer logs par défaut + UI datadog (eq. grafana)
            2. 🔍✅ Choix
               1. Vérifier vite fait comparaison des plugins de logs / Splunk (~payant avec version gratuite) or Syslog (Peu d'interêt)
               2. Compatibilité avec les outils de management de [docker swarm rocks > swarmprom](https://dockerswarm.rocks/swarmprom/)
                  1. A priori grafana s'en occupe, a tester. Tâche rajoutée au monitoring
            3. ✅ Spécifier une [taille max](https://docs.docker.com/config/containers/logging/configure/#configure-the-default-logging-driver)
               1. Note: Le fichier /etc/docker/daemon.json n'existe pas par défaut.
               2. Note: docker a **besoin de restart** pour prendre en compte la nouvelle configuration des logs
      3. 🚀 Run your app in production
         1. ✅ Modification de la conf du *docker daemon*
         2. 🔍🔍🔍 Security
   4. ♻️ Images optimisées
   5. ♻️ Images saines
   6. 🔍 [Docker and permission management](https://blog.ippon.tech/docker-and-permission-management/)
   7. 🔍 [Docker security basics](https://innablr.com.au/blog/docker-security-basics/)
2. Installer les containers de l'architecture de base via ansible
   1. Installation de traefik
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

hey

## Priorisation, détails tâche courante

1. ✅ Refacto cookbooks > 1 rôle pour chaque tâche, ne pas grouper (préfixer rôles, ex: *security-noRootPw*)
2. Refacto variables
   1. Tri variables indispensables
   2. Non indispensables > Déplacer main_not_so_real dans defaults/main.yml
   3. Indispensables
      1. Fichier à la racine avec valeurs d'exemple
      2. Chargement des variables réelles depuis repo privé
3. Lint users
   1. Replace {{ users.0.name }} & {{ users.2.name }} par les vrais users
   2. Créer liste dynamique populée à partir des utilisateurs dédiés

## Tests

hey
