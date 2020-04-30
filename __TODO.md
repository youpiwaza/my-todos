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

1. ✅ Créer 2 playboks supplémentaires
   1. ✅ 98-Maintenance    > Opération usuelles, ~os & package update, docker system prune
      1. Piocher dans les rôles d'installation
   2. ✅ 99-Crafts & tests > Playbook dédié à la création, pour éviter de tout commenter/décommenter/oublier
   3. ✅ 97-Punctal-task   > Playbook pour éxécuter une (ou plusieurs) tâches ponctuelles
2. 🚀 Installer les containers de l'architecture de base via ansible
   1. ✅ Mettre en place les noms de domaine pour les tests & services publics de base
      1. test        .DOMAIN.COM   // basic nginx
      2. prometheus  .DOMAIN.COM   // metrics database
      3. grafana     .DOMAIN.COM   // visualize metrics
      4. alertmanager.DOMAIN.COM   // alerts dispatcher
      5. unsee       .DOMAIN.COM   // alert manager dashboard
   2. ✅ Informer l'utilisateur via debug, en fin de playbook 3.
   3. ✅ docker maintenance
      1. System prune
      2. Images removal
   4. ✅ Initialiser la stack
   5. ✅ Vérifier que l'utilisateur the_docker_guy peut lancer des stacks
      1. ✅ Utiliser la version curated
      2. ✅ Resoudre les problèmes de droits
      3. 🚧 Cleaner et mettre en place (99e playbook > 4eme playbook)
   6. Reverse Proxy
      1. Installation de [traefik pour Docker](https://docs.traefik.io/providers/docker/)
         1. Besoin de l'accès a la socket ! (même via un conteneur proxy)
         2. Ou [Nginx](https://hub.docker.com/r/jwilder/nginx-proxy/) ? / [proxy_pass](https://medium.com/@mannycodes/create-an-nginx-reverse-proxy-with-docker-a1c0aa9078f1)
         3. Exemple avec conf dans un container alakon avec un label traefik ?
   7. Utiliser des [fichiers de configs](https://docs.docker.com/engine/swarm/configs/) plutôt que mount/bind pour Nginx example
   8. Test avec 2 urls pour 2 sites
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
   6. 💥 /!\ Attention pour bdd et contenus, utiliser [volumes NOMMÉS pour Dstack](https://docs.docker.com/compose/compose-file/#volumes-for-services-swarms-and-stack-files), ou DESTRUCTION lors de la fin du service (si V anonyme)

128> Docker certification [175€](https://success.docker.com/certification)

## 🚧 WIP 🚧

.

## Priorisation, détails tâche courante

Sécurités SSL/TLS (Transport Layer Security / https) >
   Privilégier TLS 1.3 (le reste **deprecated** a part TLS 1.2)
   Doit être enregistré auprès d'une autorité de confiance > [liste française](https://webgate.ec.europa.eu/tl-browser/#/tl/FR)
   Privilégier les certificats courts (1 a 3 mois) au cas ou le serveur serait compromis (et possibilité de résilier un certif manuellement)
   Favoriser le mutual Auth
   Automatiser avec Let's encrypt

## Tests

hey
