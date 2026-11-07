# Gestion des ordinateurs

Application Vue.js 3 de gestion d’un parc informatique. Elle permet de consulter les ordinateurs, les ajouter, les modifier et les supprimer avec un stockage LocalStorage.

## Dépôt GitHub

https://github.com/aymen000777/gestion_ord

## Installation

```bash
npm install
```

## Lancement

```bash
npm run dev
```

## Construction

```bash
npm run build
```

## Fonctionnalités

- Liste des ordinateurs sous forme de cartes.
- Ajout et modification via la même vue de formulaire.
- Suppression avec confirmation `confirm()`.
- Validation des champs obligatoires et des valeurs strictement positives.
- Recherche par modèle ou processeur.
- Tri par mémoire ou alphabétique.
- Persistance des données dans `localStorage`.

## Routes

- `/ordinateurs` : liste des ordinateurs
- `/ordinateurs/ajouter` : ajout
- `/ordinateurs/modifier/:id` : modification

## Captures d’écran

Les captures de la liste, de l’ajout et de la modification se trouvent dans [`captures/`](./captures/).

- [Liste des ordinateurs](./captures/01-liste-ordinateurs.png)
- [Formulaire d’ajout](./captures/02-ajout-ordinateur.png)
- [Liste après ajout](./captures/03-liste-apres-ajout.png)
- [Formulaire de modification](./captures/04-modification-ordinateur.png)
- [Liste après modification](./captures/05-liste-apres-modification.png)

## Compte rendu

Le compte rendu des composants, fonctionnalités et difficultés est disponible dans [`compte-rendu/compte-rendu.md`](./compte-rendu/compte-rendu.md).
