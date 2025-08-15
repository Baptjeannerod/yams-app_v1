# Yam’s — Score & Classement (PWA)

Application Web pour saisir les scores du Yam’s (Yahtzee) et obtenir un **classement instantané**.
- Saisie fluide (pas de perte de focus)
- Limites de score par catégorie (ex: 1× ≤ 6, Full = 25, etc.)
- Bonus automatique (+35 si 1→6 ≥ 63)
- Export / Import JSON
- **PWA installable** (icône, plein écran, offline)
- iPad-friendly (grands boutons, pas de zoom auto)

## Déploiement rapide sur GitHub Pages

1. Crée un nouveau dépôt **public** sur GitHub (ex: `yams-app`).  
2. Téléverse ces fichiers à la racine : `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`, `.nojekyll` (et ce README).
3. Dans **Settings → Pages** :  
   - *Build and deployment* → **Source** = `Deploy from a branch`  
   - **Branch** = `main` / **root** (ou `master` selon ton dépôt)  
4. Attends l’URL de mise en ligne (ex: `https://<ton-user>.github.io/yams-app/`).  
5. Ouvre l’URL sur l’iPad → **Partager** → **Sur l’écran d’accueil**.

> Alternative: utilise `user.github.io` (Pages “utilisateur”) et place les fichiers à la racine du dépôt.

## Déploiement via Git en ligne de commande

```bash
# 0) Décompresse le zip et entre dans le dossier
unzip yams_github_pages_bundle.zip -d yams-app
cd yams-app

# 1) Initialise Git
git init
git add .
git commit -m "Initial commit: Yam’s PWA"

# 2) Ajoute la remote (remplace TON-USER et yams-app par tes valeurs)
git branch -M main
git remote add origin git@github.com:TON-USER/yams-app.git

# 3) Push
git push -u origin main
```

Ensuite, active GitHub Pages comme décrit ci-dessus.

## Arborescence
```
.
├─ index.html
├─ manifest.webmanifest
├─ sw.js
├─ icon-192.png
├─ icon-512.png
├─ .nojekyll
└─ README.md
```

## Notes techniques
- Le service worker met en cache l’app shell pour un usage hors-ligne.  
- En cas de mise à jour, pense à **rafraîchir** (ou désinstaller/réinstaller sur l’écran d’accueil) si nécessaire.
- Les données (scores) sont stockées en `localStorage` — indépendantes par navigateur/appareil.
