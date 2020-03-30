# Shame / Vider la tête sans rien oublier

## Rangement

- Ranger notes-install... > Séparer Ansible de Docker de Serveur

## Prio

## Environnement de dev

- [Sanitize Ansible](https://docs.ansible.com/ansible/2.3/dev_guide/testing_sanity.html)
- Automatiser l'installation de l'environnement de developpement VIA projet install-dev-env
  - Full WSL
  - Bash > Installation d'ansible
  - Ansible > Mise en place du terminal + différentes conneries (tmux, zsh, etc.)
  - DCompose dédié pour image Ansible et tests des scripts sur image ubuntu, cf. [cocadmin](https://www.youtube.com/watch?v=yqLPUOsy-8M)
  - Installation et configuration de Docker
- Possibilité d'en faire un conteneur ? Ex: Alpine > avec interface graphique
- Docker GUI / [Kitematic](https://kitematic.com/) > Docker GUI
- [Packer](https://www.packer.io/) / Image build/vm/container automation
- Images basiques dédiées
  - Serveur PHP (nginx ou apache)
  - Serveur Node
  - Docker GUI [Portainer](https://blog.ippon.tech/tips-and-reminders-for-using-docker-daily/#tip3portainerftw)

## Divers

- Mettre en place l'envoi d'emails > 1 conteneur par site
- Oh my zsh > plugins docker++
- [Pimper vim](https://github.com/amix/vimrc) > awesome vim (fonts, etc.)
- [Pimper terminal avec tmux](https://www.grafikart.fr/tutoriels/pimp-my-shell-750) // zsh + omz faits

## Setup serveur

- 🐛 Clean system updates > Retours utilisateurs
- 🌱 Importer des variables depuis un repo privé
- Si zsh déjà installé, l'utiliser (afin de ne pas le virer en cas de reinstallation)
- Mails
  - Changer l'expéditeur > jax_the_mail_guy_WHATAVER@masamune.fr
  - Maj expediteur de fail2ban (rechercher 'fail2ban_sender')
  - Tester envoi
  - Tester envoi fail2ban
  - [Tester spam](https://www.mail-tester.com/)
- 🌱 [Backup via rsync](https://www.grafikart.fr/tutoriels/rsync-1012)
- [Users quota](https://www.digitalocean.com/community/tutorials/how-to-set-filesystem-quotas-on-ubuntu-18-04)
- Warning ubuntu : Canonical Livepatch is available for installation.
  - Reduce system reboots and improve kernel security. [Activate at](https://ubuntu.com/livepatch)
- Mise en place des CRONs
  - [docker system prune](https://docs.docker.com/config/pruning/)
- ♻️ Sécurité
  - remove unused
    - packages
    - process
- ♻️ Bonne pratiques
- [Customisable theme built to enhance the experience of browsing web directories](https://github.com/oupala/apaxy)
- Docker tests > if fail, remove test related containers/compose/services

### Images docker

- [Docker / How to Improve your Docker Image Builds](https://www.youtube.com/watch?v=npC0W2CW_as)
- ♻️ Healthcheck
  - [Doc docker](https://docs.docker.com/engine/reference/builder/#healthcheck)
  - Possibilité de mise en place [via Ansible](https://docs.ansible.com/ansible/latest/modules/docker_container_module.html#parameter-healthcheck)
- ♻️ Limitation de la RAM
- MAINTAINER
- [Best practices for writing Dockerfiles](https://docs.docker.com/develop/develop-images/dockerfile_best-practices/)
- Conteneurs montés a la volée en fonction des besoins, données persistées via *volumes*
- docker > client ftp pour les sites client : [ftp](https://www.grafikart.fr/tutoriels/proftpd-755) ?
- nginx > Prevent Flood/DDOS avec la configuration, [tuto grafikart](https://www.grafikart.fr/tutoriels/flood-ddos-fail2ban-884)
- [Analyser les configurations](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Docker_Security_Cheat_Sheet.md#rule-9---use-static-analysis-tools)
- 🔍 [Understanding and Hardening Linux Containers](https://www.nccgroup.trust/uk/our-research/understanding-and-hardening-linux-containers/)

## Ansible

- optimisation, utilisation systématique de changed
  - tâche 1 > `register: resultat`
  - tâche 2 dépendante : `when: resultat.changed`
- validate sur templates
  - [Iptables](https://www.grafikart.fr/tutoriels/iptables-694)

## Done

- ✅ Vérifier le bon fonctionnement de docker en local depuis la réinstallation
