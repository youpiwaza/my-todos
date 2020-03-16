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

1. Mettre en place la sécurité du serveur
   1. 🔍 Grafikart / Mise en place d'un serveur web
      1. 🌱 Envoi de mail / [Postfix](https://www.grafikart.fr/tutoriels/postfix-sendonly-695) ou [autre](https://www.ubuntupit.com/best-linux-mail-server-software-and-solutions/),
         1. // Necessaire pour envoi de mails depuis le serveur (erreurs, logs, etc.)
         2. Config fail2ban pour envoi de mail approprié
         3. fail2ban config > ban_action : action_mwl (mail with logs en cas de ban)
   2. [Iptables](https://www.grafikart.fr/tutoriels/iptables-694)
      1. 🌱 Avec un validate
   3. 🚧♻️ Mise à l'heure du serveur
      1. 🚨 systemctl status systemd-timesyncd > inactive dead
         1. [doc](https://www.digitalocean.com/community/tutorials/how-to-set-up-time-synchronization-on-ubuntu-18-04#controlling-timesyncd-with-timedatectl)
      2. 🚧 Firewall / Autoriser Mise à l'heure du serveur [NTP](https://www.google.com/search?q=ntp)
   4. 🔍♻️ Reprendre la vidéo de cocadmin sur la sécurité
2. Installation de docker
   1. iptables firewall > docker [needs update](https://github.com/nickjj/ansible-iptables/blob/master/tasks/main.yml)
3. Installation de traefik
4. Mettre en place un nginx hello world sur un DNS
   1. HTTPS Automatique / Let's Encrypt

## 🚧 WIP 🚧

hey

## Priorisation, détails tâche courante

REMPLACER NTP PAR CHRONY ???

- [Chrony faq](https://chrony.tuxfamily.org/faq.html)
- [Comparaison chrony vs ntp](https://chrony.tuxfamily.org/comparison.html)
- [timesyncd.conf](http://manpages.ubuntu.com/manpages/cosmic/man5/timesyncd.conf.5.html)
- [keep-your-clock-sync-with-internet-time-servers-in-ubuntu](https://vitux.com/keep-your-clock-sync-with-internet-time-servers-in-ubuntu/)

> Fin du comparatif : tester si implémentation rapide ( sudo nano /etc/systemd/timesyncd.conf ou mieux can be stored in /etc/systemd/timesyncd.conf.d/ ) sinon oseb go ntp
> Commenter ntp au cas ou

- Si zsh déjà installé, l'utiliser (afin de ne pas le virer en cas de reinstallation)
- Forcer la version d'ansible dans les fichiers de conf

## Tests

hey
