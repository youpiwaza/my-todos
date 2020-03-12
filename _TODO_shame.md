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