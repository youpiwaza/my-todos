# Contenus importants mais ne pas polluer TODO simple

## Serveur

cocadmin / [Sécuriser son serveur comme la NSA](https://www.youtube.com/watch?v=UmbndsZFIUE)

- Utiliser les utils de sécurité
  - SELinux / AppArmor
    - Droits d'accès des programmes aux ressources
  - grsec
  - egress / Restrict network access
- Limiter les droits et accès au strict minimum

Concrètement

1. Modifier les [privilèges sudo](https://youtu.be/UmbndsZFIUE?t=390)
   - `visudo` // accéder au ficher de conf sudo
2. Rendre publique uniquement ce qui doit l'être, sinon réseau privé // traefik ?
   - Machine SSH publique pour accès au réseau privé (uniquement serveur ssh)
      - Désactiver OpenSSH
      - `vi /etc/ssh/sshd_config`
      - cf. [vidéo](https://youtu.be/UmbndsZFIUE?t=750)
         - `PermitRootLogin no`
         - `UsePAM no` // Attention ça empêche la connexion SSH ?
         - `PasswordAuthentication no`
      - Relancer le service SSH pour prendre en compte la conf
3. Mettre en place des backups
   - Manuels, en cas de grosse maj
   - Automatiques, régulièrement (par jour ou semaine)
      - Avec un système de purge (1 mois max ?)
   - Tester le backup, régulièrement !

## Docker

cocadmin / [Docker Hacké ! Analyse de la faille CVE-2019-5736](https://www.youtube.com/watch?v=Ktud3FDkKcE)

Bonne pratique Dockerfile

- Toujours utiliser un utilsateur dédié !

```yaml
FROM ...
RUN ...
USER pasRoot
```

---

Healthcheck example

```yml
  daServiceQuiTapeSurDeuxPoints3000:
    healthcheck:
      test: ["CMD", "curl", "-f", "http://localhost:3000"]
      interval: 5s
      timeout: 1s
      retries: 5
 ```

 Possibilité d'appeler un script pré-fait en cas d'echec (au lieu de [exit 1](https://www.udemy.com/course/docker-for-beginners/learn/lecture/14002044#overview), go envoyer un mail)

---

Limiter les ressources allouées

```yml
  daService
    deploy:
      resources:
        limits:
          memory: 128M
        reservations:
          memory: 64M
```

---

cocadmin / [Erreurs à éviter avec Docker et les conteneurs](https://www.youtube.com/watch?v=XPmmlqTgKGI)

- 1 conteneur par stack (ex: Ne pas lancer 1 conteneur avec un apache ET un sql)
- Ne pas accéder au conteneur pour modifier la conf > Modifier la conf et relancer le conteneur (sinon conf perdue au reboot)
- Ne pas créer d'images différentes dev/prod > Utiliser des variables de conf
- Dev > ne pas build systématiquement les images, utiliser les volumes
- Prod > Ne pas laisser les outils de dev a l'intérieur
  - Images plus grosse que nécessaire
  - Risques de sécurité
  - Solution : multi stage build : Créer l'image prod a partir des artéfacts de l'image de dev
- Ne pas stacker les commandes RUN (création d'autres layer)
  - Solution : Utiliser && dans la même commande RUN
- Spécifier la version de l'image de base (instruction FROM)

---

Docker for web hosting

[Bonnes pratiques](https://forums.docker.com/t/shared-web-hosting-with-docker-best-practices/7893)

- Ne jamais faire tourner les conteneurs via `root`, toujours utiliser `USER` (ajout d'utilisateurs)
- Utiliser AppArmor
- Utiliser grsec
- Utiliser SELinux
- Restrict network access (e.g. egress) in running containers as much as possible
- Look into --cap-drop and drop the caps those containers won’t need
  - [Docker container capabilites](https://opensource.com/business/15/3/docker-security-tuning)
- Do not allow anyone access to the Docker API or CLI
- Do not bind mount files to/from the host
  - Utiliser `volume` et non `links`
  - Passer par un serveur FTP dans son propre conteneur [Go](https://forums.docker.com/t/shared-web-hosting-with-docker-best-practices/7893/4?u=youpiwaza)
- Stay on top of CVEs, especially for the Linux kernel itself
  - Common Vulnerabilities and Exposures (CVE)
  - [Linux](https://www.google.com/search?q=linux+CVEs)
  - [Ubuntu](https://www.google.com/search?q=ubuntu+CVEs)

---

- [Utiliser ARG pour stocker les versions](https://www.udemy.com/course/docker-essentials/learn/lecture/12339826#overview)
- [Utiliser ENV](https://www.udemy.com/course/docker-essentials/learn/lecture/12339842#overview)

---

docker multi stage build
