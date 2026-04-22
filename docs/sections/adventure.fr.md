# Aventure

![Dashboard Aventure](../images/avventura/it_dashboardavventura.png){ .img-hero }

La section **Aventure** est le centre d'organisation d'une campagne dans DnDino. C'est ici que prend forme la structure principale de ton travail : le titre de la campagne, son identité visuelle, les personnages liés, les sessions, les lieux, les images partagées, les cartes et les accès rapides aux combats.

!!! tip
    Considère la dashboard de l'aventure comme le **quartier général de la campagne** : ce n'est pas l'endroit où tu fais tout dans le détail, mais celui depuis lequel tu rejoins rapidement toutes les zones vraiment opérationnelles.

Cette page explique le parcours principal :

- création d'une nouvelle aventure
- modification et gestion d'une aventure existante
- fonctionnement de la dashboard de l'aventure
- lien entre la dashboard et les sous-pages dédiées

Les zones plus spécifiques, comme **Lieux**, **Cartes conceptuelles**, **Session live**, **Personnages**, **Images** et **Cartes**, seront approfondies dans leurs pages dédiées.

## À quoi sert une aventure

Dans DnDino, une aventure est le conteneur principal d'une campagne ou d'un arc narratif. Elle sert à réunir, dans un même contexte :

- les personnages liés à la campagne
- les lieux et les quêtes
- les sessions textuelles et live
- les images partagées
- les cartes associées aux lieux
- les cartes conceptuelles globales
- les combats qui naissent dans les lieux liés à l'aventure

L'aventure n'est donc pas une simple fiche d'identité, mais le point d'entrée vers toute la partie opérationnelle de la campagne.

## Où créer une aventure

La création commence dans la **liste des aventures**.

Depuis cet écran, tu peux :

- créer une nouvelle aventure avec le bouton `Nouvelle`
- créer la première aventure avec le grand bouton central `Créer une aventure` si la base est encore vide
- ouvrir une aventure existante en cliquant sur sa ligne
- modifier une aventure existante
- cloner une aventure déjà présente
- supprimer une aventure

La liste peut aussi être triée par :

- nom
- date de création
- dernière modification

!!! note
    Quand tu tries par **dernière modification**, DnDino ne regarde pas seulement la fiche d'aventure : il prend aussi en compte l'activité liée, comme les lieux, les sessions, les personnages d'aventure, les cartes conceptuelles et les combats.

## Création d'une nouvelle aventure

Lorsque tu ouvres le formulaire de création, DnDino te propose une fiche avec les informations principales de la campagne.

Les champs principaux sont :

- `Titre`
- `Auteur`
- `Cadre`
- `Description courte`
- `État`

Le champ **État** utilise un contrôle segmenté et permet d'indiquer si l'aventure est :

- non commencée
- en cours
- terminée

## Description étendue

Sous les informations principales, tu trouves aussi une section **Description** plus large.

Cette zone sert à noter une présentation plus complète de la campagne, par exemple :

- le ton de l'aventure
- le contexte narratif
- les objectifs initiaux
- les notes générales pour le maître du jeu

La description longue n'est pas perdue dans la dashboard : si elle existe, elle peut être rouverte rapidement plus tard.

## Couverture et images de l'aventure

Dans le formulaire, tu peux attribuer une **image de couverture** à l'aventure. La couverture est utilisée comme image représentative de la campagne dans les écrans principaux.

Tu peux aussi ajouter des images dans la section **Images de l'aventure**. Ces images :

- restent liées à l'aventure
- n'appartiennent à aucun lieu spécifique
- peuvent être montrées rapidement aux joueurs ou au maître du jeu depuis la dashboard

Pour chaque image, tu peux gérer :

- le nom affiché
- la visibilité pour les `Joueurs`
- la visibilité pour le `Maître`

## Modification d'une aventure existante

Lorsque tu ouvres une aventure existante en modification, le formulaire est le même que pour la création, mais avec une section supplémentaire : **Réinitialisation de l'aventure**.

La réinitialisation ne supprime pas la structure de la campagne, mais remet à zéro l'état de jeu courant. En particulier, elle :

- retire tous les personnages d'aventure liés
- supprime toutes les sessions enregistrées
- remet lieux et quêtes à leur état initial
- remet PNJ et monstres à plein PV et sans conditions
- réinitialise les combats préparés sans en supprimer la structure

Cette fonction est utile si tu veux réutiliser l'ossature d'une campagne ou remettre l'aventure dans un état propre sans la reconstruire depuis zéro.

## Clonage et suppression

Depuis la liste des aventures, tu peux aussi :

### Cloner une aventure

Le clonage crée une copie de la campagne via le service interne de duplication. C'est utile si tu veux :

- partir d'une structure proche
- réutiliser une base existante
- créer une variante d'une campagne déjà présente

### Supprimer une aventure

Quand tu supprimes une aventure, DnDino retire l'enregistrement principal et lance aussi le nettoyage des ressources liées. Il met également à jour les références des personnages globaux pour retirer le lien avec l'aventure supprimée.

## Ouverture de la dashboard de l'aventure

En cliquant sur une aventure dans la liste, tu entres dans sa **dashboard**, qui est le véritable centre opérationnel de la campagne.

La dashboard est organisée comme un écran à panneaux :

- une bande supérieure avec l'en-tête et le contrôle de la session live
- deux colonnes inférieures avec des cartes dédiées aux différentes zones de la campagne

L'ordre des panneaux peut être personnalisé depuis les paramètres de l'application.

## En-tête de la dashboard

