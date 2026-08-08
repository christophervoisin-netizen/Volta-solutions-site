VoltaSite V5.8 - Correctif SEO technique Search Console

Base : V5.7 fournie le 08/08/2026.

Modifications ciblées :
- Ajout des balises canonical auto-référentes sur mentions-legales.html et politique-confidentialite.html.
- Ajout de _redirects : /index.html -> / en redirection permanente 301.
- Ajout/mise à jour de sitemap.xml avec uniquement les URL canoniques https://voltasolutions71.fr/ sans www.
- robots.txt conservé et cohérent avec le sitemap canonique.
- Ajout au paquet des 2 pages services référencées par l'accueil : tableau-renovation-electrique-louhans.html et solutions-energetiques-louhans.html.
- Conservation des pages V5.7, Analytics, consentement, formulaire, téléphone, WhatsApp et informations Allianz.

IMPORTANT DÉPLOIEMENT :
- Ce paquet reste un PACK DE MISE À JOUR : ne supprimez pas style.css, site-update-v57.css, les logos, favicon, apple-touch-icon ni les photos déjà en ligne.
- Copier/remplacer les fichiers de ce paquet à la racine du projet.
- La redirection www -> sans www doit être configurée au niveau Cloudflare (Redirect Rule/Bulk Redirect), car un fichier _redirects de Pages ne permet pas de fiabiliser à lui seul une redirection conditionnée par le hostname.
- Cible unique recommandée : https://voltasolutions71.fr/$1
- Après déploiement : tester https://voltasolutions71.fr/index.html (doit arriver directement sur https://voltasolutions71.fr/) et les variantes www.
- Puis renvoyer https://voltasolutions71.fr/sitemap.xml dans Google Search Console.
