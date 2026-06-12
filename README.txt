VoltaSite V4.5.3 - Correctif définitif formulaire + stabilité visuelle

Base utilisée : V4.4.0 stable, qui conservait le bon affichage du site.

Corrigé dans cette version :
- Restauration du style stable d'origine pour éviter les images zoomées et les textes cassés.
- Restauration du comportement visuel des choix de projet : toute la tuile devient dorée quand elle est sélectionnée.
- Restauration du bouton de retour en haut dans son style d'origine.
- Animation électrique conservée pendant l'envoi, mais sans bloquer le formulaire.
- Suppression du délai JavaScript qui pouvait provoquer le chargement infini.
- Message de confirmation premium après retour sur le site.
- Formulaire direct avec photos/documents conservé vers voltasolutions71@mail.fr.
- Tentative d'accusé de réception automatique client conservée via FormSubmit.

Important :
- Si l'accusé de réception automatique client ne part pas, cela dépend des limites de FormSubmit.
- Le message de confirmation sur le site reste fiable.
- Après mise en ligne, vider le cache Cloudflare et faire un hard refresh si l'ancien CSS reste affiché.
