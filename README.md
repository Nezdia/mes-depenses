# Mes Dépenses

Application de suivi des dépenses (PWA), installable sur iPhone, fonctionne hors ligne.
Les données restent uniquement sur le téléphone (IndexedDB).

## Fichiers
- `index.html` : toute l'application (HTML, CSS, JavaScript)
- `sw.js` : service worker (hors ligne). Changer `CACHE` après modification de sw.js, du manifest ou des icônes.
- `manifest.webmanifest` : nom, couleurs, icônes de l'app
- `seed.json` : historique importé depuis l'Excel (mai à octobre 2026), chargé au premier lancement
- `icons/` : icônes de l'app

## Mise à jour
Modifier `index.html`, pousser sur GitHub. À la prochaine ouverture avec du réseau, l'iPhone récupère la nouvelle version
(ferme et rouvre l'app une fois si besoin). Les données ne sont pas touchées.
