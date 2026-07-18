VoltaSite V4.7.1 - Correctif galerie

- Correction définitive des filtres de la galerie réalisations.
- Les boutons Tout / Électricité / Photovoltaïque / Stockage / Borne masquent et affichent bien les cartes.
- Correction CSS empêchant .filtered-hidden d’être écrasé par .real-card display:flex.
- Photos forcées en affichage complet, sans crop/zoom.
- Lightbox masquée hors ouverture pour éviter les images parasites en bas de page.


V4.7.2 - Section Mon engagement enrichie
- Ajout d’une photo naturelle de Christopher dans la section Mon engagement.
- Ajout d’une promesse, de 3 valeurs et d’un appel direct.
- Conservation du formulaire, des filtres de galerie, du footer premium et des scripts existants.


VoltaSite V4.7.3 - Correctif confirmation formulaire
- Ajout du champ FormSubmit _autoresponse pour envoyer un email automatique au visiteur.
- Conservation du reCAPTCHA FormSubmit, car l'auto-réponse ne fonctionne pas si le captcha est désactivé.
- Conservation de l'envoi classique du formulaire, sans AJAX, car l'auto-réponse ne fonctionne pas avec un envoi AJAX.
- Message de succès sur le site enrichi après redirection vers ?devis=envoye#devis.
- Important : si FormSubmit affiche encore sa page de confirmation ou d'activation, vérifier que l'adresse voltasolutions71@mail.fr est bien activée dans FormSubmit en cliquant sur l'email de validation reçu.


VoltaSite V4.7.4 - Google Analytics
- Ajout de la balise Google Analytics 4 G-HGPQYC1PJX sur toutes les pages HTML.
- Ajout du Consent Mode v2 avec stockage Analytics refusé par défaut.
- Ajout d’un bandeau Accepter / Refuser.
- Mise à jour de la politique de confidentialité.
- Mise à jour de la Content-Security-Policy pour autoriser Google Analytics.


VoltaSite V5.0 - SEO local et conversion
- Base stable : V4.7.4 conservée (Analytics, consentement, formulaire, galerie et design premium).
- Ajout de 6 pages de services avec contenus uniques et liens internes.
- Ajout d’une FAQ visible et de données structurées FAQPage.
- Enrichissement des données structurées Electrician, WebSite, Service et BreadcrumbList.
- Ajout de robots.txt et sitemap.xml.
- Ajout d’un bloc local Louhans / communes voisines.
- Remplacement des faux avis anonymes par des engagements vérifiables, en attendant de vrais avis Google.
- Ajout du suivi Analytics des clics téléphone, email, devis et pages services.
- Conservation du style noir/orange, des photos, du formulaire FormSubmit et des correctifs précédents.
- Important : conserver dans le déploiement tous les fichiers images déjà présents sur le site.


VoltaSite V5.1 - Correctifs de finition
- Suppression du commentaire HTML mal encodé qui apparaissait en haut de la page.
- Remplacement du titre répétitif de la section Services.
- Réécriture de l'introduction de la section Services pour mieux la distinguer de Mon engagement.
- Correction des ancres avec scroll-margin-top / scroll-padding-top.
- FAQ refermée au chargement et limitée à une seule réponse ouverte à la fois.
- Renforcement CSS pour empêcher l'affichage d'une réponse lorsque son bloc details est fermé.
