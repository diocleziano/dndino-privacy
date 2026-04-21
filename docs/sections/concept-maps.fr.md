# Cartes conceptuelles

La section **Cartes conceptuelles** sert à construire une représentation visuelle des relations entre lieux, personnages, autres cartes conceptuelles et notes libres.

Ce n’est ni une carte géographique ni un tableau blanc générique : c’est un outil pensé pour relier les nœuds de la campagne de façon rapide, lisible et navigable.

Tu peux l’utiliser pour :

- organiser la structure narrative de l’aventure
- relier lieux et personnages
- tracer les relations entre éléments importants
- ajouter des cadres thématiques
- annoter des idées directement sur les nœuds, cadres et liens

## Où la trouver

Les cartes conceptuelles s’ouvrent depuis deux points principaux :

- depuis la **dashboard aventure**, dans le panneau `Cartes conceptuelles`
- depuis la dashboard d’un **lieu**, quand tu veux créer ou ouvrir une carte conceptuelle liée à ce lieu

Cela signifie qu’une carte conceptuelle peut être :

- **globale à l’aventure**
- **liée à un lieu précis**

## Structure de l’écran

L’écran des cartes conceptuelles est divisé en trois colonnes principales :

- **barre latérale gauche** avec la palette et la liste des cartes
- **canvas central** où tu construis la carte
- **inspector à droite** avec les détails de l’élément sélectionné

## Sidebar : palette et sources

La barre latérale de gauche rassemble tout ce que tu peux insérer dans la carte.

Les principales catégories sont :

- `Lieux`
- `Personnages`
- `Cartes`

En plus, tu peux travailler avec :

- filtres
- recherche textuelle
- création de cadres
- création de nœuds libres

## Filtres de la palette

La palette prend en charge un filtre dédié avec ces modes :

- `Tout`
- `Lieux`
- `Personnages`
- `Cartes`

## Recherche dans la palette

La barre de recherche de la palette sert à trouver rapidement :

- un lieu
- un personnage
- une carte conceptuelle existante

## Ce que tu peux faire glisser dans le canvas

Dans le canvas, tu peux faire glisser :

- les lieux de l’aventure
- les personnages disponibles pour l’aventure
- d’autres cartes conceptuelles
- des nœuds libres

Les personnages disponibles dans la palette ne sont pas tous les personnages de la base de données sans distinction : le système utilise les personnages liés à l’aventure.

## Lieux dans la palette

Les lieux dans la palette sont affichés en tenant compte de la hiérarchie des lieux de l’aventure.

## Personnages dans la palette

Les personnages affichés dans la palette ont un sous-titre informatif qui peut inclure :

- type
- race
- classe

## Cartes dans la palette

La section `Cartes` de la palette montre les autres cartes conceptuelles de l’aventure.

Cela est particulièrement utile parce qu’une carte conceptuelle peut contenir un nœud pointant vers une autre carte conceptuelle, créant ainsi un réseau de cartes liées entre elles.

## Créer une nouvelle carte conceptuelle

Tu peux créer une nouvelle carte conceptuelle :

- depuis la dashboard aventure
- depuis la dashboard d’un lieu
- directement depuis l’écran des cartes conceptuelles, si tu en gères déjà une

Quand elle est créée, DnDino lui attribue automatiquement un nom progressif comme :

- `Carte conceptuelle`
- `Carte conceptuelle 2`
- `Carte conceptuelle 3`

## Renommer une carte

Le titre de la carte active peut être modifié directement dans l’écran.

Quand tu quittes le champ ou confirmes la modification, DnDino sauvegarde le nouveau nom.

## Supprimer une carte

En sélectionnant une carte active, tu peux la supprimer avec le bouton `Supprimer`.

## Le canvas central

Le **canvas** est la zone principale dans laquelle tu construis la carte.

Ici, tu peux :

- faire glisser des nœuds depuis la palette
- déplacer les nœuds
- créer des cadres
- relier nœuds et cadres avec des flèches
- lire d’un coup d’œil la structure générale de la campagne

## Types d’éléments dans le canvas

Dans le canvas, il existe trois grandes familles d’éléments :

- **nœuds**
- **cadres**
- **liens**

### Nœuds

Les nœuds représentent :

- un lieu
- un personnage
- une carte conceptuelle
- un nœud libre

### Cadres

Les cadres servent à regrouper visuellement plusieurs nœuds dans une même zone.

### Liens

Les liens sont des flèches qui relient nœuds et cadres.

## Nœuds normaux et nœuds libres

### Nœuds liés à de vrais enregistrements

Quand tu fais glisser dans le canvas un lieu, un personnage ou une carte conceptuelle, tu crées un nœud lié à un vrai enregistrement de l’application.

Cela signifie que le nœud :

- montre le titre réel de l’élément
- peut montrer un sous-titre contextuel
- peut ouvrir l’enregistrement lié depuis l’inspector

### Nœud libre

Le `Nœud libre` est un nœud spécial pour les idées et notes non liées à un enregistrement réel.

Il est utile pour :

- annotations narratives
- concepts abstraits
- événements
- groupes d’idées
- mémos de design

## Cadres de groupe

Le bouton `Cadre` crée un conteneur visuel à l’intérieur du canvas.

Un cadre :

- a un titre
- a une note dédiée
- peut être déplacé
- peut être redimensionné
- peut être réduit
- peut contenir automatiquement les nœuds qui tombent à l’intérieur

## Comment les nœuds se déplacent

Les nœuds peuvent être déplacés librement dans le canvas.

Leur position est sauvegardée dans la carte, de sorte que l’organisation reste persistante.

## Comment les cadres se déplacent

Les cadres peuvent eux aussi être déplacés.

