# Digor — Commerces ouverts à Bréhat

> *Digor* signifie « ouvert » en breton.

Page personnelle listant les commerces de l'île de Bréhat (22870) avec leurs horaires du jour, une carte interactive et les numéros utiles.

Accessible sur : [https://didoune2026.github.io/digor/](https://didoune2026.github.io/digor/)

---

## Fonctionnement

Les horaires et informations des commerces sont récupérés en temps réel via l'API Google Maps (Places API). La navigation par jour permet de consulter les horaires d'un jour précis. Les marqueurs sur la carte sont cliquables.

Les informations complémentaires (transports, médecin, mairie, déchetterie) sont statiques et mises à jour manuellement dans le fichier `index.html`.

---

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | Page principale, contient tout le code HTML/CSS/JS |
| `blason-brehat.svg` | Blason de l'île de Bréhat, affiché dans le header et en favicon |
| `apple-touch-icon.png` | Icône 180×180px pour l'écran d'accueil iOS |
| `README.md` | Ce fichier |

---

## Configuration

La clé API Google Maps est placée à deux endroits dans `index.html` :

- `const API_KEY = 'VOTRE_CLE_API';` dans le bloc `<script>`
- `key=VOTRE_CLE_API` dans la balise `<script>` de chargement de la librairie Maps en bas de page

La clé est restreinte au domaine `didoune2026.github.io` dans Google Cloud Console.

---

## Commerces référencés

| Nom | Place ID Google |
|---|---|
| Le Pain de Sucre | ChIJIa8XaRMPEkgRvoTtwRKFp_A |
| L'Alegoat | ChIJkb12iAEQEkgRZf3zp0m3yvE |
| La Potinière | ChIJ1S-OIFUFEkgR6GQ8KzAVcMA |
| Le 22 | ChIJfadwMpwREkgR-CwE61MU_sU |
| Bellevue | ChIJ12oME6oaEkgR-puWcvDcVyk |
| Carrefour Market | ChIJkVtjPtIPEkgRqV5iZ68xJJA |
| Bréhat Services | ChIJ7d6eBQAREkgRlW_zdFzWCAM |
| La Bréhatine | ChIJtYImAcEPEkgRb323CQuX4E4 |
| Crech Kerio | ChIJL-c-ZAAQEkgRPR9uUZ7xFaQ |
| Shamrock | ChIJ58f9HP4PEkgROVRK9un-xZk |
| L'Archipel | ChIJO2e-OxwREkgRqNPkK9PXfRw |
| Les Verreries | ChIJqcr_VKgaEkgRjPTw_gzgsEQ |
| Dalibot | ChIJIdF3pwAQEkgRTz_6E8_Rtb8 |
| L'Equipage | ChIJ58f9HP4PEkgRq0lERbLX12c |
| L'Epicerie | ChIJNVgOAwIQEkgR6kTg5GyLQwc |

---

## Limites

Les horaires proviennent de Google Maps et peuvent être incomplets ou erronés, notamment pour les fermetures exceptionnelles. Ce projet est à usage personnel.
