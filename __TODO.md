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

X. ✅🐛 Traefik doesn't restart on host reboot

1. ✅ Faire une repasse sur les questions du début / notes-installation-serveur-web-docker/docs/08-Questions.md
2. Wordpress / Travail préliminaire
   1. ✅ Tests en local
      1. 📌 Choix: bitnami ATM (tester compatibilité avec custom user)
   2. Tests en ligne
      1. Mettre en place un wordpress de test (DNS test-wordpress.masamune.fr déjà en place)
         1. Faire tourner la stack
            1. ✅ docker run
            2. ✅ docker-compose
            3. ✅ docker-stack
         2. ✅ Ajouter les labels traefik
         3. ✅ Gestion des logs
      2. Curated/security
         1. Mine
            1. ✅ Usual security stuff
            2. 🌱 Custom user ? (bitnami already done on 1001)
            3. ✅ Replicas
               1. Check for favicon 500 ; check traefik logs to make sure 0 error 500 (related to replicas ?)
                  1. Ok w. only 1 mariadb
            4. ✅ Healtcheck
            5. ✅ Big checkup
               1. ✅ Ajout article/page
               2. ✅ Upload fichier
               3. ✅ Installation/activation/test plugin
         2. 🚀 bitnamis
            1. ✅ [~Optimize WordPress](https://docs.bitnami.com/bch/apps/wordpress/troubleshooting/optimize-bitnami-wordpress/)
               1. Activate W3 Total Cache (might need to chmod wp-config.php 660 to apply settings, then back to 440)
               2. [Pagespeed verifications](https://developers.google.com/speed/pagespeed/insights/?hl=fr&url=https%3A%2F%2Ftest-wordpress.masamune.fr%2F)
                  1. Avant opti: 1st: 500-1500ms, Suivants: 240ms. Pagespeed 93, ~indice de vitesse 2.8s
                  2. Après opti: 1st: 460-480ms, suivants: 150-170. Pagespeed 99, ~indice de vitesse 1.5s
               3. Note: police not embedded (theme wp 2020) qui ralentissent, il existe des articles dédiés pour retirer leurs chargements..
                  1. ~~Plugin OMGF / Optimize My Google Font > Télécharge en local et fout en cache~~
                     1. Nouvelle technos font vars ou chp > [besoin d'être viré](https://ryandaniels.ca/blog/set-up-customize-wordpress-twenty-twenty/#Delete-embedded-fonts)
                  2. Après opti: 1st: 420-430ms, suivants: 180. Pagespeed 100, ~indice de vitesse 1.3s
               4. Voir pour les plugins qui passent le site en statique
            2. ✅  [Secure WordPress](https://docs.bitnami.com/bch/apps/wordpress/troubleshooting/enforce-security/)
               1. Install WordFence security plugin x') > Scan > Start scan
         3. WP containers recommandations
            1. 🔍 Docs
               1. ✅ [DH wordpress official README](https://hub.docker.com/_/wordpress/)
               2. ✅ [DH bitnami WP README](https://hub.docker.com/r/bitnami/wordpress/)
               3. ✅ [DH bitnami mariadb README](https://hub.docker.com/r/bitnami/mariadb/)
            2. ✅ All variables + Reorga
            3. ✅ Custom values tests + recos
            4. Use docker secrets for sensitive stuff
            5. Big checkup
         4. WP
            1. When lunched w. docker-compose (no -d, json-file logs)
            2. /wp-admin/site-health.php
            3. [Wp recos](https://make.wordpress.org/hosting/handbook/handbook/server-environment/#php-extensions)
            4. plugin wp faster admin
         5. Check [WP-CLI](https://make.wordpress.org/cli/handbook/config/)
      3. Nomenclature
      4. Ansible > Test & template
3. Mettre en place un conteneur SFTP ?
4. Mettre en place un conteneur Accès bdd ?
5. Tâche ponctuelle clean logs (en attendant automatisation > traefik.log > 200514-traefik.log)
6. Veille securité
   1. [Docker Production Best Practices from Bret Fisher at DockerCon](https://www.youtube.com/watch?v=V4f_sHTzvCI)
   2. [Container security free pdf](http://containersecurity.tech/)
7. Installation du Monitoring
   1. 🔍 Docs
      - [Monitoring, the Prometheus Way](https://www.youtube.com/watch?v=PDxcEzu62jk)
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

128> Docker certification [175€](https://success.docker.com/certification)

## 🚧 WIP 🚧

.

## Priorisation, détails tâche courante

.

## Tests

hey
