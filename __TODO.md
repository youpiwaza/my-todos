# Taf en cours

Légende :

- 🚀  En cours / **1 MAX A LA FOIS**
- ✅  Terminé
- ⏩  Suite
- 📌 A tester
- ♻️  Contenus/notes dans TODO_details_shame.md
- 🔍  Lecture/Vidéos
- 🌱 TODO
- 🚧 WIP / Work In Progress

**Tâches récurrentes** :

- Déplacer les terminés ✅ à chaque début de semaine dans README.
- Déplacer les TODO 🌱 dans _TODO_shame.md

## Priorisation, simple

Mettre en place le nouveau serveur

1. Tutoriels Ansible
   1. ✅ Prise en main ansible, repomper commandes grafikart ♻️ Grafikart Ansible + doc
   2. ✅ Rangement en recette clean (arborescence) > Création des roles
      1. ✅ Lancer un service après installation
      2. ✅ Créer des dossiers & fichiers
      3. ✅ Modifier une ligne dans un fichier (.. de configuration)
      4. ✅ Importer du contenu depuis un repo
2. Mettre en place la sécurité du serveur
   1. ✅ Create server repo & obfuscate vars
   2. ✅ Create a repo for Ansible role template
   3. ✅ Gestion de la connexion
      1. ✅ Création des clés SSH publiques et privées
      2. ✅ Implémentation des clés en local (.sh)
         1. ✅ Définition de l'agent ssh
         2. ✅ Ajout des clés
      3. ✅ Implémentation des clés sur le serveur
      4. ✅ Changement du port SSH
      5. ✅ Reconnexion avec *the_builder_guy* avec le bon port
   4. ✅ Installation des logiciels de base sur le serveur
   5. ✅ [Installation d'un utilisateur](https://www.grafikart.fr/tutoriels/ansible-753) sur le serveur et [bases SSH](https://www.grafikart.fr/tutoriels/ssh-686)
      1. ✅ Template de génération d'utilisateurs
         1. ✅ Roles différents (ex: sudo conditionnel)
      2. ✅ Retirer connexion par mots de passe
      3. ✅ Retirer connexion root
   6. 🔍 Grafikart / Mise en place d'un serveur web
      1. ✅ [Configration de VIM](https://www.grafikart.fr/tutoriels/vim-685)
      2. ✅ [CRONs](https://www.grafikart.fr/tutoriels/cron-tache-recurrente-1013)
         1. ✅ Faire un utilisateur dédié pour les crons
         2. ✅ Retirer les droits aux autres utilisateurs "cron.allow / cron.deny"
      3. ✅ [Shell](https://www.grafikart.fr/tutoriels/pimp-my-shell-750)
      4. 🌱 Envoi de mail / [Postfix](https://www.grafikart.fr/tutoriels/postfix-sendonly-695) ou [autre](https://www.ubuntupit.com/best-linux-mail-server-software-and-solutions/),
         1. // Necessaire pour envoi de mails depuis le serveur (erreurs, logs, etc.)
         2. Config fail2ban pour envoi de mail approprié
         3. fail2ban config > ban_action : action_mwl (mail with logs en cas de ban)
   7. [Iptables](https://www.grafikart.fr/tutoriels/iptables-694)
      1. ✅ Règles de base
      2. ✅ Autoriser [apt-get](https://www.grafikart.fr/tutoriels/iptables-694#c44945)
      3. ✅ Autoriser [monitoring ovh](https://docs.ovh.com/fr/dedicated/monitoring-ip-ovh/)
      4. 🌱 Avec un validate
   8. 🚧♻️ Mise à l'heure du serveur
      1. Ubuntu [doc officielle](https://help.ubuntu.com/lts/serverguide/NTP.html)
      2. 🚧 Firewall / Autoriser Mise à l'heure du serveur [NTP](https://www.google.com/search?q=ntp)
   9. ✅ [fail2ban](https://www.grafikart.fr/tutoriels/fail2ban-698)
      3. ✅ Recos grafikart
      4. ✅ Recos archi linux
   10. 🔍♻️ Reprendre la vidéo de cocadmin sur la sécurité
3. Installation de docker
   1. iptables firewall > docker [needs update](https://github.com/nickjj/ansible-iptables/blob/master/tasks/main.yml)
4. Installation de traefik
5. Mettre en place un nginx hello world sur un DNS
   1. HTTPS Automatique / Let's Encrypt

## 🚧 WIP 🚧

**Mise en place de la synchro du temps** > changer la timezone ET qu'elle persiste au reboot

- [Ubuntu Time Synchronization](https://help.ubuntu.com/lts/serverguide/NTP.html)
- [Tuto > How To Set Up Time Synchronization on Ubuntu 18.04](https://www.digitalocean.com/community/tutorials/how-to-set-up-time-synchronization-on-ubuntu-18-04)
- [Tuto > Keep Your Clock Sync with Internet Time Servers in Ubuntu 18.04](https://vitux.com/keep-your-clock-sync-with-internet-time-servers-in-ubuntu/)
- [Ansible timezone module](https://docs.ansible.com/ansible/latest/modules/timezone_module.html)
- [Ansible cookbook > ansible-clock](https://github.com/fabiocorneti/ansible-clock)


## Priorisation, détails tâche courante

- 🌱 fail2ban > [securité++](https://wiki.archlinux.org/index.php/Fail2ban#Service_hardening)

## Tests

- ✅ Multiples hosts
- ✅ Accès machine locale
- ✅ Génération complète de première clé SSH
- ✅ Génération automatique des clés SSH des autres utilisateurs (sans ajout à l'agent)
  - ✅ Générer le fichier users/README_secret.md automatiquement, comme pour root
- ✅ Fix installation zsh : une pour root, une pour les autres utilisateurs
- ✅ Accès root avec nouvel utilisateur généré *the_builder_guy*
- ✅ Changement du port SSH custom avant reco
  - ✅ !!! Ajout nouvel utilisateur a l'agent local
- ✅ FIXer auto update OS

- fail2ban [autoriser nginx port 80](https://unihost.com/help/how-to-protect-a-server-with-fail2ban/)