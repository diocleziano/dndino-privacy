# Cartes interactives

Les **cartes interactives** servent à naviguer visuellement entre les lieux de l’aventure sur une véritable carte graphique, à l’aide de marqueurs cliquables reliés aux fiches de lieu.

Elles sont pensées pour les cas où la simple structure en arbre ne suffit plus et où tu veux te déplacer dans l’espace de la campagne de façon plus naturelle, par exemple sur :

- une ville
- un château
- un quartier
- un donjon
- une région

## À quoi elles servent

Les cartes interactives sont utiles quand tu veux :

- utiliser une carte comme surface principale de navigation
- ouvrir les lieux en cliquant sur des marqueurs visuels
- donner une structure spatiale plus claire à la campagne
- passer d’une carte de détail à une carte plus large

Elles ne remplacent ni les **Lieux** ni les **Cartes conceptuelles** :

- les **Lieux** restent les vraies fiches de la campagne
- les **Cartes conceptuelles** servent à montrer des relations logiques et narratives
- les **Cartes interactives** servent au contraire à naviguer dans des lieux réels à partir d’une image de carte

## D’où elles viennent

Les cartes interactives ne sont pas un type d’enregistrement séparé créé dans un module à part. Elles naissent à partir des **images de type carte** liées aux lieux.

En pratique :

1. tu relies une ou plusieurs images de type `Carte` à un lieu
2. tu choisis laquelle doit être utilisée comme carte interactive par défaut
3. tu ajoutes sur cette carte des marqueurs reliés à des lieux

## Où elles sont utilisées

Les cartes interactives vivent dans la section **Lieux et Quêtes**.

Elles peuvent être utilisées de deux manières :

- comme **mode interactif intégré** dans la dashboard des lieux
- comme **grand panneau carte** ouvert depuis `Médias`

## Différence entre le mode intégré et le grand panneau

### Mode interactif intégré

Quand l’aventure dispose de cartes, dans la dashboard des lieux tu peux passer de la vue normale à la vue `Interactive`.

Dans ce mode :

- la partie gauche de l’écran montre la carte à la place de l’arbre classique
- le panneau de droite continue à afficher le détail du lieu sélectionné
- en cliquant sur les marqueurs, tu navigues directement entre les lieux

### Grand panneau carte

Depuis le panneau `Médias` d’un lieu, tu peux aussi ouvrir une carte interactive dans un panneau dédié plus grand.

Ce mode est particulièrement utile quand tu veux :

- modifier les marqueurs
- corriger les liens
- travailler avec plus de précision sur la carte

## Comment préparer une carte interactive

Le bon flux est le suivant :

1. ouvre le lieu qui doit posséder la carte
2. va dans la section `Médias`
3. ajoute une ou plusieurs images de type `Carte`
4. choisis laquelle doit devenir la carte interactive par défaut
5. ouvre la carte interactive
6. crée les marqueurs et relie-les aux lieux

## Comment la carte par défaut est choisie

Un lieu peut avoir plusieurs cartes liées. Parmi elles, l’une peut être marquée comme carte interactive de référence.

Quand DnDino doit déterminer quelle carte afficher pour un lieu, il suit cette logique :

- si le lieu a une carte explicitement choisie comme carte interactive, il utilise celle-là
- sinon il utilise la première carte disponible du lieu
- si le lieu n’a pas de carte propre, il peut utiliser la carte d’un lieu parent

## Relation entre lieu et carte

Chaque carte interactive appartient à un lieu.

Le lieu propriétaire de la carte n’est pas forcément le seul lieu ouvrable depuis cette carte : les marqueurs peuvent en effet relier n’importe quel lieu de la structure de l’aventure.

## Comment entrer dans le mode interactif

Dans la dashboard `Lieux`, quand des cartes sont disponibles, tu peux passer à la vue `Interactive`.

Dans ce mode, tu trouves :

- en-tête de la carte interactive
- sélecteur `Carte`
- éventuel bouton `Retour`
- éventuel bouton `Niveau supérieur`
- toggle `Afficher les noms des marqueurs`
- contrôles de zoom
- canvas de la carte

## Sélecteur de carte

Le menu `Carte` permet de choisir quelle carte afficher parmi celles disponibles dans l’aventure.

## Navigation entre cartes

Le mode interactif prend en charge deux types de navigation entre cartes.

### Retour

Le bouton `Retour` ramène à la carte affichée précédemment.

### Niveau supérieur

Si le lieu courant a un lieu parent qui possède une carte interactive, le bouton `Niveau supérieur` peut apparaître.

Il te permet de remonter vers une carte plus large.

## Le canvas de la carte

Le canvas est la surface centrale où la carte elle-même est affichée.

Tu peux y :

- voir la carte
- voir les marqueurs
- cliquer ou double-cliquer sur les marqueurs
- utiliser zoom et pan

## Zoom et déplacement

Les cartes interactives prennent en charge :

- zoom avant et arrière
- réinitialisation du zoom
- défilement horizontal et vertical
- pan en faisant glisser la carte
- geste de pincement
- zoom à la molette lorsque le curseur est au-dessus de la carte

## Afficher les noms des marqueurs

Avec le toggle `Afficher les noms des marqueurs`, tu peux décider si les étiquettes des marqueurs doivent être visibles directement sur la carte.

Quand il est actif :

- chaque marqueur peut montrer son propre nom ou, si le titre est vide, le nom du lieu lié

Quand il est désactivé :

