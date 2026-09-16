# Earnlix Africa

Landing page one-page pour Earnlix Africa Community — communauté africaine dédiée au marketing digital, à l'IA, au trading et à l'e-commerce via Earnlix Digital.

## Structure

- `index.html` — page unique (HTML/CSS/JS), aucune étape de build nécessaire.
  - Police via Google Fonts (Syne, Inter)
  - Animation 3D du hero via [Three.js](https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js) (CDN)
  - Canvas réseau de particules pour la section communauté
  - Typewriter, scroll-reveal, tilt 3D sur les cartes, FAQ accordéon — tout en vanilla JS
- `vercel.json` — configuration de déploiement (URLs propres, pas de trailing slash)
- `95217.png` — logo Earnlix Digital (optionnel : la page fonctionne sans, l'image se masque automatiquement si absente)

## Déploiement sur Vercel

Ce projet est un site statique, aucun build n'est requis.

1. Pousse ce dépôt sur GitHub (déjà fait si tu lis ceci depuis le repo).
2. Sur [vercel.com](https://vercel.com), clique sur **Add New → Project**.
3. Importe ce dépôt GitHub.
4. Vercel détecte automatiquement un projet statique (**Framework Preset: Other**) :
   - Build Command : *(vide)*
   - Output Directory : *(racine `.`)*
5. Clique sur **Deploy**.

Le site sera en ligne en quelques secondes.

## Développement local

Aucune dépendance n'est requise. Ouvre simplement `index.html` dans un navigateur, ou sers le dossier avec n'importe quel serveur statique, par exemple :

```bash
npx serve .
```
