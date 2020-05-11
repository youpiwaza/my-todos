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
      3. ✅ Cleaner et mettre en place (99e playbook > 4eme playbook)
   6. 🚀 Reverse Proxy
      1. Installation de [traefik pour Docker](https://docs.traefik.io/providers/docker/)
         1. ✅ Docs
            1. [Traefik > Docker swarm discovery](https://docs.traefik.io/providers/docker/)
            2. [Traefik > Docker swarm routing](https://docs.traefik.io/routing/providers/docker/)
            3. [Traefik > Docker basic example](https://docs.traefik.io/user-guides/docker-compose/basic-example/)
            4. [Traefik > Docker TLS example](https://docs.traefik.io/user-guides/docker-compose/acme-tls/)
            5. [Traefik v2.2 notes](https://containo.us/blog/traefik-2-2-ingress/)
         2. Exemples en local
            1. ✅ Base stacks traefik + hello world
            2. Linted
               1. ✅ Toutes la doc
               2. 🐛✅ Problème avec sous domaines > Ressources statiques non trouvées (image tutum)
               3. ✅ Socket > [conteneur proxy pour accès à la socket](https://chriswiegman.com/2019/11/protecting-your-docker-socket-with-traefik-2/)
            3. ✅ Curated > Add my Dcompose recos (DBS, Labels, etc.)
            4. ✅ En faire des projets docker compose pour utilisation avec stack
               1. ✅ Ajout de l'utilisateur
               2. ✅ +1 pour site de test
            5. 🚀 Tests en ligne , cf. server-related-tutorials/01-docker/04-my-tests/09-traefik-curated/06-prod-traefik-curated
               1. ✅ Faire marcher, déjà
               2. ✅ Linter README & versionner tests cancer
               3. ✅ Faire marcher, déjà
                  1. Bad gateway 502 / connection refused / connect: permission denied / mes couilles
                     1. Rajouter au service Traefik
            6. 🌱 Résoudre les éventuels problèmes dans les logs
            7. ✅ Alpha reorder
            8. ✅ Comments
            9. ✅ Proper renaming
               1. ✅ Nomenclature ports exterieurs services (pas de doublons) / Regarder pour gestion automatique
                  1. Pas besoin de spécifier explicitement le port de sortie
               2. ✅ Nomenclature clients pour services et autres conneries traefik
                  1. Tester conflits de noms si services muliples
                  2. traefik_1            | {"level":"error","msg":"Router defined multiple times with different configurations in [hello-helloworld-ziecuama7f13gx12pg8vh11jt helloDeux-helloworld-g79k1r85gyzcuxv3v33k7lwnq]","providerName":"docker","routerName":"helloworld","time":"2020-05-08T14:37:31Z"}
                  3. > Cf. nomenclature
            10. ✅ Minor linting/tweaks
                1. ✅ Force bridge driver for socket network
                2. ✅ socket volume > force read only
                3. ✅ Activer l'encryptage du réseau d'accès à la socket [bret fisher stack example](https://github.com/BretFisher/dogvscat/blob/master/stack-proxy-global.yml)
                4. ✅ Lancer traefik as read only, cf bret ^
                5. ✅ Cap drop all + Cap_ADD "CAP_NET_BIND_SERVICE"
                6. ✅ Specific user > docker peon
                   1. command traefik error: error while building entryPoint web: error preparing server: error opening listener: listen tcp :80: bind: permission denied
                   2. // Specific unprivileged user needs access to ports < 1024
                     - sysctls:
                       - net.ipv4.ip_unprivileged_port_start: 0
                7. ✅ Traefik stats > Stats collection is disabled. Help us improve Traefik by turning this feature on :). More details [here](https://docs.traefik.io/contributing/data-collection/)
            11. ✅ Résoudre problèmes divers
                1. ✅ healthcheck traefik > OK direct
                2. ✅ "traefik.http.routers.helloworld.entrypoints=web" ???
                   1. WARN > No entryPoint defined for this router, using the default one(s) instead: [web]
                   2. Vérifier pour https
                   3. > Plus de trace dans les logs
            12. ✅ Rajouter mes recos de sécurité
                1. ✅ Proxy
                2. ✅ Traefik
                3. ✅ Tests hello
            13. 🌱 Répliques
                1. ✅ Tests hello
                2. ✅ Proxy
                3. ❌ Traefik / Published port 80 can be allocated to one container only (traefik + replicas = 2 containers)
                   1. TODO: Fix ?
            14. ✅ Test avec 2 services
            15. ✅ Test sur sous dossier
            16. ✅ Gestion des logs traefik (json + volumes > fichiers sur host)
                1. Docs
                    1. [Official docs](https://docs.traefik.io/observability/logs/)
                    2. [exemple](https://community.containo.us/t/502-bad-gateway-solved/2947)
                    3. [Access logs](https://docs.traefik.io/observability/access-logs/)
                2. ~~/var/log/*~~
                3. Traefik's container > /home/traefik.log
                4. Stored inside a named volume 'logs-traefik' in /home/traefik.log
            17. ✅ [Manage access logs](https://docs.traefik.io/observability/access-logs/)
            18. 🚀 HTTPS stuff
            19. Récupérer nomenclature server-related-tutorials\01-docker\04-my-tests\09-traefik-curated\Nomenclatures.md
                1. Fixer arborescence prod
                2. Logs traefik > nammed volume 'logs-traefik'
                   1. /home/traefik-debug.log
                   2. /home/traefik-access.log
            20. Host / Via ansible
                1. Sur host > Mettre dans un endroit correct ( docker_peon/core/ ?)
                2. Pas oublier network
                3. Pas oublier volume pour logs
         3. Vérifier que l'accès est bien bloqué en ligne [http://localhost:2375/version](http://localhost:2375/version) avec l'IP du serveur
         4. Tester routing via 3 conteneurs alakon > test.DOMAIN.COM, grafana.DOMAIN.COM & test.DOMAIN.COM/sub
         5. Accès en HTTPS (Port 443)
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
