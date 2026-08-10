VoltaSite V5.10 - Correctif définitif URL Cloudflare Pages / Google Search Console

Base : V5.8 réellement déployée et fournie le 09/08/2026.

CAUSE CONFIRMÉE :
- Cloudflare Pages redirige automatiquement les fichiers HTML publics vers leur URL sans extension : /page.html -> /page.
- La V5.8 indiquait encore les URL .html dans le sitemap, les balises canonical, les données structurées et les liens internes.
- Google recevait donc des URL annoncées comme canoniques qui redirigeaient, ce qui a déclenché les erreurs de redirection dans Search Console.

CORRECTIONS V5.10 :
- Sitemap entièrement harmonisé avec les 9 URL finales sans .html.
- Balises rel=canonical des pages services et légales passées sur les URL finales sans .html.
- URL des données structurées Service/Breadcrumb harmonisées sans .html.
- Liens internes de la page d'accueil, des pages services, du footer et des pages légales passés sur les URL finales sans .html.
- Les retours vers l'accueil utilisent / et les liens devis depuis les pages services utilisent /#devis.
- Les fichiers physiques restent nommés .html : c'est normal et nécessaire au déploiement statique ; seule l'URL publique est sans extension.
- _redirects conservé : /index.html -> / en 301.
- _headers, Analytics, consentement, formulaire, téléphone, WhatsApp, assurance Allianz, design et contenu conservés.
- robots.txt conserve https://voltasolutions71.fr/sitemap.xml.

CLOUDFLARE :
- Conserver la Redirect Rule www -> domaine racine déjà créée dans le tableau de bord Cloudflare.
- Ne pas créer de règle supplémentaire pour enlever .html : Cloudflare Pages le fait nativement.

APRÈS DÉPLOIEMENT :
1. Vérifier que https://voltasolutions71.fr/electricite-generale-louhans répond directement comme URL finale.
2. Ouvrir https://voltasolutions71.fr/sitemap.xml et vérifier qu'aucune URL ne contient .html.
3. Renvoyer https://voltasolutions71.fr/sitemap.xml dans Search Console.
4. Inspecter UNE URL finale sans .html, puis demander l'indexation si nécessaire.
5. Relancer ensuite la validation du problème « Erreur liée à des redirections ».

IMPORTANT DÉPLOIEMENT :
- Pack de mise à jour : ne pas supprimer style.css, site-update-v57.css, logos, favicon, apple-touch-icon ou photos existantes.
- Copier/remplacer les fichiers du paquet à la racine du projet.
