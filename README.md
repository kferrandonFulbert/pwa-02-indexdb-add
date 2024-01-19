# pwa-02-Indexdb Ajout de biere personnelle

## Attendu

https://kferrandonfulbert.github.io/pwa-02-indexdb-add/

## Rappel 

Il s'agit d'une application web simple pour gérer une liste de bières en utilisant HTML, Bootstrap et IndexedDB. L'application permet aux utilisateurs d'ajouter de nouvelles bières à une base de données IndexedDB locale.

## Prérequis

Assurez-vous d'avoir les dépendances suivantes installées :

- Bootstrap 5.3.2
- Popper.js Core 2.11.8
- Un navigateur prenant en charge les Service Workers et IndexedDB

## Installation

Clonez le dépôt sur votre machine locale :

```bash
git clone https://github.com/votre-nom/utilisateur-application-web-gestion-bieres.git
```

Ouvrez le projet dans votre éditeur de texte ou IDE préféré.
Exécutez l'application à l'aide d'un serveur local. Vous pouvez utiliser des outils tels que Live Server si vous utilisez Visual Studio Code.

## fonctionnalité attendue

- Ouvrez le fichier index.html dans votre navigateur.
- Accédez à la page "Ajouter une bière" en cliquant sur le lien "Ajouter une bière" dans la barre de navigation.
- Remplissez le formulaire avec les détails de la bière : Nom, Slogan et Description.
- Cliquez sur le bouton "Soumettre" pour ajouter la bière à la base de données IndexedDB locale.

## Service Worker

L'application inclut un Service Worker pour les fonctionnalités hors ligne. Il est enregistré dans le fichier HTML (index.html), permettant la mise en cache des ressources pour une meilleure expérience utilisateur en cas de déconnexion.

## IndexedDB

La fonctionnalité IndexedDB est mise en œuvre dans la section script du fichier HTML (index.html). Elle inclut la création d'une base de données IndexedDB nommée "BeerDB" avec deux object stores : "beers". Lorsqu'une nouvelle bière est soumise via le formulaire, elle est ajoutée à l'object store "beers".

