# Lieux

La section **Lieux** regroupe tout ce qui concerne les espaces de jeu d'une aventure : villes, donjons, salles, zones narratives, quêtes liées, présences, combats, images, cartes et cartes interactives.

C'est l'une des sections les plus riches de l'application, parce qu'elle réunit :

- la structure narrative
- l'état d'exploration
- les contenus à montrer aux joueurs
- les présences contextuelles
- l'accès rapide aux combats

## À quoi sert la section Lieux

La dashboard des lieux sert à organiser l'aventure sur le plan spatial et narratif.

Ici tu peux :

- créer des lieux et des quêtes
- construire des hiérarchies de lieux et de sous-lieux
- lier des images et des cartes
- gérer les présences dans un lieu
- créer et rouvrir des combats liés à un lieu précis
- conserver des descriptions séparées pour le MJ et les joueurs
- utiliser une carte interactive pour te déplacer entre les lieux

## Comment y accéder

La section s'ouvre depuis la **dashboard de l'aventure**, en entrant dans la carte `Lieux et Quêtes`.

Depuis cette carte, tu peux :

- ouvrir toute la dashboard des lieux
- utiliser des raccourcis éventuels vers un lieu récent
- utiliser des raccourcis éventuels vers un combat récent lié à un lieu

## Structure de l'écran

La dashboard `Lieux` est organisée autour de deux modes principaux :

- `Normal`
- `Interactif`

et de deux zones :

- une **colonne de gauche** avec arbre, recherche, filtres et actions rapides
- un **panneau de droite** avec le détail du lieu sélectionné

## Modes Normal et Interactif

### Mode Normal

![Mode Normal des Lieux](../images/avventura/it_LuoghiNormale.png){ .img-hero }

Il s'agit du mode classique, pensé pour travailler directement sur :

- l'arbre des lieux
- le détail du lieu sélectionné
- les présences
- les combats
- les médias
- les notes

C'est le mode le plus adapté pour préparer et modifier l'aventure.

### Mode Interactif

![Mode Interactif des Lieux](../images/avventura/it_LuoghiInterattiva.png){ .img-hero }

Le mode `Interactif` devient disponible lorsqu'il existe des cartes interactives utilisables dans l'aventure.

Dans ce mode, le focus passe à la navigation par carte :

- la partie gauche de l'écran affiche la carte interactive à la place de l'arbre classique
- les marqueurs peuvent être sélectionnés
- un double clic peut ouvrir le lieu lié dans le panneau de droite
- on peut afficher ou masquer les noms des marqueurs
- on peut gérer le zoom et le déplacement de la carte

Depuis l'onglet `Médias`, tu peux toujours ouvrir rapidement la carte interactive associée à une carte du lieu, mais en mode `Interactif`, la carte devient le contenu principal de la partie gauche de la dashboard.

## La colonne de gauche

La colonne de gauche est le panneau de navigation de la section.

Tu y trouves :

- la recherche
- les filtres
- un résumé rapide
- l'arbre des lieux et des quêtes

### Menu contextuel sur les lieux dans l'arbre

En mode arborescent, tu peux faire un **clic droit sur un lieu** pour ouvrir un menu contextuel avec des actions rapides directement sur ce nœud.

Les actions disponibles sont :

- `Ajouter un sous-lieu`
- `Ajouter une présence`
- `Ajouter un lien`
- `Retirer le lien`
- `Créer une carte conceptuelle`
- `Créer un combat`
- `Modifier`
- `Supprimer le lieu`

Ce menu est l'un des moyens les plus rapides de construire la structure de l'aventure pendant que tu travailles dans l'arbre.

En pratique, il te permet de réorganiser l'arbre très vite sans ouvrir à chaque fois le formulaire complet du lieu.

### Réorganisation rapide par glisser-déposer

L'arbre des lieux prend aussi en charge une méthode rapide par glisser-déposer.

Tu peux :

