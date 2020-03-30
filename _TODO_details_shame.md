# Contenus importants mais ne pas polluer TODO simple

## Serveur

cocadmin / [Sécuriser son serveur comme la NSA](https://www.youtube.com/watch?v=UmbndsZFIUE)

1. Mettre en place des backups
   - Manuels, en cas de grosse maj
   - Automatiques, régulièrement (par jour ou semaine)
      - Avec un système de purge (1 mois max ?)
   - Tester le backup, régulièrement !

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

- Prod > Ne pas laisser les outils de dev a l'intérieur
  - Images plus grosse que nécessaire
  - Risques de sécurité
  - Solution : multi stage build : Créer l'image prod a partir des artéfacts de l'image de dev
  - Solution : Utiliser && dans la même commande RUN
- Spécifier la version de l'image de base (instruction FROM)

---

Docker for web hosting

[Bonnes pratiques](https://forums.docker.com/t/shared-web-hosting-with-docker-best-practices/7893)

- Do not allow anyone access to the Docker API or CLI
- Do not bind mount files to/from the host
  - Utiliser `volume` et non `links`
  - Passer par un serveur FTP dans son propre conteneur [Go](https://forums.docker.com/t/shared-web-hosting-with-docker-best-practices/7893/4?u=youpiwaza)

---

- [Utiliser ARG pour stocker les versions](https://www.udemy.com/course/docker-essentials/learn/lecture/12339826#overview)
- [Utiliser ENV](https://www.udemy.com/course/docker-essentials/learn/lecture/12339842#overview)

---
