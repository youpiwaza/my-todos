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

- Oh my zeh > plugins docker++

- [Pimper vim](https://github.com/amix/vimrc) > awesome vim (fonts, etc.)

- [Pimper terminal avec tmux](https://www.grafikart.fr/tutoriels/pimp-my-shell-750) // zsh + omz faits

## Setup serveur

🐛 Clean system updates > Retours utilisateurs
✅ Utiliser *the_builder* pour installation des packages // besoin acl ? / https://docs.ansible.com/ansible/latest/user_guide/become.html#becoming-an-unprivileged-user
🌱 Importer des variables depuis un repo privé
🌱 Backup via rsync / https://www.grafikart.fr/tutoriels/rsync-1012

✅ zsh > gives root his own zsh + omz & remove tweak (root's $HOME is /root, other user's are /home/$USER)

docker > client ftp pour les sites client : [ftp](https://www.grafikart.fr/tutoriels/proftpd-755) ?

ansible > optimisation, utilisation systématique de changed
  tâche 1 > `register: resultat`
  tâche 2 dépendante : `when: resultat.changed`

ansible > validate sur templates

🚨 Mise en place de la synchro du temps du serveur / NTP

- [How to Install NTP Server and Client on Ubuntu](https://www.tecmint.com/install-ntp-server-and-client-on-ubuntu/)  // Classique mais serveur et client
- [ansible-role-ntp](https://github.com/geerlingguy/ansible-role-ntp)                                                 // Rôle compliqué
- [Set up NTP with Ansible, dedicating one as a timelord](https://gist.github.com/phillipuniverse/7721288)            // Rôle un peu plus simple

nginx > Prevent Flood/DDOSavec la configuration, [tuto grafikart](https://www.grafikart.fr/tutoriels/flood-ddos-fail2ban-884)

ansible local > playbook rename all *_not_so_real to * (/vars/main_not_so_real.yml)

Tuto complet [installation de serveur](https://www.howtoforge.com/perfect-server-debian-10-buster-apache-bind-dovecot-ispconfig-3-1/) a l'ancienne, voir s'il n'ya pas des outils a recup