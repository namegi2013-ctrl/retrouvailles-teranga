# Site — Les Retrouvailles de la Teranga Gabonaise

Programme de l'événement du 18 juillet 2026 (Salle Pelé, Stade d'Angondjé), avec QR code d'accès généré automatiquement.

## Contenu du dossier
- `index.html` — la page complète (autonome, aucune dépendance à installer)

## Déployer le site

### Option A — GitHub Pages (gratuit)
1. Crée un repo GitHub (ex: `retrouvailles-teranga`)
2. Ajoute `index.html` à la racine du repo
3. Dans Settings → Pages, choisis la branche `main` et le dossier `/root`
4. Le site sera en ligne à l'adresse : `https://<ton-utilisateur>.github.io/retrouvailles-teranga/`

Commandes :
```bash
cd site-teranga
git init
git add .
git commit -m "Site programme Retrouvailles Teranga Gabonaise"
git branch -M main
git remote add origin https://github.com/<ton-utilisateur>/retrouvailles-teranga.git
git push -u origin main
```

### Option B — Netlify (encore plus rapide)
1. Va sur https://app.netlify.com/drop
2. Glisse-dépose le dossier `site-teranga` (ou juste `index.html`)
3. Le site est en ligne en quelques secondes avec une URL type `xxxx.netlify.app`
4. Tu peux renommer le sous-domaine dans Site settings → Change site name

### Option C — Nom de domaine personnalisé
Si tu réserves un nom de domaine (`.com`, `.ga`...), relie-le à GitHub Pages ou Netlify dans les paramètres DNS (les deux plateformes expliquent la marche à suivre une fois le domaine ajouté dans leurs réglages).

## À propos du QR code
Le QR code affiché sur la page encode automatiquement l'URL de la page elle-même (`window.location.href`). Cela signifie :
- Tu n'as rien à régénérer manuellement
- Une fois le site déployé (Option A ou B), ouvre la page en ligne, fais une capture d'écran du QR code affiché, et utilise cette image sur tes invitations, affiches ou flyers.

## Modifier le contenu
Toutes les informations (dates, horaires, intervenants) sont dans `index.html`, à l'intérieur des balises `<div class="item">`. Aucun outil spécial n'est nécessaire — un simple éditeur de texte suffit.
