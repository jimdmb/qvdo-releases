# Video Data Optimizer pour QNAP

*[English below](#english)*

Réduisez la place prise par vos vidéos sur votre NAS QNAP : l'application réencode vos films et séries en H.265 (HEVC), H.264, AV1 ou VP9, garde l'original en sécurité et range vos fichiers.

**[⬇ Télécharger la dernière version](../../releases/latest)**

## Fonctions

- Réduction de taille au choix : pourcentage de l'original, taille fixe, qualité constante…
- Sécurité des fichiers : l'original est gardé (corbeille réseau ou dossier caché) jusqu'à ce que vous décidiez ; le résultat est vérifié avant de remplacer quoi que ce soit.
- **Workers** : faites encoder par un PC plus rapide (Docker), le NAS reste maître de vos fichiers.
- Organisation et renommage (films, séries, vidéos personnelles), plage horaire, pause, sauvegarde de la configuration.
- Interface web en français et en anglais, avec tutoriels.

## Quel fichier choisir ?

| Votre NAS | Fichier |
|---|---|
| Intel / AMD 64 bits (TS-x53, TS-x63, TS-x73…) | `VideoDataOptimizer_<version>_x86_64.qpkg` |
| ARM 64 bits | `…_arm_64.qpkg` |
| ARM 32 bits (Alpine) | `…_arm-x41.qpkg` |
| ARM 32 bits (Annapurna) | `…_arm-x31.qpkg` |
| Intel 32 bits | `…_x86.qpkg` |

Le paquet **sans « -lite »** contient les codecs (ffmpeg) : c'est celui à prendre. La version « -lite » est pour ceux qui fournissent leur propre ffmpeg.

## Installation

1. *App Center → ⚙ Réglages* : autorisez l'installation d'applications sans signature numérique (seule QNAP peut signer un paquet ; l'avertissement est normal).
2. *App Center → Installation manuelle* : choisissez le fichier `.qpkg` téléchargé.
3. Ouvrez l'application depuis le menu de QTS, ou `https://IP-DU-NAS:8765`, et créez votre mot de passe.

**Mise à jour** : installez la nouvelle version par-dessus ; vos réglages sont conservés. L'application vous prévient quand une nouvelle version sort.

## Essai et licence

L'application s'installe gratuitement avec un **essai complet** (14 jours à partir du premier encodage, 10 vidéos ou 50 Go). Un numéro de série débloque ensuite l'édition Standard ou Pro, sans réinstaller.

## Logiciels tiers

Le paquet avec codecs contient [FFmpeg](https://ffmpeg.org), sous licence GPL v3 : son code source est publié avec chaque version (`ffmpeg-…-source.tar.xz`). Video Data Optimizer lui-même est un logiciel propriétaire.

---

## English

Shrink the space your videos take on your QNAP NAS: the app re-encodes your movies and shows to H.265 (HEVC), H.264, AV1 or VP9, keeps the original safe and organizes your files.

**[⬇ Download the latest version](../../releases/latest)**

- **Pick the file** for your NAS from the table above (x86_64 for most Intel/AMD models). Take the package **without "-lite"**: it includes the codecs.
- **Install**: App Center → ⚙ Settings → allow apps without a digital signature; then App Center → Manual install → pick the `.qpkg`. Open the app from QTS or `https://NAS-IP:8765`.
- **Update**: install the new version over the old one; settings are kept. The app tells you when a new version is out.
- **Trial and license**: free install with a full trial (14 days from the first encode, 10 videos or 50 GB); a serial number then unlocks the Standard or Pro edition without reinstalling.
- **Workers**: let a faster PC (Docker) do the encoding while the NAS keeps control of your files.
- **Third-party software**: the package with codecs includes [FFmpeg](https://ffmpeg.org) under the GPL v3; its source is published with every release. Video Data Optimizer itself is proprietary software.
