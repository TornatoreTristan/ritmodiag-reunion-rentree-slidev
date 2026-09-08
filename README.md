# Présentation Slidev — Réunion de rentrée franchisés RITMODiag 2026

Projet créé pour une présentation **premium light**, énergique et professionnelle, destinée aux franchisés RITMODiag déjà ancrés et aux nouveaux entrants.

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

## Exporter

```bash
npm run build      # génère le site statique dans dist/
npm run export     # export PDF si le navigateur headless requis est disponible
```

## Structure du projet

- `slides.md` : présentation complète, environ 44 slides modulaires, avec notes speaker en commentaires Markdown.
- `style.css` : direction artistique premium light, fonts Funnel Display / Satoshi, composants visuels.
- `package.json` : scripts `dev`, `build`, `export`.
- `public/assets/drive/logos/` : assets téléchargés depuis Drive quand disponibles.
- `public/assets/drive/formation/` : dossier prévu pour photos d’action / Immersion Formation.
- `public/assets/placeholders/` : dossier prévu pour éventuels placeholders ou exports additionnels.

## Assets Drive récupérés

Google Drive était authentifié. Une sélection raisonnable d’assets logo/visuels a été téléchargée sans modification de Drive :

- `public/assets/drive/logos/logo-ritmodiag.svg`
- `public/assets/drive/logos/ritmodiag.svg`
- `public/assets/drive/logos/ritmodiag-plan-travail.png`
- `public/assets/drive/logos/ritmodiag-photo.jpg`

Je n’ai pas trouvé de photos action clairement identifiées dans les dossiers demandés `Marketing > Projets > Réunion de rentrée` et `Marketing > Franchise : Agents co' > Immersion : Formation` via les requêtes Drive accessibles. La présentation contient donc une section **Immersion Formation** avec emplacement propre.

## Où déposer les assets manquants

Déposer les photos d’action / formation ici :

```text
public/assets/drive/formation/
```

Puis remplacer le placeholder dans `slides.md`, par exemple :

```html
<div class="photo-frame h-80"><img src="/assets/drive/formation/nom-photo.jpg" /></div>
```

Assets utiles pour prochaine itération :

1. Logo officiel final RITMODiag en SVG/PNG haute définition.
2. Palette officielle si différente du bleu/cyan/teal utilisé.
3. Photos d’équipe / formation / immersion terrain.
4. Photos agences physiques : Caen, Saint-Lô, Cherbourg.
5. Captures propres des outils réseau, CRM/tableau de suivi, fiche Google Business Profile.
6. Icônes ou pictogrammes métier validés.
7. Toute photo ambiance pour l’apéro pétanque / convivialité.

## Notes de contenu

Le PDF source a été relu via extraction texte locale. La qualité d’extraction est bonne et exploitable. Les formulations internes ou trop brouillonnes de la trame ont été gardées en notes speaker ou reformulées dans un style plus premium.

Les slides sont volontairement courtes : elles servent à accompagner un speaker pendant environ 2h, pas à remplacer sa parole.

## Modifier le style

Les variables de couleur sont en haut de `style.css` :

```css
:root {
  --rd-bg: #f7f9fb;
  --rd-ink: #111827;
  --rd-blue: #00a7df;
  --rd-teal: #0fb7a4;
  --rd-green: #8cc63f;
}
```

Pour une version encore plus brandée, remplacer ces couleurs par celles extraites de la charte officielle.
