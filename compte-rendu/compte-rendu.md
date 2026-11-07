# Compte rendu — Gestion des ordinateurs

## Présentation

Cette application Vue.js 3 permet de gérer un petit parc informatique sans serveur ni base de données externe. Les ordinateurs sont enregistrés dans le `localStorage` du navigateur.

## Composants et organisation

- `src/views/ListeOrdinateurs.vue` affiche les ordinateurs, la recherche et le tri. Elle gère aussi la confirmation avant suppression.
- `src/views/EditOrdinateur.vue` contient le formulaire commun à l’ajout et à la modification. Le mode dépend de la route.
- `src/components/OrdinateurCard.vue` affiche les caractéristiques d’un ordinateur et émet les actions Modifier et Supprimer.
- `src/data/ordinateurs.ts` définit le modèle, les exemples initiaux et les fonctions de lecture et d’écriture du stockage local.
- `src/router/index.ts` configure les routes de la liste, de l’ajout et de la modification.

## Fonctionnalités réalisées

- Affichage des ordinateurs en cartes avec photo et caractéristiques.
- Ajout et modification avec validation des champs obligatoires et des valeurs positives.
- Suppression après confirmation.
- Recherche par modèle ou processeur et tri par mémoire ou par modèle.
- Conservation des données après rechargement grâce au `localStorage`.

## Difficultés rencontrées

- Distinguer l’ajout de la modification tout en réutilisant le même formulaire.
- Préremplir le formulaire à partir de l’identifiant présent dans la route.
- Maintenir la liste synchronisée avec le `localStorage` après les opérations.
- Valider les champs et conserver un affichage utilisable sur les petits écrans.

## Vérification

La construction et la vérification TypeScript ont été exécutées avec `npm run build`.

## Captures d’écran

Les captures de la liste et des opérations d’ajout et de modification sont disponibles dans le dossier [`captures/`](../captures/).