Quand tu déplaces un cadre, DnDino peut déplacer avec lui les nœuds qui en font partie, ce qui garde le groupe lisible.

## Redimensionner un cadre

Les cadres peuvent être redimensionnés à partir de leurs angles.

## Réduire un cadre

Un cadre peut être réduit.

Quand il est réduit :

- il prend moins de place
- les nœuds internes sont cachés du canvas
- les liens des éléments cachés n’alourdissent pas la lecture

## Créer un lien

Les liens entre éléments se créent en faisant glisser depuis le point d’accroche d’un nœud ou d’un cadre vers un autre élément compatible.

Tu peux relier :

- nœud → nœud
- nœud → cadre
- cadre → nœud
- cadre → cadre

DnDino évite :

- les liens dupliqués à l’identique
- les liens d’un élément vers lui-même

## À quoi servent les flèches

Les flèches servent à représenter des relations, par exemple :

- un personnage qui contrôle un lieu
- un lieu qui mène à un autre
- une carte qui renvoie à une sous-carte
- un groupe thématique relié à un nœud narratif

Le sens des flèches est libre, donc il vaut mieux adopter une convention cohérente dans ta campagne.

## Inspector : détails de l’élément sélectionné

La colonne de droite change selon ce que tu sélectionnes.

Elle peut montrer les détails :

- d’un nœud
- d’un cadre
- d’un lien
- ou de la carte dans son ensemble, si rien n’est sélectionné

## Si tu sélectionnes un nœud

Quand tu sélectionnes un nœud, l’inspector montre :

- titre
- sous-titre
- éventuel bouton `Ouvrir l’enregistrement`
- description contextuelle, si disponible
- notes du nœud
- bouton pour supprimer le nœud

### Ouvrir l’enregistrement lié

Si le nœud est lié à :

- un lieu
- un personnage

tu peux ouvrir directement le formulaire correspondant.

Si, en revanche, le nœud est lié à une autre **carte conceptuelle**, le bouton ouvre cette carte et conserve aussi un petit historique de navigation entre cartes.

### Description contextuelle du nœud

Pour certains types de nœuds, l’inspector montre aussi une description réelle déjà présente dans l’application :

- pour un **lieu**, il affiche la `Description MJ`
- pour un **personnage**, il affiche la description du personnage

### Notes du nœud

Chaque nœud possède aussi ses propres notes, séparées de l’enregistrement source.

## Si tu sélectionnes un cadre

Quand tu sélectionnes un cadre, l’inspector montre :

- titre du cadre
- nombre d’éléments contenus
- notes du cadre
- bouton pour supprimer le cadre

## Si tu sélectionnes un lien

Quand tu sélectionnes une flèche, l’inspector montre :

- résumé du lien
- note de la flèche
- bouton pour supprimer le lien

Les notes sur les liens sont très utiles lorsque tu veux donner un sens plus précis à la relation, par exemple :

- alliance
- dépendance
- parenté
- passage
- cause à effet

## Si tu ne sélectionnes rien

Quand aucun élément n’est sélectionné, l’inspector montre un résumé de la carte :

- nom de la carte
- nombre de nœuds
- nombre de liens

## Zoom et navigation

L’écran prend en charge :

- zoom
- pan du canvas
- gestes de pincement
- raccourcis rapides à la souris et au trackpad

## Images dans les nœuds

Les nœuds liés à des lieux ou à des personnages peuvent aussi utiliser l’image de couverture de l’enregistrement lié comme fond visuel.

## Cartes conceptuelles liées entre elles

L’un des usages les plus puissants du système est la possibilité de relier une carte conceptuelle à une autre.

Cela permet de construire :

- une carte générale de l’aventure
- des cartes secondaires pour des zones spécifiques
- des cartes spécialisées pour des personnages, des factions ou des sous-intrigues

## Quand il est utile de les utiliser

Les cartes conceptuelles sont particulièrement utiles quand tu veux :

- planifier une campagne longue
- visualiser des relations complexes
- organiser personnages et lieux en blocs
- préparer des sous-intrigues
- conserver une vue stratégique qui ne dépend pas de longs textes

## Différence par rapport aux Lieux

La section `Lieux` organise l’aventure sur le plan spatial et en termes de contenu.

Les **cartes conceptuelles**, elles, organisent la campagne sur le plan relationnel.

En bref :

- `Lieux` = structure du monde et contenus contextuels
- `Cartes conceptuelles` = structure logique, narrative et relationnelle

## Différence par rapport aux cartes interactives

Les **cartes interactives** servent à naviguer entre des lieux réels à l’aide de marqueurs sur une carte graphique.

Les **cartes conceptuelles**, elles, servent à relier concepts, personnages, lieux et idées.

## Bonnes pratiques

Pour bien utiliser les cartes conceptuelles, il est conseillé de :

- garder une carte générale de l’aventure
- créer des cartes plus petites pour des zones ou des chapitres
- utiliser les cadres pour séparer des groupes de nœuds
- utiliser des nœuds libres pour des idées qui n’ont pas encore de vraie fiche
- annoter les nœuds et les flèches avec des notes courtes mais utiles

## En résumé

Les cartes conceptuelles de DnDino sont un outil d’organisation avancée.

Elles permettent de construire une vue visuelle et navigable de la campagne en reliant :

- lieux
- personnages
- autres cartes
- notes libres
- relations exprimées avec des flèches

!!! tip
    Si une campagne devient complexe, essaie d’utiliser une carte conceptuelle générale pour la vue d’ensemble et des cartes plus petites pour des villes, des factions ou des sous-intrigues précises. C’est l’un des moyens les plus efficaces de ne pas perdre le fil.
