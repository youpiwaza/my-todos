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
      3. 🌱 NDD > Ajout SPF            / Sender Policy Framework
      4. 🌱 NDD & mail() > Ajout DKIM  / DomainKeys Identified Mail
      5. 🌱 DMARC                      / Domain-Based Message Authentication, Reporting, and Conformance
      6. ✅ fail2ban config > ban_action : action_mwl (mail with logs en cas de ban)
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
2. Environnement de dev propre
   1. ✅🔍 Docs
      1. [cocadmin](https://www.youtube.com/watch?v=yqLPUOsy-8M)
         1. Avoir une image docker pour faire tourner ansible (installation un poil plus complexe avec manip de docker)
         2. Utiliser docker pour monter un ubuntu (serveur) et faire tourner les scripts ansible dessus
   2. ✅ Faire tourner l'exemple
   3. ✅ Update > ansible:alpine & ubuntu:18.04
   4. ✅ Faire tourner un nginx (install via ansible) alakon sur 8080
      1. ✅ Vérif via ~~[curl](https://www.ansible.com/blog/six-ways-ansible-makes-docker-compose-better)~~ [uri](https://docs.ansible.com/ansible/latest/modules/uri_module.html)
   5. 🚀Installer docker et y monter un container nginx alakon
      1. Vérif via curl
3. Installation de docker
   1. Note: Rootless Docker
      1. is experimental
      2. features are not supported : Overlay network
      3. > Installation classique
      4. Note: App armor pas dispo dans docker rootless, SEL Linux?
      5. Note: **Véritable besoin de réseau overlay ?**
   2. 🔍 Docs
      - [Docker / Installation officielle](https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-using-the-repository)
        - [Post-installation steps for Linux](https://docs.docker.com/install/linux/linux-postinstall/)
        - [Run your app in production](https://docs.docker.com/get-started/orchestration/)
      - [Ansible Docker guide](https://docs.ansible.com/ansible/latest/scenario_guides/guide_docker.html)
      - [Digital ocean > Automate Docker install on ubuntu](https://www.digitalocean.com/community/tutorials/how-to-use-ansible-to-install-and-set-up-docker-on-ubuntu-18-04)
        - [+ playbook de base <3](https://github.com/do-community/ansible-playbooks/tree/master/docker_ubuntu1804)
   3. iptables firewall > docker [needs update](https://github.com/nickjj/ansible-iptables/blob/master/tasks/main.yml)
4. Mettre en place un conteneur nginx hello world sur l'ip du serveur
5. Recos [Faire tourner Docker pour la production](https://docs.docker.com/get-started/orchestration/)
6. Installation de traefik
7. ♻️(tests) Mettre en place un nginx hello world sur un DNS, gestion du reverse proxy via traefik
   1. +1 Caddy
   2. 📌 Test des performances > Choix
      1. Si choix Nginx Mettre en place HTTPS Automatique via Let's Encrypt
8. Mettre en place la sécurité en vérifiant que tout roule toujours
   1. 🔍 Docs
      - [Docker security](https://docs.docker.com/engine/security/security/)
      - [Docker Post-installation steps for Linux](https://docs.docker.com/install/linux/linux-postinstall/)
9. Installer les containers de base grâce à [ansible](https://www.ansible.com/blog/six-ways-ansible-makes-docker-compose-better)
10. Monitoring
11. ♻️ Optimiser Dockerfiles

## 🚧 WIP 🚧

Bureau > doc installation docker via ansible

## Priorisation, détails tâche courante

1. Ansible > virer le warning python
   1. ansible_python_interpreter / [Forcer choix python pour ansible](https://docs.ansible.com/ansible/latest/reference_appendices/python_3_support.html)

## Tests

- ✅ Changer d'utilisateur en cours de playbook

- [Caddy](https://caddyserver.com/) vs [Nginx](https://www.nginx.com/)
  - [stackshare](https://stackshare.io/stackups/caddy-vs-nginx)
  - [rex](https://medium.com/@torch2424/my-experience-of-switching-from-nginx-to-caddy-79bc8cd627c0)
    - Caddy
      - HTTPS automatique
      - Configuration réduite et plus simple
      - Moins bonnes performances
