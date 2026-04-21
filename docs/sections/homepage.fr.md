# Page d'accueil

La **page d'accueil** est l'écran d'ouverture de DnDino. Ce n'est pas un panneau opérationnel destiné à gérer directement chaque module de l'application, mais un **point d'accès rapide** pensé pour :

- reprendre immédiatement la dernière aventure utilisée
- revenir rapidement aux outils principaux
- s'orienter dès l'ouverture de l'application

La page d'accueil a donc deux fonctions principales :

- une **reprise rapide**, si une campagne est déjà en cours
- un **démarrage guidé**, si tu commences de zéro

## Structure de l'écran

La page d'accueil est composée de trois zones principales :

1. un en-tête de bienvenue
2. un panneau principal consacré à la dernière aventure ou au premier lancement
3. une grille avec les outils principaux de l'application

## En-tête de bienvenue

En haut de l'écran, un message d'accueil apparaît.

Si le nom du maître du jeu a été renseigné dans les paramètres, la page d'accueil affiche un message personnalisé, par exemple :

- `Bonjour, Marc !`

Sinon, l'application utilise une version générique :

- `Bonjour, MJ !`

Sous ce message, une courte phrase rappelle le rôle de cet écran : reprendre le travail là où il s'est arrêté ou ouvrir immédiatement l'un des outils principaux.

## Panneau principal

Le panneau principal change selon l'état de l'application.

### Si une aventure récente existe déjà

Quand l'application trouve une aventure utilisée récemment, la page d'accueil affiche une grande carte dédiée à la **dernière aventure**.

Cette carte contient :

- le titre de l'aventure
- une courte description, si elle existe
- un bouton `Ouvrir l'aventure`
- un bouton éventuel pour aller directement au dernier lieu visité
- quelques statistiques de synthèse
- une zone visuelle avec les héros liés à l'aventure

Si l'aventure possède une image de couverture, elle est utilisée comme fond de la carte. Sinon, un fond graphique par défaut est affiché.

#### Bouton Ouvrir l'aventure

Le bouton principal ouvre directement la **dashboard de l'aventure**, c'est-à-dire le centre opérationnel de la campagne.

C'est le moyen le plus rapide de reprendre le travail.

#### Bouton Aller au dernier lieu visité

Si l'application connaît le dernier lieu ouvert dans l'aventure, un second bouton apparaît sur la carte et permet d'y retourner directement.

C'est particulièrement utile si tu veux reprendre aussitôt l'exploration ou revenir à une zone narrative précise de la campagne.

## Statistiques de l'aventure

Le panneau principal affiche aussi quelques indicateurs de synthèse sur la dernière aventure.

Les statistiques visibles sont :

- `Quêtes`
- `Lieux`
- `Sessions`
- `Combats`

Ces valeurs servent surtout de vue d'ensemble rapide pour comprendre combien de contenu a déjà été préparé pour la campagne.

## Héros de l'aventure

Si l'aventure possède des héros liés, la partie droite de la carte leur est consacrée.

Cette zone peut montrer :

- le nombre total de héros
- leurs portraits, si disponibles
- un message invitant à ajouter une image de couverture s'ils n'en ont pas

Quand il n'y a qu'un seul héros, son portrait est affiché en plus grand. Quand il y en a plusieurs, les portraits sont regroupés dans une présentation plus compacte.

Cette section a une fonction surtout visuelle : elle permet de reconnaître la campagne d'un seul coup d'œil.

## Quand aucune aventure n'existe encore

Si l'utilisateur n'a encore aucune aventure, la page d'accueil affiche un panneau alternatif pensé pour accompagner la première utilisation.

Dans ce cas, l'écran présente :

- le titre `Prêt à commencer`
- une courte description d'introduction
- un bouton `Aller aux aventures`
- trois étapes conseillées pour commencer à utiliser DnDino

Les trois étapes affichées sont :

1. créer une aventure
2. ajouter des personnages
3. construire des lieux et des quêtes

Dans ce cas, la page d'accueil joue donc un rôle d'onboarding et accompagne la création de la première campagne.

## Outils principaux

Sous le panneau principal se trouve une grille de cartes représentant les outils les plus importants de l'application.

Les sections accessibles depuis la page d'accueil sont :

- `Aventures`
- `Héros, PNJ et Monstres`
- `Équipement`
- `Règles`
- `Générateur de noms`
- `Paramètres`

Chaque carte contient :

- un titre
- un court sous-titre descriptif
- une icône
- un fond illustré dédié

### Aventures

Ouvre la liste des campagnes et permet de :

- créer une nouvelle aventure
- ouvrir une campagne existante
- reprendre le travail de préparation

### Héros, PNJ et Monstres

Ouvre la section qui rassemble les fiches des créatures. Depuis là, il est possible de travailler sur :

- les héros
- les PNJ
- les monstres
- les données de base liées aux fiches

!!! tip
    Avec le temps, tu verras que beaucoup de personnages peuvent aussi être ouverts et modifiés directement depuis l'intérieur d'une aventure, sans casser ton flux de préparation.

### Équipement

Ouvre la section consacrée :

- aux armes
- aux armures
- aux outils
- au matériel

### Règles

Ouvre la zone de consultation rapide des règles et des références. C'est utile pour :

- consulter du matériel de support
- rechercher des règles
- ouvrir des contenus liés au jeu

### Générateur de noms

Ouvre l'outil qui permet de générer rapidement des noms utiles pendant la préparation ou l'improvisation, par exemple pour :

- les PNJ
- les monstres
- les rencontres imprévues

!!! tip
    Pendant une séance, le mini générateur de noms de la topbar est souvent encore plus pratique, car il permet de produire un nom sans quitter l'écran sur lequel tu travailles.

### Paramètres

Ouvre le panneau des préférences globales de l'application et de la gestion locale de la base de données.

## Quand utiliser la page d'accueil

La page d'accueil est particulièrement utile lorsque tu veux :

- reprendre rapidement la dernière campagne
- ouvrir la dashboard de l'aventure la plus récente
- revenir au dernier lieu visité
- accéder rapidement aux outils principaux de l'application
- démarrer une nouvelle campagne si la base de données est encore vide

!!! tip
    Si tu travailles presque toujours sur la même campagne, la carte de la dernière aventure est le moyen le plus rapide de revenir directement au bon endroit sans repasser à chaque fois par la liste complète des aventures.
