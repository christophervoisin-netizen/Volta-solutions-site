Volta Solutions 71 — V5.11 Conversion + SEO local
Date : 10/09/2026
Base : V5.10 fournie par Christopher.

OBJECTIF
- Augmenter les appels et demandes de devis qualifiées sans refaire le design.
- Renforcer immédiatement l’intention locale « électricien / dépannage / tableau / borne ».
- Conserver les URL finales Cloudflare sans extension .html.

MODIFICATIONS PRINCIPALES
1. Accueil
- H1 remplacé par « Électricien à Louhans et alentours ».
- Premier écran orienté besoin client : panne, tableau, rénovation, recharge VE.
- Bouton d’appel placé en CTA principal ; devis en CTA secondaire.
- Preuve sociale mise à jour : 5,0/5 et 10 avis Google (vérifié le 10/09/2026).
- Services réordonnés : dépannage, électricité générale, tableaux/rénovation, recharge VE, domotique, solutions énergétiques.
- Meta title/description et Open Graph raccourcis et recentrés sur l’intention locale.
- Données structurées Electrician enrichies avec les services réellement proposés.
- Périmètre photovoltaïque clarifié dans la galerie : raccordements électriques / onduleurs / batteries selon assurance, sans pose des panneaux.
- Formulaire : retrait du champ _replyto incorrect ; attributs autocomplete ajoutés.
- Événement Analytics generate_lead ajouté après retour de formulaire réussi.

2. Page dépannage
- H1 et meta centrés sur « dépannage électrique Louhans ».
- Appel téléphonique en CTA principal.
- Week-end, dimanche et jours fériés mentionnés « selon disponibilité ».
- Processus adapté au dépannage : appel → diagnostic → accord client → remise en service.
- Règle « accord préalable avant remplacement matériel » intégrée.

3. Page borne de recharge
- Positionnement explicite « borne de recharge + prise renforcée ».
- Contenu plus proche des recherches client : tableau, puissance, protections, pilotage.
- FAQ simplifiée et cohérente avec l’étude électrique préalable.

4. Électricité générale / domotique
- Titles, descriptions et contenus clarifiés pour les recherches locales.
- Zones desservies détaillées dans les données structurées Service.

5. Sécurité / technique
- _headers conservé, mais HSTS corrigé : 1 an + includeSubDomains, sans token preload non nécessaire.
- _redirects conservé : /index.html -> / 301.
- sitemap.xml et robots.txt inclus avec les 9 URL finales sans .html.
- URLs canoniques existantes conservées.
- JSON-LD vérifié comme JSON valide.

IMPORTANT — PACK DE MISE À JOUR HTML + SEO
Les assets suivants n’étaient pas fournis dans ce lot et ne doivent PAS être supprimés du projet Cloudflare :
- style.css
- site-update-v57.css
- logos, favicon, apple-touch-icon
- photos / images de réalisations
- tout autre asset déjà présent

Les deux pages service non jointes au lot (tableau/rénovation et solutions énergétiques) ont été reconstruites à partir de leur version publique actuelle et du même gabarit V5.10, puis optimisées sans changer les classes CSS.

DÉPLOIEMENT
- Copier/remplacer uniquement les fichiers de ce pack à la racine du projet existant.
- Ne pas vider le projet avant l’upload si Cloudflare exige un dossier complet : dans ce cas fusionner ce pack avec le dossier complet actuel.
- Conserver la Redirect Rule www -> domaine racine déjà en place.

APRÈS DÉPLOIEMENT
1. Vérifier la page d’accueil sur mobile et ordinateur (H1, boutons Appeler/Devis, avis 10).
2. Vérifier /depannage-electrique-louhans et le bouton tel:.
3. Vérifier /borne-recharge-louhans.
4. Vérifier /sitemap.xml et /robots.txt.
5. Dans Search Console, renvoyer le sitemap puis inspecter l’accueil + la page dépannage.
6. Dans Google Business Profile, ne pas afficher l’adresse si aucun client n’est reçu sur place ; conserver les zones desservies exactes.
