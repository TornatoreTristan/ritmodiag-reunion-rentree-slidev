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
- `public/assets/drive/logos/` : logos et visuels de marque.
- `public/assets/drive/photos/` : photos d’équipe / agence téléchargées depuis Drive.
- `public/assets/drive/formation/` : photos d’action / immersion téléchargées depuis Drive.

## Assets Drive récupérés

Google Drive était authentifié. Une sélection d’assets a été téléchargée sans modification de Drive :

- Logos : `logo-ritmodiag.svg`, `ritmodiag.svg`, `ritmodiag-plan-travail.png`, `ritmodiag-photo.jpg`.
- Photos formation / immersion : `formation-01.jpg`, `formation-02.jpg`, `formation-03.jpg`.
- Photos agence / équipe : `agence-caen-01.jpg`, `agence-caen-02.jpg`, `equipe-01.jpg`, `equipe-02.jpg`, `equipe-03.jpg`.

Les requêtes Drive demandées ont été tentées. Les dossiers exacts `Marketing > Projets > Réunion de rentrée` et `Marketing > Franchise : Agents co' > Immersion : Formation` n’étaient pas retrouvés tels quels via la recherche accessible ; des photos pertinentes ont donc été récupérées depuis les dossiers Marketing/Photos et une série récente de photos image dans Drive.

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
