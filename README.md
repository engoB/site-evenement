# Site d'événement — clé en main

Un site de mariage (ou d'anniversaire, de baptême, de fête de famille) en une seule page,
élégant sur mobile comme sur ordinateur, **sans abonnement ni serveur**.

**Démo : https://engob.github.io/site-evenement/** — mot de passe invités : `demo`
(couple, lieux et témoins fictifs).

## Ce que ça fait

- **Écran d'accès** protégé par un mot de passe à donner aux invités, avec indice.
- **Notre histoire, le jour J** (compte à rebours, ajout à l'agenda Google / Outlook / Apple),
  **lieux** avec itinéraires, **programme** heure par heure, **témoins**.
- **RSVP** : présence, adultes / enfants, chanson préférée, allergies. Les réponses arrivent
  dans un Google Sheet (et par email) via un petit script Google Apps Script — sinon elles
  restent sur l'appareil de l'invité.
- **Tableau de bord des réponses** : qui vient, qui n'a pas répondu, export CSV.
- **Séjour** : où dormir, que faire dans la région, triés par budget.
- **Galerie**, **contact**, thème (couleurs, polices) personnalisable.
- **Mode édition** (`?edit=1`) : on modifie tous les textes, photos et sections directement
  dans la page, puis **Publier** envoie les changements sur GitHub Pages.

## Le personnaliser

1. Ouvrez la page avec `?edit=1` à la fin de l'adresse.
2. **Réglages** : prénoms, monogramme, date, lieu, date limite des réponses, mot de passe.
3. Cliquez sur n'importe quel texte ou photo pour le changer. **Thème** pour les couleurs.
4. **Publier** (jeton GitHub fine-grained limité au dépôt, permission *Contents : Read and write*),
   ou **Télécharger** le fichier et remplacez `index.html`.

Toute la configuration vit dans le bloc `<script id="site-config">` en haut de `index.html`.

## Confidentialité

Aucun compte, aucun traceur. Le jeton GitHub reste dans le navigateur de l'organisateur et
n'est jamais inclus dans le site publié. Les réponses des invités ne vont que dans le Google
Sheet des organisateurs.

---

Conçu et développé par [Sébastien Khai](https://engob.github.io/portofolio/) — tous droits réservés.
