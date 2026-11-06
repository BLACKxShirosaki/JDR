# Fa’Diel — habillage CSS

Déposer `sheet.css`, `.nojekyll` et `assets/` à la racine du dépôt.
Le dossier `assets/` doit rester au même niveau que `sheet.css`.

Cette archive contient uniquement l’habillage. Le HTML et le JavaScript de
la fiche restent ceux de l’application existante.

## Derniers correctifs inclus

- Avatar à gauche ; Identité et Caractéristiques sur la largeur restante.
- Identité sur deux colonnes et Métier sur une ligne entière.
- Bouquets de feuilles et fleurs ivoire dans les deux coins inférieurs de
  l’Identité, sans cadre ni cristaux, sur fond transparent.
- Titre, bordure extérieure continue et corrections des raccords des coins.
- Adaptation aux petits écrans.

Les images sont séparées du CSS : aucune chaîne d’image Base64 à éditer.

## Publication GitHub Pages

1. Créer un dépôt public, par exemple `fadiel-css`, en cochant Add README.
2. Décompresser cette archive puis utiliser Add file > Upload files.
3. Déposer le CONTENU de l’archive, en conservant le dossier assets.
4. Dans Settings > Pages : Deploy from a branch, main, /(root), Save.
5. Attendre la publication puis ouvrir l’URL publiée de `sheet.css`.
   Cette URL doit afficher du code CSS, pas la page GitHub du fichier.
6. Dans le fichier `style.css` du Pen, remplacer l’ancien contenu par :
   `@import url("URL_HTTPS_PUBLIQUE_DU_FICHIER_SHEET_CSS");`
   L’URL entre guillemets doit être remplacée par l’adresse réelle publiée.
7. Placer les prochains ajustements CSS après cet import.

Ne pas effacer l’ancien style.css de CodePen avant d’avoir vérifié que la
nouvelle URL de sheet.css est accessible. Aucun changement HTML ou JS requis.

Le domaine GitHub Pages est distinct de github.com : ne pas utiliser le lien
/blob/ du dépôt comme adresse CSS.

## Réglages

Palette : variables --fd-* au début de sheet.css.
Titre visuel : --fd-titre-fiche.
Bouquets Identité : chercher BOUQUETS FLEURIS ; opacity:.28.
Asset : assets/identite/bouquet-fleuri.webp.
Les parties du bouquet cachées sous le cadre ont été reconstituées.
