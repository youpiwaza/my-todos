# Contenus importants mais ne pas polluer TODO simple

cocadmin / Sécuriser son serveur comme la NSA
https://www.youtube.com/watch?v=UmbndsZFIUE

- Utiliser les utils de sécurité
  - SELinux
    - Droits d'accès des programmes aux ressources
- Limiter les droits et accès au strict minimum

Concrètement

1. Clé ssh pour se connecter
2. Autre utilisateur que root
  - `adduser LENOM`
  - `usermod -aG sudo LENOM`
  - Ne pas utiliser de noms génériques (root, admin, etc.)
3. Modifier les privilèges sudo
  - `visudo` // accéder au ficher de conf sudo
4. Mises a jour
  - `apt-get update && apt-get upgrade -y` // maj listes packets et installation avec "oui" à toutes les questions
  - Recommandé : tous les jours // cron ?
5. Rendre publique uniquement ce qui doit l'être, sinon réseau privé // traefik ?
  - Machine SSH publique pour accès au réseau privé (uniquement serveur ssh)
    - Désactiver OpenSSH
    - `vi /etc/ssh/sshd_config`
    - cf. vidéo https://youtu.be/UmbndsZFIUE?t=750
      - `PermitRootLogin no`
      - `UsePAM no`
      - `PasswordAuthentication no`
    - Relancer le service SSH pour prendre en compte la conf
6. Bannir ips qui tentent de brute force
  - `apt-get install fail2ban -y` // installation
  - `vi /etc/fail2ban/jain.conf` // configuration
    - `maxretry = 15`
7. Changer le port SSH par défaut (virer 22) // Préviens une partie du spam
8. Ajouter un firewall, plus connu : iptable
  - Fermer tous les ports, excepté le port SSH
    - `iptable -A INPUT -i eth0 -p tcp --dport 22 -m state --state NEW,ESTABLISHED -j ACCEPT` // entrée
    - `iptable -A OUTPUT -0 eth0 -p tcp --sport 22 -m state --state ESTABLISHED -j ACCEPT` // sortie
    - ` iptables -P INPUT DROP` // Enpécher tout le reste
9. Mettre en place des backups
  - Manuels, en cas de grosse maj
  - Automatiques, régulièrement (par jour ou semaine)
    - Avec un système de purge (1 mois max ?)
  - Tester le backup, régulièrement !
10. Protéger l'accès physique à la machine
  - Mot de passe BIOS
  - Désactiver USB