La partie haute de la dashboard regroupe les informations essentielles de l'aventure :

- couverture
- titre
- état
- description courte
- cadre
- auteur

Si l'aventure possède aussi une description longue, un bouton dédié permet de l'ouvrir dans un popover et de la lire sans quitter la dashboard.

Depuis cette zone, tu peux aussi entrer dans **Modifier** pour revenir au formulaire de l'aventure et mettre à jour ses données.

## Session live

À côté de l'en-tête se trouve le panneau **Session live**.

Cette section sert à :

- lancer une nouvelle session live pour l'aventure
- voir si une session est en cours ou en pause
- suivre le temps écoulé
- mettre la session en pause
- la fermer et l'enregistrer

Quand la session live de l'aventure est active, le **lecteur global** et les **lieux** suivent ce contexte.

S'il existe déjà une session live ouverte dans une autre aventure, la dashboard le signale clairement et ne te laisse pas en démarrer une deuxième en parallèle.

## Les panneaux de la dashboard

Sous l'en-tête, la dashboard affiche les panneaux principaux de l'aventure.

Ceux prévus actuellement sont :

- `Lieux et Quêtes`
- `Personnages`
- `Sessions`
- `Images`
- `Cartes`
- `Cartes conceptuelles`
- `Métadonnées`

!!! tip
    Depuis les paramètres, il est possible de modifier l'ordre des panneaux dans la Dashboard Aventure, aussi bien pour leur colonne que pour leur position.

### Lieux et Quêtes

Ce panneau est le point d'entrée vers la dashboard des lieux.

Tu peux y voir rapidement :

- le nombre total de lieux
- le nombre de quêtes
- le nombre de quêtes terminées

Des accès rapides peuvent aussi apparaître vers :

- le dernier lieu utile
- le dernier combat utile

En ouvrant cette carte, tu entres dans la section qui gère :

- les lieux
- les sous-lieux
- les présences
- les images de lieu
- les cartes
- les cartes interactives
- les combats liés aux lieux

Cette partie sera décrite plus en détail dans la page dédiée aux **Lieux**.

### Personnages

Le panneau **Personnages** montre les personnages liés à la campagne.

Ici tu peux :

- voir les personnages d'aventure déjà liés
- en ajouter de nouveaux
- les soigner rapidement avec `Soigner tout`
- ouvrir leur état contextuel de campagne

Cette section ne remplace pas la fiche de base du personnage : elle montre la couche spécifique à l'aventure, avec état, PV et conditions contextuels.

La différence entre :

- fiche de base
- personnage d'aventure
- personnage de lieu
- participant au combat

sera approfondie dans la page dédiée aux **Personnages**.

### Sessions

Le panneau **Sessions** rassemble :

- les sessions textuelles
- les sessions live
- les notes
- les résumés
- la timeline

Depuis là, tu peux aussi créer une nouvelle session textuelle. Les sessions constituent donc la mémoire narrative et opérationnelle de la campagne.

Cette zone sera approfondie dans la page dédiée à la **Session live** et à la gestion des sessions.

### Images

Le panneau **Images** rassemble les images globales de l'aventure, c'est-à-dire celles qui ne sont pas liées à un lieu spécifique.

Depuis là, tu peux :

- ajouter des images
- les parcourir par pages
- les montrer rapidement aux joueurs
- les montrer rapidement au maître

C'est la bonne zone pour tout le matériel visuel de campagne qui n'appartient pas à un lieu précis.

### Cartes

Le panneau **Cartes** montre toutes les cartes liées aux lieux de l'aventure.

Les cartes ne s'ajoutent pas directement ici : elles apparaissent dans la dashboard une fois déjà liées à un lieu.

Depuis cette carte, tu peux :

- parcourir les cartes de l'aventure
- les montrer aux joueurs ou au maître
- ouvrir directement la carte interactive du lieu correspondant, si elle existe

Cette partie sera détaillée dans les pages dédiées aux **Cartes** et aux **Cartes interactives**.

### Cartes conceptuelles

Le panneau **Cartes conceptuelles** rassemble les cartes globales de l'aventure.

Depuis là, tu peux :

- voir combien de cartes conceptuelles existent
- les ouvrir rapidement
- en créer une nouvelle

Les cartes conceptuelles sont utiles pour relier idées, lieux, personnages et relations narratives. Elles seront détaillées dans leur page dédiée.

### Métadonnées

Si l'affichage des métadonnées est activé dans les paramètres, un panneau technique apparaît aussi avec :

- l'ID de l'aventure
- la date de création
- la date de dernière modification

Cette section est surtout utile pour le contrôle, la diagnostique ou une gestion avancée.

## Relation avec les sous-pages

La page **Aventure** est une vue d'ensemble générale. À partir d'ici, les pages filles approfondissent chaque outil opérationnel spécifique.

Les sous-pages de ce guide seront :

- **Lieux et Quêtes**
- **Cartes conceptuelles**
- **Images**
- **Cartes**
- **Cartes interactives**
- **Session live**
- **Personnages**

En pratique :

- cette page explique **comment une aventure naît et comment elle est structurée**, ainsi que l'organisation de la Dashboard Aventure
- les pages filles expliquent **comment chaque section interne s'utilise réellement**

## Quand utiliser cette section

La section Aventure est le bon point d'entrée quand tu veux :

- créer une nouvelle campagne
- définir la couverture, l'état et la description de l'aventure
- reprendre le travail sur une campagne existante
- entrer dans la dashboard principale
- lancer une session live
- atteindre rapidement les lieux, personnages, sessions, images et cartes de la campagne