- seules les icônes des marqueurs restent visibles

## Comment fonctionnent les marqueurs

Un marqueur contient :

- une position normalisée sur la carte
- un titre optionnel
- un lien optionnel vers un lieu

Le marqueur est enregistré relativement aux coordonnées de la carte, et reste donc au bon endroit même si le zoom change.

Les marqueurs changent aussi de couleur selon l'état du lieu lié, ce qui permet de lire plus facilement la progression de l'exploration d'un seul coup d'oeil :

- une couleur pour les lieux `Non visités`
- une couleur pour les lieux `En visite`
- une couleur pour les lieux `Visités`

Ces couleurs sont fixes et ne changent pas selon le thème actif, afin que leur signification reste cohérente dans toute l'application.

## Comportement des marqueurs en lecture

Quand tu n’es pas en mode modification :

- un **clic simple** sélectionne un marqueur
- un **double clic** ouvre le lieu lié

Dans le mode interactif intégré, ouvrir un lieu signifie mettre immédiatement à jour le panneau de droite.

Dans le grand panneau carte, ouvrir un lieu ferme le panneau carte et redonne le focus au lieu sélectionné dans la dashboard.

## Comment créer un marqueur

Pour créer un marqueur dans le grand panneau carte :

1. ouvre la carte interactive depuis `Médias`
2. appuie sur `Modifier`
3. appuie sur `Nouveau marqueur`
4. choisis le lieu à associer
5. clique sur un point de la carte

## Mode Modification

Dans le grand panneau, il existe un véritable état d’édition.

Quand tu appuies sur `Modifier` :

- la carte entre en mode édition
- tu peux créer de nouveaux marqueurs
- tu peux sélectionner des marqueurs existants pour les modifier
- tu peux faire glisser les marqueurs pour les repositionner

Quand tu appuies sur `Verrouiller`, tu sors du mode édition.

## Nouveau marqueur

Quand tu actives `Nouveau marqueur` :

- DnDino te demande d’abord de choisir le lieu à associer
- puis t’invite à cliquer sur la carte pour le positionner

## Choix du lieu lié

Quand tu crées ou modifies un marqueur, l’inspector à droite affiche le sélecteur de lieux.

Depuis là, tu peux :

- rechercher par nom
- voir les lieux organisés dans une structure hiérarchique
- assigner le marqueur au bon lieu

## Modifier un marqueur existant

Quand un marqueur est sélectionné en mode édition, tu peux modifier dans l’inspector :

- `Titre du marqueur`
- `Lieu lié`

Si le titre est laissé vide, DnDino utilise comme fallback le nom du lieu lié ou un titre générique.

## Déplacer un marqueur

En mode modification, tu peux faire glisser un marqueur vers un nouveau point de la carte.

À la fin du déplacement, DnDino enregistre :

- nouvelle position X
- nouvelle position Y

## Supprimer un marqueur

Toujours depuis l’inspector, quand un marqueur est sélectionné, tu peux utiliser :

- `Supprimer le marqueur`

## L’inspector de la carte

Le panneau latéral de la grande carte change selon l’état courant.

### En lecture

Si tu n’es pas en train de modifier, l’inspector montre simplement la liste des marqueurs existants.

### Pendant la création d’un marqueur

Si tu as activé `Nouveau marqueur`, l’inspector montre :

- instructions
- champ de recherche
- liste des lieux sélectionnables

### Pendant la modification d’un marqueur

Si tu as sélectionné un marqueur existant, l’inspector montre :

- champ titre
- sélecteur du lieu lié
- résumé du lieu actuel
- bouton pour supprimer le marqueur

## Liste des marqueurs

La liste des marqueurs dans l’inspector peut aussi être utilisée pour naviguer.

Chaque ligne montre :

- titre du marqueur
- lieu lié, s’il existe

En lecture, en cliquant sur une ligne, tu peux ouvrir le lieu lié.

## Comportement de la carte en mode intégré

Quand tu utilises le mode `Interactive` directement dans la dashboard des lieux :

- la carte suit le lieu sélectionné
- DnDino essaie de montrer la carte la plus adaptée à ce lieu
- si le lieu n’a pas de carte propre, il peut utiliser une carte d’un niveau supérieur

## Héritage de la carte depuis le lieu parent

Une partie très utile du système est qu’un lieu peut aussi utiliser une carte d’un niveau supérieur.

Cela permet des cas comme :

- un quartier qui utilise la carte de la ville
- une salle qui utilise la carte du château
- un point d’intérêt qui utilise la carte de la région

## Comment ouvrir une carte interactive depuis Médias

Dans le panneau `Médias` d’un lieu, les cartes de type `Carte` peuvent montrer l’action :

- `Ouvrir la carte interactive`

## Quand utiliser le mode intégré

Le mode interactif intégré est idéal quand tu veux :

- naviguer rapidement entre les lieux
- travailler avec la carte et le panneau lieu côte à côte
- utiliser la carte comme alternative à l’arbre classique

## Quand utiliser le grand panneau

Le grand panneau est plus adapté quand tu veux :

- créer des marqueurs
- déplacer des marqueurs
- changer les liens
- travailler avec plus de précision

## En pratique

Les cartes interactives sont l’outil qu’il faut quand tu veux donner une vraie dimension spatiale aux lieux.

L’idée de base est simple :

- le **lieu** reste la fiche principale
- la **carte** devient la surface visuelle
- le **marqueur** est le lien opérationnel entre l’image et le contenu