- changer l'ordre des lieux frères
- déplacer un lieu sous un autre lieu
- renvoyer un lieu à la racine si tu le fais glisser hors d'une branche parente

Cela rend la mise au point de la structure narrative beaucoup plus rapide pendant la préparation.

### Filtres et résumé

La barre latérale affiche aussi un résumé compact avec :

- total des lieux
- nombre de quêtes
- nombre de lieux en visite

Selon le mode et le contexte, les filtres peuvent inclure :

- tous
- lieux
- quêtes
- en visite
- actives

## Création d'un lieu ou d'une quête

Pour créer un nouvel enregistrement, tu utilises le bouton de création dans la dashboard des lieux.

Le formulaire est divisé en trois groupes principaux :

- `Informations principales`
- `Descriptions`
- `Assets du lieu`

## Informations principales du lieu

Dans le formulaire, tu peux remplir :

- `Nom`
- lieu parent ou liens vers lieux parents
- `Type`
- `Signalement`
- état du lieu ou état de la quête

### Type : Lieu ou Quête

Le champ `Type` permet de choisir si l'enregistrement est :

- un `Lieu`
- une `Quête`

Si l'enregistrement est un **Lieu**, il utilise l'état de visite :

- non visité
- en visite
- visité

Si l'enregistrement est une **Quête**, il utilise l'état d'avancement :

- inactive
- indisponible
- active
- terminée

## Lieux parents et hiérarchie

Le formulaire des lieux prend en charge une hiérarchie avancée.

Tu peux sélectionner un ou plusieurs lieux parents, et DnDino enregistre réellement ce lien comme une structure hiérarchique.

Cela signifie qu'un lieu peut :

- se trouver à la racine de l'aventure
- exister comme sous-lieu d'un autre lieu
- être lié à plusieurs endroits de la structure quand cela a du sens

Cela est utile, par exemple, si tu veux :

- rattacher tout un groupe de lieux à une quête
- faire apparaître le même lieu dans plusieurs branches de l'arbre
- créer plusieurs parcours narratifs sans dupliquer la fiche

Dans ces cas, le lieu **n'est pas dupliqué** : l'arbre ajoute simplement un lien supplémentaire vers le même lieu.

Quand tu retires un lien :

- le lieu lui-même n'est pas supprimé
- s'il a plusieurs parents, seul le lien supplémentaire est retiré
- s'il perd son unique parent, il revient à la racine de l'arbre

Le formulaire empêche toutefois de créer des cycles, en excluant automatiquement le lieu lui-même et son sous-arbre des parents sélectionnables.

## Signalements du lieu

Chaque lieu peut avoir un ou plusieurs signalements spéciaux, également visibles dans la dashboard.

Les signalements disponibles incluent :

- dangereux
- important
- secret
- bloqué

Ils servent d'indicateurs visuels rapides pour lire plus facilement l'aventure d'un coup d'œil.

## Descriptions du lieu

La section `Descriptions` du formulaire est divisée en plusieurs champs rich text :

- `Description MJ`
- `Description joueurs`
- `Indices`
- `Trésors`
- `Notes`

Cette séparation est très utile, car elle permet de distinguer :

- ce que le MJ doit savoir
- ce que les joueurs peuvent voir ou découvrir
- les informations de support comme les indices et trésors

## Liens internes dans les textes du lieu

Dans la section `Lieux`, le système de **liens internes** est lui aussi très utile.

Ici, il sert moins à automatiser des attaques qu'à rendre le texte du lieu **navigable** et plus rapide à utiliser pendant la partie.

Dans les champs rich text du lieu, tu peux insérer des liens vers :

- `Personnage`
- `Lieu`
- `Sort`
- `Don`
- `Règle`
- et, si besoin, aussi des liens de lancer

### Pourquoi ils sont utiles dans les lieux

Les lieux contiennent souvent un texte riche en références :

- personnages présents ou mentionnés
- lieux liés
- objets ou sorts cités
- règles spéciales de scène

Transformer ces références en liens internes permet de :

