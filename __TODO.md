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

1. Mettre en place la sécurité du serveur
   1. 🌱 Envoi de mail
      1. ✅🔍 Docs
         - [Ubuntu](https://help.ubuntu.com/lts/serverguide/postfix.html)
         - [Grafikart Postfix](https://www.grafikart.fr/tutoriels/postfix-sendonly-695)
         - [How to Setup Postfix as Send-only Mail Server on an Ubuntu 18.04 Dedicated Server or VPS](https://hostadvice.com/how-to/how-to-setup-postfix-as-send-only-mail-server-on-an-ubuntu-18-04-dedicated-server-or-vps/)
         - // Necessaire pour envoi de mails depuis le serveur (erreurs, logs, etc.)
      2. ✅ Config iptables pour envoi de mail approprié
      3. ✅ Test OK mais arrivée dans spams. En attendant la config > Gmail filtrer expéditeur > jamais dans spam
      4. 🌱 NDD > Ajout SPF            / Sender Policy Framework
      5. 🌱 NDD & mail() > Ajout DKIM  / DomainKeys Identified Mail
      6. 🌱 DMARC                      / Domain-Based Message Authentication, Reporting, and Conformance
      7. ✅ fail2ban config > ban_action : action_mwl (mail with logs en cas de ban)
   2. ✅ Mise à l'heure du serveur
      1. ✅🔍 Docs
         - [Chrony faq](https://chrony.tuxfamily.org/faq.html)
         - [Comparaison chrony vs ntp](https://chrony.tuxfamily.org/comparison.html)
         - [timesyncd.conf](http://manpages.ubuntu.com/manpages/cosmic/man5/timesyncd.conf.5.html)
         - [keep-your-clock-sync-with-internet-time-servers-in-ubuntu](https://vitux.com/keep-your-clock-sync-with-internet-time-servers-in-ubuntu/)
      2. ✅ Remplacer NTP par Chrony
      3. ✅ systemctl status systemd-timesyncd > inactive dead
         1. [doc](https://unix.stackexchange.com/questions/504381/chrony-vs-systemd-timesyncd-what-are-the-differences-and-use-cases-as-ntp-cli)
      4. ✅ Firewall / Autoriser Mise à l'heure du serveur [NTP](https://www.google.com/search?q=ntp)
   3. ✅ Sécurité
      1. ✅🔍 cocadmin / [sécurité serveur](https://www.youtube.com/watch?v=UmbndsZFIUE)
2. ✅ Environnement de dev propre
   1. ✅🔍 Docs
      1. [cocadmin](https://www.youtube.com/watch?v=yqLPUOsy-8M)
         1. Avoir une image docker pour faire tourner ansible (installation un poil plus complexe avec manip de docker)
         2. Utiliser docker pour monter un ubuntu (serveur) et faire tourner les scripts ansible dessus
   2. ✅ Faire tourner l'exemple
   3. ✅ Update > ansible:alpine & ubuntu:18.04
   4. ✅ Faire tourner un nginx (install via ansible) alakon sur 8080
      1. ✅ Vérif via ~~[curl](https://www.ansible.com/blog/six-ways-ansible-makes-docker-compose-better)~~ [uri](https://docs.ansible.com/ansible/latest/modules/uri_module.html)
   5. 💩 Installer docker et y monter un container nginx alakon
      1. KO / WSL + DinD
3. Installation de docker
   1. ✅🔍 Note: Rootless Docker
      1. is experimental
      2. features are not supported : Overlay network
         1. Nécessaire pour [réseau swarm](https://docs.docker.com/network/overlay/)
      3. Note: App armor pas dispo dans docker rootless, SEL Linux?
      4. 💩 > Installation classique
   2. ✅🔍 Docs
      - [Docker / Installation officielle](https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-using-the-repository)
      - [Digital ocean > Automate Docker install on ubuntu](https://www.digitalocean.com/community/tutorials/how-to-use-ansible-to-install-and-set-up-docker-on-ubuntu-18-04)
        - [+ playbook de base <3](https://github.com/do-community/ansible-playbooks/tree/master/docker_ubuntu1804)
      - Manage docker through ansible [Ansible Docker guide](https://docs.ansible.com/ansible/latest/scenario_guides/guide_docker.html)
   3. ✅🔍 Note: Docker in Docker (DinD), pour tests en local
      1. [First old article](https://www.docker.com/blog/docker-can-now-run-within-docker/)
      2. [Updated article](https://jpetazzo.github.io/2015/09/03/do-not-use-docker-in-docker-for-ci/)
      3. [Alternative : Run nested docker through global daemon (share socket)](https://itnext.io/docker-in-docker-521958d34efd)
      4. [--privileged / Not in prod](https://blog.trendmicro.com/trendlabs-security-intelligence/why-running-a-privileged-container-in-docker-is-a-bad-idea/)
      5. [Official docker image](https://hub.docker.com/_/docker)
4. ✅ Mettre en place un conteneur nginx hello world sur l'ip du serveur
   1. cf. `/ansible/roles/docker-installation/tasks/main.yml` > uncomment `include test-nginx.yml`
5. Utiliser Docker compose & swarm pour faire la même chose
   1. ✅ Installation des [plugins recommandés](https://docs.ansible.com/ansible/latest/modules/docker_compose_module.html#requirements)
   2. ✅ Faire tourner un projet compose
   3. 🚀Faire tourner des services via swarm
      1. 🔍 Docs ansible
         - [Créer un swarm](https://docs.ansible.com/ansible/latest/modules/docker_swarm_module.html)
         - [Gérer les services](https://docs.ansible.com/ansible/latest/modules/docker_swarm_service_module.html)
6. Mettre en place la sécurité en vérifiant que tout roule toujours
   1. 🔍 Docs
      - 🚧 iptables firewall > docker [needs update](https://github.com/nickjj/ansible-iptables/blob/master/tasks/main.yml)
      - [Docker Post-installation steps for Linux](https://docs.docker.com/install/linux/linux-postinstall/)
      - [Run your app in production](https://docs.docker.com/get-started/orchestration/)
      - [Docker security](https://docs.docker.com/engine/security/security/)
      - Utilisateur dédié pour docker / *the_docker_guy*
7. Installer les containers de base grâce à [ansible](https://www.ansible.com/blog/six-ways-ansible-makes-docker-compose-better)
   1. 🔍 Docs
       1. [Ansible docker guide](https://docs.ansible.com/ansible/latest/scenario_guides/guide_docker.html)
       2. [Ansible docker_image module](https://docs.ansible.com/ansible/latest/modules/docker_image_module.html)
       3. [Ansible docker_container module](https://docs.ansible.com/ansible/latest/modules/docker_container_module.html)
          1. Security > capabilites. [Dedicated article](https://opensource.com/business/15/3/docker-security-tuning) as ansible official doc sucks
          2. [Docker doc on capabilities](https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities) defauts & dispos
       4. [Ansible docker_compose module](https://docs.ansible.com/ansible/latest/modules/docker_compose_module.html), également utilisé pour swarm
   2. Installation de traefik
   3. Test avec 2 urls pour 2 sites
8. Installation du Monitoring
9. Choix du serveur web par défaut
   1. ♻️(tests) Mettre en place un nginx hello world sur un DNS, gestion du reverse proxy via traefik
   2. [Nginx](https://hub.docker.com/_/nginx)
      1. Sans reverse proxy ni dns ni style ni js > 1er affichage [80-120ms], suivants [30-40ms, pics a 60ms]
   3. +1 [Caddy](https://hub.docker.com/r/yobasystems/alpine-caddy/)
      1. Sans reverse proxy ni dns ni style ni js > 1er affichage [70-120ms], suivants [35-45ms, pics a 70ms]
   4. 📌 Test des performances > Choix
      1. Si choix Nginx Mettre en place HTTPS Automatique via Let's Encrypt
10. ♻️ Optimiser Dockerfiles

## 🚧 WIP 🚧

Bureau > doc installation docker via ansible

## Priorisation, détails tâche courante

1. ✅ Ansible > virer le warning python
   1. ansible_python_interpreter / [Forcer choix python pour ansible](https://docs.ansible.com/ansible/latest/reference_appendices/python_3_support.html)
   2. Modification des fichiers hosts
2. ✅ Lint > Tous les fichiers commencent par `---` et se terminent par `...`
3. clean install docker > ansible req on host
4. Refacto cookbooks > 1 rôle pour chaque tâche, ne pas grouper (préfixer rôles, ex: *security-noRootPw*)

## Tests

- ✅ Changer d'utilisateur en cours de playbook

- [Caddy](https://caddyserver.com/) vs [Nginx](https://www.nginx.com/)
  - [stackshare](https://stackshare.io/stackups/caddy-vs-nginx)
  - [rex](https://medium.com/@torch2424/my-experience-of-switching-from-nginx-to-caddy-79bc8cd627c0)
    - Caddy
      - HTTPS automatique
      - Configuration réduite et plus simple
      - Moins bonnes performances
