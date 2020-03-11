# Shame / Vider la tête sans rien oublier

- **Ranger notes-install.../TODO.md**
- Séparer Ansible de Docker de Serveur

- [Packer](https://www.packer.io/) / Image build/vm/container automation

- Vérifier le bon fonctionnement de docker en local depuis la réinstallation

- Cleaner environnement de développement VIA projet install-dev-env
  - Si possible via différents ansible
    - Mettre en place une image docker dédiée
    - Mise en place du terminal + différentes conneries (tmux, zsh, etc.)

- Récupérer la gestion des linters en global pour l'appliquer sur l'environnement de developpement
  - .md
  - ansible

- Mettre en place l'envoi d'emails > 1 serveur ou 1 conteneur par site ?

- Oh my zeh > plugins docker++

- [Pimper vim](https://github.com/amix/vimrc) > awesome vim (fonts, etc.)

- [Pimper terminal avec tmux](https://www.grafikart.fr/tutoriels/pimp-my-shell-750) // zsh + omz faits

## Setup serveur

🐛 Fix system updates > auto upgrade (update-manager-core > do-release-upgrade) KO ?
🐛 Clean system updates > Retours utilisateurs
🌱 Utiliser *the_builder* pour installation des packages // besoin acl ? / https://docs.ansible.com/ansible/latest/user_guide/become.html#becoming-an-unprivileged-user
🌱 Importer des variables depuis un repo privé
🌱 Configuration du SSH / A la mano pour le moment / https://www.grafikart.fr/tutoriels/ssh-686
  Use the [fetch](https://docs.ansible.com/ansible/latest/modules/fetch_module.html#fetch-module) module to copy files from remote locations to the local box.
🌱 Backup via rsync / https://www.grafikart.fr/tutoriels/rsync-1012