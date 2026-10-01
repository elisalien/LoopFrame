# Loopframe

Aperçu de vos visuels animés avant publication : **Spotify Canvas** (fond vertical plein écran) et **Apple Music Motion Artwork** (pochette animée). Chargez votre fichier, voyez-le dans une maquette de l'écran « À l'écoute », repérez ce qui sera rogné selon le téléphone et vérifiez qu'il respecte les specs officielles.

Outil **100 % statique** : une seule page HTML, sans dépendance, sans serveur. Tout se passe dans votre navigateur — **aucun fichier n'est envoyé en ligne**.

## ▶️ En ligne

https://elisalien.github.io/LoopFrame/

## ✨ Fonctionnalités

- **Spotify · Aperçu** : maquette de l'écran « À l'écoute » (barre du haut, titre, progression, boutons) + mini-lecteur avec la pochette. Chaque élément d'interface peut être masqué.
- **Rognage par appareil** : iPhone, Galaxy, Pixel, 21:9… ou ratio libre au curseur. Pixels coupés par côté affichés en direct.
- **Spotify · Zones sûres** : cadre complet 1080 × 1920 avec zones rognées, zones couvertes par l'UI et zone sûre (822 px au centre, visible sur tous les écrans jusqu'au 21:9).
- **Apple Music** : rendu 3:4 (iPhone) et 1:1 (Mac, iPad, TV), avec la perte de hauteur si vous recadrez un Canvas 9:16.
- **Vérification du fichier** : format, dimensions, ratio, durée, et **raccord de boucle** (écart entre 1<sup>re</sup> et dernière image), comparés aux specs Spotify et Apple.
- **Canvas fixe** : les JPG sont acceptés comme sur Spotify.
- **Glisser-déposer** du fichier n'importe où sur la page, **Espace** pour lecture/pause.
- **Export PNG** de l'image visible sur l'appareil choisi, avec la zone sûre si elle est affichée.

## 📐 Specs de référence

| | Spotify Canvas | Apple Music Motion Artwork |
|---|---|---|
| Ratio / taille | 9:16, de 720 × 1280 à 1080 × 1920 (1080 × 1920 conseillé) | 3:4 en 2048 × 2732 **et** 1:1 en 3840 × 3840 |
| Durée | 3 à 8 s, en boucle | 15 à 35 s, en boucle |
| Format | MP4 (ou JPG pour un Canvas fixe) | ProRes 422 / 4444 en `.mov`, 45–100 Mb/s |
| Son | ignoré | aucun |
| Cadence | — | 23.976, 24, 25, 29.97 ou 30 i/s |

Sources : [Spotify — Canvas guidelines](https://support.spotify.com/us/artists/article/canvas-guidelines/), specs Apple Music Motion Artwork transmises par les distributeurs. Spotify n'indique pas de limite de poids officielle.

Les positions de l'interface et la zone sûre sont des approximations : elles varient selon la version de l'app et l'appareil. Le navigateur ne lit le ProRes que sur Safari/macOS ; ailleurs, prévisualisez une copie MP4.

## 🚀 Utilisation locale

Ouvrez `index.html` dans un navigateur récent. Aucune étape de build.

## 📦 Publier sur GitHub Pages

1. Dans le dépôt : **Settings → Pages**.
2. **Build and deployment** → **Deploy from a branch**.
3. Branche **`main`**, dossier **`/ (root)`**, puis **Save**.
4. Après ~1 min, la page est servie depuis `index.html`.

## 📄 Licence

MIT — voir [LICENSE](LICENSE).