- ouvrir immédiatement la fiche d'un personnage cité
- sauter directement à un autre lieu de l'aventure
- consulter un sort ou une règle sans sortir du contexte
- écrire des descriptions plus denses mais toujours faciles à parcourir

### Exemples pratiques

Tu peux lier un personnage mentionné dans un lieu, comme `capitaine Arven`, ou un autre lieu cité dans le texte, comme `Crypte engloutie`.

Ainsi, la description ne sert plus seulement à raconter : elle devient aussi un raccourci de navigation.

### Où ils sont les plus utiles

Les meilleurs endroits de la fiche de lieu pour utiliser des liens internes sont :

- `Description MJ`
- `Description joueurs`
- `Indices`
- `Notes`

### Recherche initiale du sélecteur

Quand tu appuies sur `Lien`, le sélecteur essaie d'utiliser le texte sélectionné comme filtre initial.

S'il trouve une correspondance réelle dans le nom d'un enregistrement :

- il s'ouvre déjà filtré

Sinon :

- il efface le filtre initial
- et affiche la liste complète

## Assets du lieu

Chaque lieu peut avoir ses propres assets, répartis en :

- images
- cartes

Dans le formulaire, tu peux :

- ajouter des images
- ajouter des cartes
- choisir la couverture du lieu
- retirer la couverture

Pour chaque asset, tu peux configurer :

- nom affiché
- visibilité pour les `Joueurs`
- visibilité pour le `MJ`
- texte de présentation

## Zone héro du lieu

Quand tu sélectionnes un lieu, le panneau de droite montre une zone héro avec :

- la couverture du lieu
- le nom
- le type (`Lieu` ou `Quête`)
- l'état courant
- les signalements éventuels
- la chaîne hiérarchique du lieu

Un résumé rapide y apparaît aussi avec :

- `Présences`
- `Sous-lieux`
- `Images`
- `Cartes`

## Onglets de détail

Le panneau de droite utilise une barre de focus avec cinq sections principales :

- `Panoramique`
- `Présences`
- `Combats`
- `Médias`
- `Notes`

### Panoramique

L'onglet `Panoramique` rassemble :

- description MJ
- description joueurs
- indices
- trésors
- éventuelles cartes conceptuelles liées au lieu

### Présences

L'onglet `Présences` rassemble les personnages présents dans le lieu.

Depuis là, tu peux :

- voir toutes les présences du lieu
- ajouter une nouvelle présence
- ouvrir le détail contextuel de cette présence
- changer son rôle dans le lieu
- lire ou modifier les `Notes MJ`
- retirer la présence

### Combats

L'onglet `Combats` montre tous les affrontements liés au lieu.

Depuis là, tu peux :

- créer un nouveau combat pour le lieu
- rouvrir un combat existant
- voir s'il est non commencé, en pause ou terminé
- supprimer un combat

### Médias

L'onglet `Médias` rassemble :

- images du lieu
- cartes du lieu
- cartes héritées des lieux parents si elles sont activées

Depuis là, tu peux :

- parcourir les images
- parcourir les cartes
- les montrer aux joueurs
- les montrer au MJ
- ouvrir directement une carte interactive

### Notes

L'onglet `Notes` est consacré aux notes rapides du MJ pour le lieu.

## Présences du lieu

Les présences du lieu sont gérées de manière contextuelle et séparée des personnages d'aventure et des participants au combat.

Cela permet de conserver :

- des noms affichés contextuels
- un rôle dans le lieu
- des notes MJ locales
- un état local, quand c'est nécessaire

## Deux origines possibles pour une présence

Quand tu ajoutes une présence à un lieu, le formulaire demande l'`Origine`.

Les sources possibles sont :

- `Personnage d'aventure`
- `Fiche de base`

### Personnage d'aventure

Cette origine utilise un personnage déjà lié à l'aventure.

Dans ce cas, la présence conserve l'état contextuel de campagne.

### Fiche de base

