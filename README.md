# summit-nasto-page

Landing pages des M&C Summits, produites par Nasto International Kft. Une édition par sous-dossier, la racine redirige vers l'édition en cours.

- URL : https://summit.nasto.hu (racine → redirection /dubai/)
- Édition courante : https://summit.nasto.hu/dubai/ (25-28 novembre 2026)
- Hébergement : GitHub Pages (branche main, racine), HTTPS Let's Encrypt
- DNS : CNAME summit.nasto.hu -> louischnv.github.io (zone Netim)
- Charte : M&C (Noe Display + Inter auto-hébergées, navy #0C1B2A, orange #A5522A), CSS sur mesure dans assets/styles.css
- Tracking : pixel Meta dataset « Summit Dubaï » (1591286586126927), chargé uniquement après consentement (bandeau cookies). Événement Lead déclenché à la soumission du Typeform (postMessage form-submit).

## Variables à remplir dans dubai/index.html (bloc script en bas)

- `TYPEFORM_ID` : l'ID du formulaire Typeform (ex. `AbCdEf12`). Tant qu'il est vide, un fallback email s'affiche.
- `VSL_EMBED_URL` : URL d'embed de la VSL (ex. YouTube non répertorié `https://www.youtube.com/embed/XXXX`). Tant qu'elle est vide, la section VSL est masquée.

## Nouvelle édition

Dupliquer `dubai/` vers `[ville]/`, adapter le contenu et le dataset pixel, puis changer la redirection racine dans `index.html`.
