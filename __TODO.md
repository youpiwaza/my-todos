# Taf en cours

Légende :

- 🚀  En cours / **1 MAX A LA FOIS**
- ✅  Terminé
- ⏩  Suite
- 📌 A tester
- ♻️  Contenus/notes dans TODO_details_shame.md
- 🔍  Lecture/Vidéos
- 🌱 TODO

**Tâches récurrentes** :

- Supprimer les terminés ✅ à chaque début/fin de semaine.
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
      5. 🌱 Importer des variables depuis un repo privé
2. Mettre en place la sécurité du serveur
   1. ✅ Create server repo & obfuscate vars
   2. ✅ Create a repo for Ansible role template
   3. ✅ Installation des logiciels de base sur le serveur
   4. ✅ Installation d'un utilisateur sur le serveur
      1. 🌱 Génération de la clé SSH de manière automatique (ansible > local_action)
      2. 🌱 Template de génération d'utilisateurs
   5. 🔍 Grafikart / Mise en place d'un serveur web
      1. ✅ Configration de VIM
      2. 🚀 CRONs / https://www.grafikart.fr/tutoriels/cron-tache-recurrente-1013
         1. ⏩ Faire un utilisateur dédié pour les crons
         2. Retirer les droits aux autres utilisateurs "cron.allow / cron.deny"
         3. Tester avec un cron cf. grafikart
   6. 🔍♻️ Reprendre la vidéo de cocadmin sur la sécurité
3. Installation de docker
4. Installation de traefik
5. Mettre en place un nginx hello world sur un DNS

## Priorisation, détails tâche courante

Grafikart

- CRON / https://www.grafikart.fr/tutoriels/cron-tache-recurrente-1013
- Shell / https://www.grafikart.fr/tutoriels/pimp-my-shell-750
- Iptables / https://www.grafikart.fr/tutoriels/iptables-694
- firewall / https://www.grafikart.fr/tutoriels/ufw-696
- fail2ban / https://www.grafikart.fr/tutoriels/fail2ban-698
