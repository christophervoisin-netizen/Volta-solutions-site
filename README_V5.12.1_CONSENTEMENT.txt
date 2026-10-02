Volta Solutions 71 — V5.12.1 Correctif Consent Mode v2 / Google Ads
Date : 02/10/2026
Base : V5.12 Navigation + logo + audit fournie par Christopher.

OBJECTIF
- Corriger le diagnostic Google Tag indiquant 0 % de consentement publicitaire.
- Conserver le refus par défaut avant tout choix utilisateur.
- Autoriser, après clic sur « Accepter », la mesure Google Analytics et Google Ads utile au suivi des campagnes.
- Ne PAS activer la personnalisation publicitaire ni le remarketing.

MODIFICATIONS
1. Consent Mode v2
- Par défaut : analytics_storage, ad_storage, ad_user_data et ad_personalization = denied.
- Après « Accepter » :
  analytics_storage = granted
  ad_storage = granted
  ad_user_data = granted
  ad_personalization = denied
- Après « Refuser » : les quatre restent denied.

2. Migration du consentement
- Nouvelle clé : voltaGoogleConsentV2.
- Un ancien REFUS est conservé automatiquement.
- Un ancien ACCORD Analytics seul n’est PAS étendu automatiquement à Google Ads : la nouvelle bannière est redemandée afin d’obtenir un consentement correspondant au nouveau périmètre.

3. Texte de la bannière
- Mention explicite de Google Analytics + Google Ads pour la mesure de fréquentation et des performances de campagne.
- Mention explicite que la publicité personnalisée / le remarketing ne sont pas activés.

4. Politique de confidentialité
- Mise à jour du paragraphe de mesure d’audience et publicitaire.
- Mise à jour de la clé de stockage local utilisée pour le choix.

5. Content-Security-Policy (_headers)
- Ajout des domaines Google recommandés pour les fonctionnalités Analytics liées à Google Ads et la mesure publicitaire.

DÉPLOIEMENT
- Déployer ce pack à la racine du site Cloudflare Pages en remplaçant les fichiers correspondants.
- Après déploiement, ouvrir le site en navigation privée et tester avec Tag Assistant.
- État attendu AVANT choix : 4 signaux en « Refusé ».
- État attendu APRÈS « Accepter » : analytics_storage, ad_storage et ad_user_data en « Accordé » ; ad_personalization reste « Refusé » volontairement.
- Le diagnostic Google peut demander un délai avant de se mettre à jour.
