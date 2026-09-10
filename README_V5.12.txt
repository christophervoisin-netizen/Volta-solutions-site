Volta Solutions 71 — V5.12 Navigation + logo officiel + audit
Date : 10/09/2026
Base : V5.11 fournie par Christopher.

OBJECTIF
- Rendre les pages service moins "isolées" sans les surcharger.
- Donner un accès évident à l’accueil, à la présentation de Christopher, aux réalisations et aux avis.
- Remplacer les CTA "Appeler Christopher" par une formulation commerciale Volta Solutions 71.
- Utiliser le logo officiel fourni le 10/09/2026.
- Conserver un seul formulaire de devis, avec le service d’origine présélectionné.

MODIFICATIONS
1. Navigation des pages service
- Ajout d’une navigation rapide : Accueil • Qui suis-je ? • Réalisations • Avis clients • Demander un devis.
- Le lien "Qui suis-je ?" arrive directement sur la zone de présentation de l’accueil.
- Les pages restent courtes et orientées conversion ; les contenus de confiance restent centralisés sur l’accueil.

2. Devis
- Les boutons de devis des pages service passent par une URL du type /?projet=borne#devis.
- Le formulaire de l’accueil présélectionne automatiquement le bon service.
- Aucun deuxième formulaire n’a été créé : maintenance et suivi restent simples.

3. Appels
- "Appeler Christopher" devient "Appeler Volta Solutions 71".
- Sur la page dépannage, "Appeler pour un dépannage" est conservé car plus pertinent pour l’intention utilisateur.

4. Logo
- logo-volta-solutions-71.png = logo officiel complet fourni par Christopher.
- logo-volta-solutions-71-symbol.png = recadrage du symbole officiel uniquement, utilisé dans les petites zones de navigation pour rester lisible.
- Aucun symbole n’a été redessiné.

5. CSS
- Ajout de site-update-v512.css, chargé après site-update-v57.css.
- Couche additive uniquement : elle ne remplace pas le design existant.
- Navigation adaptée aux petits écrans.

6. SEO / technique conservés
- Canonical sans .html.
- JSON-LD existant conservé.
- _redirects /index.html -> / 301 conservé.
- _headers conservé.
- sitemap.xml / robots.txt conservés depuis le pack V5.11.
- Aucun changement du périmètre d’assurance ou des prestations photovoltaïques.

IMPORTANT DÉPLOIEMENT
- Ce ZIP est un PACK DE MISE À JOUR, pas une copie de tous les assets du site.
- Conserver dans le projet Cloudflare : style.css, site-update-v57.css, photos, favicon, apple-touch-icon et les autres images déjà déployées.
- Copier/remplacer les fichiers présents dans ce pack à la racine du projet existant.
- Ajouter impérativement site-update-v512.css et les deux fichiers logo du pack.

CONTRÔLES EFFECTUÉS
- Un seul H1 par page.
- JSON-LD parseable.
- Pas d’identifiants HTML dupliqués.
- Pas de lien interne public en .html.
- Navigation des 6 pages service cohérente.
- Liens devis avec paramètre de présélection cohérent.
- Boutons "Appeler Christopher" supprimés.
- Logo officiel référencé sans supprimer les données de marque existantes.
