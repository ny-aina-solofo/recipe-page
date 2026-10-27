# Plan de réalisation — Recipe Page

## 1) Contexte et objectif

Le projet consiste à reproduire une page de recette selon le design fourni dans le dossier `design` pour les variantes mobile et desktop, en respectant la charte visuelle du `style-guide.md` et en utilisant les assets déjà présents dans `assets/`.

Le but est de livrer une page responsive qui s’affiche correctement sur desktop et mobile, sans casser la structure sémantique ni la lisibilité.

> Aucune modification de code n’a été faite dans ce plan. La mise en œuvre viendra seulement après validation.

---

## 2) Fichiers à explorer et à modifier

### Fichiers de référence

- `index.html` : fichier principal de contenu et structure HTML.
- `style-guide.md` : palette de couleurs, typographie, dimensions de mise en page.
- `design/desktop-design.jpg` : référence de mise en page desktop.
- `design/mobile-design.jpg` : référence de mise en page mobile.
- `assets/images/image-omelette.jpeg` : image principale de la recette.
- `assets/fonts/` : polices Young Serif et Outfit à utiliser si l’on choisit un chargement local.

### Fichiers potentiellement à créer ou compléter

- `styles.css` (optionnel) : si l’on décide de séparer le CSS du HTML pour une meilleure lisibilité.
- `index.html` : dans le cadre de ce challenge, il est également viable de garder le CSS dans une balise `<style>` à la racine, ce qui évite une étape supplémentaire.

---

## 3) Étapes dans l’ordre

### Étape 1 — Comprendre le design et la structure

- Lire le `style-guide.md` pour récupérer :
  - couleurs,
  - familles de polices,
  - tailles de texte,
  - largeur cible du layout mobile/desktop.
- Analyser les références `design/desktop-design.jpg` et `design/mobile-design.jpg`.
- Identifier les blocs majeurs :
  - image du plat,
  - titre principal,
  - intro,
  - section préparation,
  - ingrédients,
  - instructions,
  - nutrition.

### Étape 2 — Structurer le HTML de manière sémantique

- Remplacer le contenu brut actuel par une vraie structure HTML :
  - `header` ou `main`,
  - `article` pour le contenu principal,
  - `section` pour les blocs thématiques,
  - `h1` pour le titre principal,
  - `h2` pour les sous-titres,
  - `ul` / `ol` et `li` pour les listes,
  - `table` pour la nutrition.
- Ajouter l’image avec son attribut `alt` de manière descriptive.
- Vérifier la hiérarchie des titres afin d’avoir un document bien organisé.

### Étape 3 — Poser les styles de base

- Définir le fond de page beige, la largeur du conteneur central et les marges.
- Choisir les familles de police Young Serif / Outfit.
- Définir les variables CSS pour les couleurs et les espacements.
- Mettre les styles de base du texte :
  - `font-size`,
  - `line-height`,
  - `color`,
  - `font-weight`.

### Étape 4 — Styliser le bloc principal et l’image

- Créer une carte principale blanche avec bord arrondi et ombre légère.
- Placer l’image en haut avec coins arrondis.
- Ajuster la taille de l’image selon le design.
- S’assurer que le conteneur reste lisible en mobile et en desktop.

### Étape 5 — Reproduire les sections de contenu

- Titre principal avec police serif élégante.
- Description courte en italique ou style léger.
- Bloc “Preparation time” avec fond rose clair, bullet points et textes en gras.
- Section ingrédients avec liste à puces et mise en page claire.
- Section instructions avec liste ordonnée, numérotée et texte bien aligné.
- Section nutrition avec tableau stylisé et valeurs alignées à droite.

### Étape 6 — Responsive design mobile / desktop

- Commencer par la version mobile avec une largeur de contenu optimisée.
- Ajouter ensuite un breakpoint pour desktop.
- Ajuster :
  - largeur du conteneur,
  - taille du titre,
  - marges internes,
  - espacement entre sections,
  - alignement du tableau nutrition.
- Vérifier que le design reste propre sur les écrans larges et petits.

### Étape 7 — Validation visuelle et accessibilité

- Vérifier les contrastes de couleurs.
- Vérifier le rendu sur mobile et desktop.
- Contrôler la densité informative et la lisibilité.
- Vérifier l’accessibilité : `alt`, hiérarchie des titres, contraste rouge sur fond, navigation claire.

### Étape 8 — Finitions

- Supprimer les éléments temporaires de starter code.
- Nettoyer le HTML et le CSS.
- Vérifier qu’il n’y a pas de contenu texte inutile ou non structuré.
- Vérifier l’alignement final avec la maquette.

---

## 4) Risques à anticiper

### Risques visuels

- Le design peut sembler “correct” mais ne pas correspondre précisément aux marges, tailles ou espacements du mockup.
- Les polices peuvent ne pas être exactement ressemblantes si le chargement local est incomplet.
- L’image principale doit être ajustée pour éviter un rendu déformé.

### Risques structurels

- Un HTML non sémantique peut rendre la page moins lisible et moins accessible.
- Oublier les listes (`ul` / `ol`) peut brouiller le rendu attendu de la recette.
- Une mauvaise hiérarchie des titres nuit à l’accessibilité.

### Risques responsive

- Le layout peut être beau sur desktop mais cassé sur mobile.
- Les marges et la largeur du conteneur peuvent devenir trop grandes sur les petits écrans.
- Les tableaux et listes peuvent dépasser si le CSS n’est pas adapté.

### Risques accessibilité

- Couleurs trop faibles pour le contraste.
- Texte trop dense ou trop petit pour la lecture.
- Image sans `alt` ou alt non descriptif.

---

## 5) Approche recommandée pour ce projet

Pour ce challenge, l’approche la plus sûre est :

1. construire d’abord une structure HTML propre,
2. ajouter les styles de base,
3. ajuster le layout mobile,
4. étendre la version desktop avec un breakpoint,
5. corriger les écarts visuels jusqu’à l’alignement le plus proche possible du design.

Cette méthode évite d’écrire trop de CSS sans fondation solide et permet de garder le projet lisible et maintenable.

---

## 6) Validation attendue

La page sera considérée comme terminée si :

- la structure HTML est correcte et sémantique,
- la mise en page suit le design desktop et mobile,
- les couleurs et polices sont cohérentes avec le `style-guide.md`,
- les sections sont clairement lisibles,
- la version mobile est bien fonctionnelle,
- l’accessibilité de base est respectée.

---

## 7) Prochaine étape

Une fois ce plan validé, je passe à la mise en œuvre dans `index.html` et, si nécessaire, dans un fichier CSS dédié, en respectant strictement le rendu attendu.