Cette origine clone un enregistrement de base de type :

- `PNJ`
- `Monstre`

Les enregistrements de type `Héros` ne sont pas sélectionnables dans ce mode.

## Règles d'unicité des présences

Dans la dashboard des lieux, DnDino applique des règles précises :

- un `Personnage d'aventure` ne peut être placé qu'une seule fois dans le même lieu
- un `PNJ` de base ne peut être ajouté qu'une seule fois dans le même lieu
- un `Monstre` de base peut être ajouté plusieurs fois dans le même lieu

Quand tu ajoutes plusieurs instances du même monstre, le nom affiché est numéroté automatiquement, par exemple :

- `Gobelin`
- `Gobelin 2`
- `Gobelin 3`

## Données de la présence dans le lieu

Dans le formulaire de présence, tu peux définir :

- `Rôle de rencontre`
- `Nom affiché`
- `Conditions`
- `Notes MJ`

Si la présence provient d'une **fiche de base** (`PNJ` ou `Monstre`), tu disposes aussi d'un état local propre au lieu :

- PV temporaires
- PV actuels
- état

Si elle provient d'un **Personnage d'aventure**, le lieu continue à se référer à l'état contextuel de campagne plutôt que de le dupliquer de la même manière localement.

## Rôle dans le lieu

Chaque présence possède un rôle contextuel :

- allié
- neutre
- ennemi

Ce rôle est important aussi bien pour lire la scène que pour certains flux ultérieurs, par exemple les combats.

## Combats liés au lieu

Les combats dans les lieux naissent directement depuis le lieu sélectionné.

Quand tu crées un nouveau combat :

- le combat est enregistré comme rencontre de ce lieu
- il apparaît immédiatement dans l'onglet `Combats`
- il peut être rouvert plus tard

## Médias du lieu

La section médias du lieu distingue clairement :

- les images
- les cartes

La dashboard peut aussi afficher les cartes des lieux parents grâce au bouton :

- `Afficher les cartes des lieux parents`

## Carte interactive

Lorsqu'une carte est définie comme carte interactive du lieu, tu peux l'ouvrir directement depuis la dashboard.

La carte interactive prend en charge :

- le zoom
- le déplacement
- les marqueurs
- la navigation entre lieux

### Marqueurs de la carte interactive

Chaque marqueur peut avoir :

- une position sur la carte
- un titre
- un lieu cible associé

Les marqueurs peuvent être :

- créés
- déplacés
- renommés
- associés à un lieu
- supprimés

Comportement de base :

- clic simple : sélection du marqueur
- double clic : ouverture du lieu lié dans le panneau de droite

## Relation entre Lieux, Cartes et Cartes interactives

Il est utile de considérer ces trois éléments comme des niveaux différents :

- le **lieu** est le conteneur narratif et structurel
- la **carte** est un asset visuel lié au lieu
- la **carte interactive** est une carte choisie comme support navigable, enrichie de marqueurs

## Quêtes dans la section Lieux

Les quêtes vivent dans la même section que les lieux, mais elles suivent un comportement dédié.

Une quête :

- apparaît dans l'arbre à côté des lieux
- utilise un état d'avancement au lieu d'un état de visite
- peut malgré tout avoir descriptions, notes, images, cartes, présences et liens contextuels

## Quand utiliser la section Lieux

La dashboard `Lieux` est le bon endroit lorsque tu veux :

- construire la géographie de la campagne
- définir sous-lieux et liens
- préparer des quêtes et leur état
- placer des présences dans le monde
- lier images et cartes
- utiliser une carte interactive pour naviguer
- ouvrir ou créer des combats liés à un lieu précis

!!! tip
    Si l'aventure devient très grande, la section `Lieux` fonctionne au mieux quand tu l'utilises comme une véritable carte mentale de la campagne : les lieux pour la structure, les quêtes pour les nœuds narratifs, les présences pour savoir qui occupe la scène et les combats pour ce qui s'y déroule.
