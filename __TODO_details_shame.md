# Contenus importants mais ne pas polluer TODO simple

## Serveur

Healthcheck example

Possibilité d'appeler un script pré-fait en cas d'echec (au lieu de [exit 1](https://www.udemy.com/course/docker-for-beginners/learn/lecture/14002044#overview), go envoyer un mail)

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

---

- [Utiliser ARG pour stocker les versions](https://www.udemy.com/course/docker-essentials/learn/lecture/12339826#overview)
- [Utiliser ENV](https://www.udemy.com/course/docker-essentials/learn/lecture/12339842#overview)
- Utiliser Config

---

## Sécurité

Sécurités SSL/TLS (Transport Layer Security / https) >
   Privilégier TLS 1.3 (le reste **deprecated** a part TLS 1.2)
   Doit être enregistré auprès d'une autorité de confiance > [liste française](https://webgate.ec.europa.eu/tl-browser/#/tl/FR)
   Privilégier les certificats courts (1 a 3 mois) au cas ou le serveur serait compromis (et possibilité de résilier un certif manuellement)
   Favoriser le mutual Auth
   Automatiser avec Let's encrypt
