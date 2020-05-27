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

1. Mettre en place un wordpress (DNS test-wordpress.masamune.fr déjà en place)
2. Tâche ponctuelle clean logs (en attendant automatisation > traefik.log > 200514-traefik.log)
3. Installation du Monitoring
   1. 🔍 Docs
      - [Docker swarm rocks > monitoring w. swarprom](https://dockerswarm.rocks/swarmprom/)
        - [Docker / Prometheus setup](https://docs.docker.com/config/daemon/prometheus/)
          - Traefik config
            - [Official doc](https://docs.traefik.io/observability/metrics/prometheus/)
            - [Example](https://community.containo.us/t/502-bad-gateway-solved/2947) >
            - "--metrics.prometheus=true"
            - "--entryPoints.metrics.address=:8082"
            - "--metrics.prometheus.entryPoint=metrics"
            - "--metrics.prometheus.buckets=0.1,0.3,1.2,5.0"
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
      1. lel
   3. [Nginx](https://hub.docker.com/_/nginx)
      1. Sans reverse proxy ni dns ni style ni js > 1er affichage [80-120ms], suivants [30-40ms, pics a 60ms]
   4. +1 [Caddy](https://hub.docker.com/r/yobasystems/alpine-caddy/)
      1. Sans reverse proxy ni dns ni style ni js > 1er affichage [70-120ms], suivants [35-45ms, pics a 70ms]
   5. 📌 Test des performances > Choix
      1. Si choix Nginx Mettre en place HTTPS Automatique via Let's Encrypt
      2. Edit: HTTPS mis en place via Traefik
   6. 💥 /!\ Attention pour bdd et contenus, utiliser [volumes NOMMÉS pour Dstack](https://docs.docker.com/compose/compose-file/#volumes-for-services-swarms-and-stack-files), ou DESTRUCTION lors de la fin du service (si V anonyme)

128> Docker certification [175€](https://success.docker.com/certification)

## 🚧 WIP 🚧

.

## Priorisation, détails tâche courante

.

## Tests

hey
