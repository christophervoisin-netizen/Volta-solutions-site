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
