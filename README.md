# Earnlix Africa

Landing page one-page pour Earnlix Africa Community — communauté africaine dédiée au marketing digital, à l'IA, au trading et à l'e-commerce via Earnlix Digital.

**Site en ligne :** https://earnlix-africa.netlify.app

## Structure

- `index.html` — page unique (HTML/CSS/JS), aucune étape de build nécessaire.
  - Police via Google Fonts (Syne, Inter)
  - Animation 3D du hero via [Three.js](https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js) (CDN)
  - Canvas réseau de particules pour la section communauté
  - Typewriter, scroll-reveal, tilt 3D sur les cartes, FAQ accordéon, formulaire de contact vers WhatsApp — tout en vanilla JS
  - Google Analytics (gtag.js)
- `404.html` — page d'erreur personnalisée (servie automatiquement par Netlify)
- `netlify.toml` — configuration de déploiement : en-têtes de sécurité (CSP, HSTS, X-Frame-Options...) et cache long terme sur les images
- `robots.txt` / `sitemap.xml` — référencement
- `og-image.jpg` — image d'aperçu pour le partage sur WhatsApp/Facebook/Twitter
- `95217.webp`, `favicon*.png/ico`, `apple-touch-icon.png` — logo et icônes
- `illus-*.webp`, `avatar-*.webp` — illustrations des sections (Formations, À Propos, Témoignages)

## Déploiement sur Netlify

Ce projet est un site statique, aucun build n'est requis.

1. Pousse ce dépôt sur GitHub (déjà fait si tu lis ceci depuis le repo).
2. Sur [netlify.com](https://app.netlify.com), clique sur **Add new site → Import an existing project**.
3. Connecte ce dépôt GitHub.
4. Laisse les réglages de build par défaut (site 100% statique) :
   - Build command : *(vide)*
   - Publish directory : *(racine `.`)*
5. Clique sur **Deploy site**.

Netlify applique automatiquement les en-têtes définis dans `netlify.toml` (sécurité + cache) et sert `404.html` pour toute page introuvable.

## Développement local

Aucune dépendance n'est requise. Ouvre simplement `index.html` dans un navigateur, ou sers le dossier avec n'importe quel serveur statique, par exemple :

```bash
npx serve .
```
