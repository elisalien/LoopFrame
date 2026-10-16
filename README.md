# Loopframe

> Aperçu **pixel-perfect** pour vos visuels **Spotify Canvas** (et Motion Artwork Apple Music) : chargez votre vidéo, visualisez-la dans une maquette de téléphone fidèle à l'app, et vérifiez le rognage avant publication.

![Platform](https://img.shields.io/badge/platform-Web-informational) ![Stack](https://img.shields.io/badge/stack-HTML%20%2F%20CSS%20%2F%20JS-orange) ![License](https://img.shields.io/badge/license-MIT-green)

**[Ouvrir Loopframe](https://elisalien.github.io/LoopFrame/)**

## À propos

Loopframe montre comment un Canvas Spotify sera vraiment vu : dans l'écran « À l'écoute » d'un téléphone, avec l'interface par-dessus, et rogné selon le ratio de l'appareil par rapport au cadre de référence **1080 × 1920 (9:16)**.

Outil **100 % statique** : une seule page HTML, sans dépendance, sans serveur. Tout le traitement se fait dans votre navigateur — **aucune vidéo n'est envoyée en ligne**.

## Fonctionnalités

- Maquette de téléphone fidèle (mini-lecteur + plein écran) pour juger le rendu réel.
- Cadre de référence **1080 × 1920 · 9:16** avec visualisation du **rognage** selon le ratio choisi.
- Préréglages d'appareils (iPhone 15 / 16, Samsung Galaxy S24, Google Pixel 8, OnePlus / Xiaomi, Sony Xperia 1) ou ratio personnalisé au curseur.
- Pochette d'album optionnelle, titre, artiste et contexte personnalisables.
- Éléments d'interface affichables / masquables (dégradés de lisibilité, barres du haut et du bas, titre, progression, boutons de lecture).
- Guides : zone sûre (texte / logo) et carte de rognage sur le cadre complet pour repérer les zones perdues ou couvertes par l'UI.
- Rappel des contraintes Spotify Canvas : boucle **3–8 s**, **MP4 / WebM**, **< 50 Mo**.
- Onglet Apple Music : pochette animée (Motion Artwork) en 3:4 · 2048×2732 (mobile) et 1:1 · 3840×3840 (bureau · iPad · TV), boucle 15–35 s, ProRes / H.264.
- Export de l'image visible en PNG.
- Aucune installation : ouvrez `index.html` ou la page GitHub Pages.

## Installation

Ouvrez simplement `index.html` dans un navigateur moderne. Aucune étape de build n'est nécessaire.

### Publier sur GitHub Pages

1. Créez un dépôt GitHub et poussez ce dossier :
   ```bash
   git add .
   git commit -m "Loopframe"
   git branch -M main
   git remote add origin https://github.com/<votre-utilisateur>/<votre-depot>.git
   git push -u origin main
   ```
2. Dans le dépôt : **Settings → Pages**.
3. Sous **Build and deployment**, choisissez **Deploy from a branch**.
4. Sélectionnez la branche **`main`** et le dossier **`/ (root)`**, puis **Save**.
5. Patientez ~1 min : la page sera servie depuis `index.html` à l'URL `https://<votre-utilisateur>.github.io/<votre-depot>/`.

## Utilisation

1. Chargez une vidéo (MP4 / WebM) et, si vous le souhaitez, une pochette d'album.
2. Renseignez le titre, l'artiste et le contexte affiché en haut de l'écran.
3. Choisissez un appareil (ou un ratio personnalisé) et les éléments d'UI à afficher.
4. Basculez entre les vues **Spotify · Aperçu**, **Spotify · Zones sûres** et **Apple Music**.
5. Exportez l'image visible en PNG si besoin.

Les positions exactes des éléments d'interface peuvent varier selon la version de l'app.

## Stack technique

HTML, CSS, JavaScript vanilla — un seul fichier `index.html`, sans dépendance.

## Crédits & licence

Distribué sous licence MIT — voir [LICENSE](LICENSE) (© 2026 kur0r3x).

---

<p align="center">
  Fait par <a href="https://github.com/elisalien">Élisalien</a> ·
  <a href="https://gitlab.com/elisalien/catalog">Catalogue des shaders, sources & logiciels</a>
</p>
