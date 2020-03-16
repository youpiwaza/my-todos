# Shame / Vider la tête sans rien oublier

- **Ranger notes-install.../TODO.md**
- Séparer Ansible de Docker de Serveur

- [Packer](https://www.packer.io/) / Image build/vm/container automation

- Vérifier le bon fonctionnement de docker en local depuis la réinstallation

- Cleaner environnement de développement VIA projet install-dev-env
  - Si possible via différents ansible
    - Mettre en place une image docker dédiée
    - Mise en place du terminal + différentes conneries (tmux, zsh, etc.)

- Mettre en place l'envoi d'emails > 1 serveur ou 1 conteneur par site ?

- Oh my zsh > plugins docker++

- [Pimper vim](https://github.com/amix/vimrc) > awesome vim (fonts, etc.)

- [Pimper terminal avec tmux](https://www.grafikart.fr/tutoriels/pimp-my-shell-750) // zsh + omz faits

## Setup serveur

🐛 Clean system updates > Retours utilisateurs
🌱 Importer des variables depuis un repo privé
🌱 [Backup via rsync](https://www.grafikart.fr/tutoriels/rsync-1012)

docker > client ftp pour les sites client : [ftp](https://www.grafikart.fr/tutoriels/proftpd-755) ?

ansible > optimisation, utilisation systématique de changed

- tâche 1 > `register: resultat`
- tâche 2 dépendante : `when: resultat.changed`

ansible > validate sur templates

nginx > Prevent Flood/DDOS avec la configuration, [tuto grafikart](https://www.grafikart.fr/tutoriels/flood-ddos-fail2ban-884)

- ansible local > playbook rename all *_not_so_real to* (/vars/main_not_so_real.yml)
  - Utiliser main.yml par défaut, sinon remplacer par importdepuis repo privé
    - A placer dans defaults/vars/main.yml

Tuto complet [installation de serveur](https://www.howtoforge.com/perfect-server-debian-10-buster-apache-bind-dovecot-ispconfig-3-1/) a l'ancienne, voir s'il n'ya pas des outils a recup