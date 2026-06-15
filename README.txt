VoltaSite V4.3.0 - Volta Solutions 71 SEO + Logo propre

Recherche approfondie réalisée à partir de la V4.2.4 stable.

Conservé :
- Galerie Premium avec filtres Électricité / Photovoltaïque / Stockage / Borne
- Lightbox plein écran
- Formulaire de demande de devis
- Halos lumineux et animations
- Photos de réalisations
- Pages légales
- Footer premium
- Structure mobile existante

Modifié :
- Nom harmonisé en Volta Solutions 71 sur le site, les pages légales et les métadonnées.
- Hero remplacé par un logo/wordmark propre, sans effet "carte de visite flottante".
- Conservation du halo orange/doré autour de l'identité visuelle.
- Titre SEO optimisé : électricien Louhans, photovoltaïque, domotique, IRVE.
- Meta description enrichie pour le référencement local.
- Open Graph / Twitter Card améliorés pour les partages.
- JSON-LD Electrician corrigé avec Volta Solutions 71 et https://voltasolutions71.fr.
- robots.txt et sitemap.xml basculés sur https://voltasolutions71.fr.

À faire après mise en ligne :
- Vérifier que Cloudflare est actif.
- Connecter le Worker au domaine voltasolutions71.fr.
- Valider Google Search Console avec le TXT Cloudflare.
- Envoyer sitemap.xml dans Search Console.
- Remplacer l'email Outlook par contact@voltasolutions71.fr quand l'adresse pro sera configurée.


VoltaSite V4.4.0 - Formulaire de devis direct + photos

Modifié dans cette version :
- Remplacement de l'ancienne adresse email par adresse professionnelle configurée dans index.html, mentions légales, politique de confidentialité et données structurées.
- Remplacement du fonctionnement mailto par un vrai formulaire intégré au site via FormSubmit.
- Envoi direct au clic sur le bouton, sans ouvrir la boîte email du visiteur.
- Ajout d'un champ de pièces jointes/photos facultatif : images et PDF, sélection multiple.
- Ajout d'un message de confirmation après retour sur le site.
- Mise à jour de la politique de confidentialité pour mentionner les photos/documents et le service technique d'envoi du formulaire.

Important après mise en ligne :
- Faire un premier test depuis le formulaire du site.
- Au premier envoi, FormSubmit peut envoyer un email de confirmation/activation à adresse professionnelle configurée : cliquer sur le lien reçu pour activer définitivement la réception.
- Vérifier les spams lors du premier test.


VoltaSite V4.5.0 - Animation électrique + confirmation premium

Ajouté dans cette version :
- Animation électrique pendant l'envoi du formulaire de demande de devis.
- Bouton d'envoi bloqué pendant la transmission pour éviter les doubles clics.
- Message de confirmation premium après retour sur le site.
- Tentative d'accusé de réception automatique au client via le champ _autoresponse de FormSubmit.
- Conservation du formulaire direct avec photos/documents et envoi vers adresse professionnelle configurée.

Important :
- FormSubmit indique que l'accusé de réception automatique ne fonctionne pas si le reCAPTCHA est désactivé ou si le formulaire est envoyé en AJAX.
- Pour permettre l'accusé de réception client, la ligne _captcha=false a été retirée.
- Si FormSubmit affiche une étape anti-spam, c'est normal et c'est le compromis pour permettre l'accusé de réception automatique.
- Les fichiers joints restent limités par les règles FormSubmit : total maximum annoncé de 10 Mo.


VoltaSite V4.5.1 - Correctif animation visible + retour devis

Corrigé dans cette version :
- Ajout du CSS manquant pour l'animation électrique du formulaire.
- L'envoi du formulaire est maintenant retardé volontairement d'environ 1,2 seconde pour que l'animation soit réellement visible avant la redirection FormSubmit.
- Le bouton d'envoi est bloqué pendant la transmission pour éviter les doubles clics.
- Le message de confirmation premium reste affiché après le retour sur le site.
- Le retour automatique vers la section devis est renforcé après succès.

À savoir :
- L'accusé de réception automatique dépend de FormSubmit. Il peut arriver avec délai ou passer en spam côté client.
- Si l'accusé automatique ne part pas malgré _autoresponse, il faudra passer plus tard par une solution dédiée type Cloudflare Worker + service d'envoi email.


VoltaSite V4.5.6 - Sécurité formulaire stable
- Ajout d'un contrôle local avant envoi : fichiers JPG, PNG, WebP ou PDF uniquement.
- Blocage local si le total des pièces jointes dépasse 10 Mo, pour éviter la page d'erreur FormSubmit.
- Suppression de l'accusé de réception automatique FormSubmit au client, pour éviter un email qui ressemble à du spam.
- Obfuscation de l'adresse email dans les liens visibles et dans l'action du formulaire : cela masque l'adresse aux robots simples qui lisent le HTML.
- Suppression de l'email du JSON-LD public.
- Ajout d'un fichier _headers pour Cloudflare Pages avec HSTS, anti-sniffing, protection iframe, referrer policy, permissions policy et CSP adaptée au formulaire FormSubmit.

Important : pour un masquage encore plus fort, générer une clé Random String dans FormSubmit et remplacer l'action dynamique par cette clé officielle.


VoltaSite V4.6.4 - Version humaine Christopher Voisin conforme à la maquette

Réalisé à partir du ZIP original V4.5.6 stable fourni.

Modifié :
- Refonte de l’accueil en version plus humaine, proche de la maquette validée.
- Ajout de Christopher Voisin en titre principal.
- Ajout de la mention 20 ans d’expérience.
- Ajout d’une section À propos avec photo, écoute, transparence et durable.
- Ajout d’un bloc d’appel téléphonique rassurant.
- Ajout des fichiers christopher-voisin.jpg et christopher-voisin.webp optimisés.
- Conservation du formulaire sécurisé FormSubmit V4.5.6.
- Conservation de la galerie, lightbox, pages légales et headers Cloudflare.

Important :
- Remplacer tout le contenu de l’hébergement par ce dossier complet pour éviter les mélanges d’anciennes versions.
- Tester la version mobile et le formulaire après mise en ligne.
