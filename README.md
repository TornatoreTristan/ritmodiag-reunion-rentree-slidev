# Présentation Slidev — Réunion de rentrée franchisés RITMODiag 2026

Projet Slidev pour une présentation **premium light**, dynamique et professionnelle, destinée aux franchisés RITMODiag déjà ancrés et aux nouveaux entrants.

## Version en ligne

- Présentation : https://tornatoretristan.github.io/ritmodiag-reunion-rentree-slidev/
- Dépôt GitHub : https://github.com/TornatoreTristan/ritmodiag-reunion-rentree-slidev

## Lancer la présentation

```bash
cd /home/tristan/ritmodiag-reunion-rentree-slidev
npm install
npm run dev
```

Slidev affichera une URL locale, généralement `http://localhost:3030`.

## Exporter / builder

```bash
npm run build      # génère le site statique dans dist/
npm run export     # export PDF si le navigateur headless requis est disponible
```

## Structure du projet

- `slides.md` : présentation complète avec formats variés et notes speaker utiles.
- `style.css` : direction artistique alignée sur la charte RITMODiag, couleur primaire `#56a681`.
- `package.json` : scripts `dev`, `build`, `export`.
- `public/favicon.svg` : favicon vert RITMODiag `#56a681`.
- `public/assets/drive/logos/` : logos et visuels de marque historiques.
- `public/assets/reunion-rentree/` : **seules photos autorisées désormais référencées dans `slides.md`**, téléchargées depuis `Marketing > Projets > Réunion de rentrée`.

## Assets photos autorisés — Réunion de rentrée

Google Drive était authentifié. Le dossier exact `Marketing > Projets > Réunion de rentrée` a été retrouvé et les visuels utilisés dans `slides.md` proviennent exclusivement de ce dossier ou de ses sous-dossiers. La provenance est tracée dans :

- `public/assets/reunion-rentree/MANIFEST.md`
- `public/assets/reunion-rentree/MANIFEST.json`

Les anciennes photos à provenance incertaine (`public/assets/drive/photos/*`, `public/assets/drive/formation/*`, `ritmodiag-photo.jpg`, `ritmodiag-plan-travail.png`) ne sont plus référencées dans `slides.md`. Les fichiers historiques peuvent rester dans l’arborescence pour compatibilité, mais ne doivent pas être réutilisés sans preuve de présence dans `Réunion de rentrée`. Les nouveaux noms contiennent `v20260908` pour éviter que le cache masque le changement.

## Notes de contenu

Le PDF source fourni (`Présentation type RITMODiag`) a été inspecté localement : extraction texte, métadonnées et rendu de premières pages. La présentation reprend l’esprit clair de la trame : slides aérées, titres courts, blocs structurés, priorité au vert de marque `#56a681` et alternance entre chiffres, cartographie, photos, grille, manifeste et checklist.

Les notes speaker ont été nettoyées pour supprimer les remarques méta/concepteur non destinées à la prise de parole.

## Modifier le style

Les variables principales sont en haut de `style.css` :

```css
:root {
  --rd-primary: #56a681;
  --rd-primary-dark: #2f7658;
  --rd-primary-soft: #eaf6f1;
}
```
