# Canvas Preview · Spotify

Aperçu **pixel-perfect** pour vos visuels **Spotify Canvas** : chargez votre vidéo, visualisez-la dans une maquette de téléphone fidèle à l'app Spotify, et vérifiez le rognage par rapport au cadre de référence **1080 × 1920 (9:16)** avant publication.

Outil **100 % statique** : une seule page HTML, sans dépendance, sans serveur. Tout le traitement se fait dans votre navigateur — **aucune vidéo n'est envoyée en ligne**.

## ▶️ Démo en ligne

Une fois publié sur GitHub Pages :

```
https://<votre-utilisateur>.github.io/<votre-depot>/
```

## ✨ Fonctionnalités

- Maquette de téléphone fidèle (mini-lecteur + plein écran) pour juger le rendu réel.
- Cadre de référence **1080 × 1920 · 9:16** avec visualisation du **rognage** selon le ratio choisi.
- Rappel des contraintes Spotify Canvas : boucle **3–8 s**, **MP4 / WebM**, **< 50 Mo**.
- Carte de rognage sur le cadre complet pour repérer les zones perdues.
- Aucune installation : ouvrez `index.html` ou la page GitHub Pages.

## 🚀 Utilisation locale

Ouvrez simplement `index.html` dans un navigateur moderne. Aucune étape de build n'est nécessaire.

## 📦 Publier sur GitHub Pages

1. Créez un dépôt GitHub et poussez ce dossier :
   ```bash
   git add .
   git commit -m "Canvas Preview · Spotify"
   git branch -M main
   git remote add origin https://github.com/<votre-utilisateur>/<votre-depot>.git
   git push -u origin main
   ```
2. Dans le dépôt : **Settings → Pages**.
3. Sous **Build and deployment**, choisissez **Deploy from a branch**.
4. Sélectionnez la branche **`main`** et le dossier **`/ (root)`**, puis **Save**.
5. Patientez ~1 min : la page sera servie depuis `index.html` à l'URL ci-dessus.

## 📄 Licence

Distribué sous licence MIT — voir [LICENSE](LICENSE).
