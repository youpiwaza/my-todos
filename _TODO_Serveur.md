# Certaines tâches à ranger concernant le serveur / les sites vanilla

## Wordpress setup > Manual steps

1. DNS
   1. Ajouter A
   2. Ajouter MX > SPF/DKIM/DMARC
2. Copier les fichiers générés + pw sur un repo privé avec arbo
3. docker exec WP-CLI
4. Site language
5. Manage plugins
   1. Supprimer
      1. hello-dolly
      2. Bitnami Production Console Helper
      3. Jetpack
   2. Plugins
      1. 💩 VERIFIER QUE CA RAJOUTE PAS DE LA MERDE DANS LA CONSOLE
      2. Activer les plugins déjà présents
         1. Akismet Anti-Spam
            1. Besoin de création d'un compte
         2. All in One SEO Pack
            1. Régler le schéma (Infos fournies moteurs de recherche)
         3. 💩 AMP / "Accelerated Mobile Pages"
            1. Passer en mode standard
            2. 📌 Flingue pagespeed > Confirmé ça explose les résultats 💩 (100 > 65 en mobile)
         4. MonsterInsights - Google Analytics pour WordPress
            1. Besoin d'un compte GA et surement d'autres manip
         5. Simple Tags
         6. W3 Total Cache
            1. Besoin de modifier wp-config.php ! (fait avec docker run alpine /bin/ash), cf. fin de  ce fichier
            2. Performances > Paramètres généraux > Activer tous les systèmes de cache nécessaires (! CDN & Reverse proxy & Tracking)
               1. [Recos](https://onlinemediamasters.com/w3-total-cache-settings/)
               2. Ne pas mettre le lazy loading, il déconne
               3. Performances > Minifier > JS > Defer (plutôt que async)
            3. Performances > Mise en cache objet > Activer pour wp-admin/
            4. Les règles de caches sont ~KO, a revoir
            5. Besoin de repasser sur chaque putain de catégorie > Faire une fois & exporter, puis importer nouvelles install
      3. Installer les plugins requis
         1. Check Email
            1. Vérifier le bon envoi des emails depuis WP
         2. (Optimisation des images, si possible WEBP)
            1. ShortPixel Image Optimizer
               1. Besoin d'inscription et clé API
               2. Seems ~OK, mais limité par mois (100 credits images en tout, 1 image = 4-5 crédits avec miniatures )
         3. Heartbeat Control
            1. Disable all
         4. Wordfence security plugin
            1. Wordfence > Scan > Start new scan > tout goude
         5. Html sitemaps / Simple Sitemap – Create a Responsive HTML Sitemap
         6. RGPD
      4. MAJ tous les plugins
6. Utilisateurs > Votre profil > Prénom Nom
7. Réglages > Général > Langue > Français
8. Create clients' admin redactors
   1. Manage Admin display (remove menus theme/plugins, etc.)
9. Supprimer page et articles d'exemple
10. Create secondary pages
    1. Mentions légales
    2. Crédits
    3. Sitemap
    4. Politique de confidentialité, [exemple WP](https://dev.champagne-didier-lapie.com/wp-admin/privacy-policy-guide.php)
    5. Boite à outils (liste balises pour tester rendu)
11. Create secondary menu
    1. Affect secondary pages
12. ~~Réglages > Permaliens~~
13. Outils > Santé du site [ex](https://dev.champagne-didier-lapie.com/wp-admin/site-health.php)
     1. Supprimer les thèmes inutiles
     2. MAJ thème utilisé
14. Recos pagespeed [ex](https://developers.google.com/speed/pagespeed/insights/?hl=fr&url=https%3A%2F%2Fdev.champagne-didier-lapie.com%2F)
     1. Trop rien a faire une fois AMP & W3 Total Cache activés ET configurés
15. Recos Slow admins
     1. Heartbeat Control
16. Virer/Opti police alakon theme
17. Virer footer "propulsé par WordPress"
