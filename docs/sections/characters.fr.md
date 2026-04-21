# Héros, PNJ et Monstres

La section **Héros, PNJ et Monstres** regroupe toutes les fiches de base des personnages de l'application. C'est l'endroit où l'on crée, modifie et clone les enregistrements qui pourront ensuite être liés aux aventures, aux lieux et aux combats.

Cette page est importante car, dans DnDino, il existe **plusieurs niveaux de personnage**, chacun avec un rôle différent :

- la **fiche de base**
- le **personnage d'aventure**
- la **présence dans un lieu**
- le **participant au combat**

Ce ne sont pas des doublons inutiles : ils servent à conserver **des données contextuelles séparées**, comme le nom affiché, les points de vie, les conditions, l'initiative et les notes MJ, sans perdre le lien avec la fiche d'origine.

## Fiche de base

La **fiche de base** est l'enregistrement principal stocké dans la section `Héros, PNJ et Monstres`.

Tu y définis tout ce qui appartient au personnage de manière générale :

- nom
- type : `Héros`, `PNJ` ou `Monstre`
- espèce, classe, taille, alignement
- caractéristiques
- CA, PV maximum, vitesse, initiative
- description, capacités, attaques
- images liées
- sorts liés
- équipement et autres données de référence

La fiche de base ne représente pas automatiquement un personnage “présent” dans une aventure, dans un lieu ou dans un combat. C'est le modèle dont partent les niveaux suivants.

## Créer, modifier et cloner un personnage

Pour créer une nouvelle fiche :

1. ouvre la section `Héros, PNJ et Monstres`
2. appuie sur le bouton d'ajout
3. remplis le formulaire du personnage
4. enregistre la fiche

Dans le formulaire, tu peux créer :

- des héros
- des PNJ
- des monstres

Le type choisi influence certains champs et certains comportements. Par exemple :

- pour les **héros**, la présence dans l'aventure, l'inspiration et l'état contextuel sont particulièrement importants
- pour les **monstres**, le FP, les attaques et l'usage multiple dans les contextes opérationnels prennent plus d'importance

Quand tu ouvres une fiche existante, tu peux la modifier dans tous ses détails. Les changements effectués ici mettent à jour la source, mais n'écrasent pas toujours automatiquement tous les enregistrements contextuels déjà créés dans l'aventure, les lieux ou le combat. C'est volontaire.

Le **clonage** crée une nouvelle fiche de base à partir d'une fiche existante, en copiant aussi des éléments liés comme :

- les champs de la fiche
- les sorts liés
- les attaques structurées
- les images liées

Il est particulièrement utile pour :

- créer des variantes proches d'un même monstre
- partir d'un PNJ déjà préparé
- construire rapidement plusieurs fiches avec une structure similaire

## Liens internes dans les textes du personnage

L'une des fonctions les plus utiles de la fiche de base, surtout pour les **PNJ** et les **Monstres**, est le système de **liens internes** dans les champs rich text.

Cette fonction est particulièrement précieuse dans la section **Attaques**, car elle permet de transformer un texte descriptif en outil opérationnel prêt à être utilisé pendant la partie et en combat.

En pratique, tu peux insérer des liens qui ouvrent directement :

- un jet de dés
- un jet pour toucher
- une attaque complète avec dégâts
- un personnage
- un lieu
- un sort
- un don
- une règle du glossaire

## Où les utiliser

Les liens internes sont particulièrement utiles dans les champs rich text de la fiche, par exemple :

- `Attaques`
- `Capacités spéciales`
- `Description`
- d'autres champs descriptifs où tu veux des références rapides

Le cas le plus utile reste cependant **Attaques**, car il te permet de rendre immédiatement cliquables :

- le jet pour toucher
- les dés de dégâts
- une attaque complète déjà prête

Pour les monstres, c'est très pratique, car cela réduit le temps passé à relire les formules ou à reconstruire les jets à la main.

## Comment insérer un lien

Le bon flux est le suivant :

1. ouvre un champ rich text de la fiche
2. sélectionne le texte que tu veux transformer en lien, ou place simplement le curseur
3. appuie sur le bouton `Lien`
4. choisis le type de lien dans le sélecteur
5. confirme la création

Selon le texte sélectionné, le sélecteur peut déjà te proposer certains liens automatiques prêts à l'emploi.

## Les quatre liens les plus utiles pour les jets

### Jet libre

`Jet libre` est le lien le plus flexible. Il est toujours disponible dans le sélecteur et sert quand tu veux créer un lancer configurable sans structure rigide.

Il est utile pour :

- une formule complète comme `1d6+3`
- un simple dé comme `1d20`
- une formule que tu veux encore ajuster juste avant le lancer

### Lancer les dés

`Lancer les dés` apparaît seulement si le texte sélectionné est une **formule de dés valide**.

Exemples valides :

- `1d6`
- `2d8+4`
- `4d4 + 1`

Ce lien est idéal pour des dégâts simples, des dés de soin, des effets aléatoires et des jets séparés rapides.

### Jet pour toucher

`Jet pour toucher` apparaît seulement si le texte sélectionné est un **modificateur valide**, et non une formule complète `1d20`.

Exemples valides :

- `+5`
- `-1`
- `0`
- `2`

Quand tu crées ce lien, DnDino sait qu'il doit lancer un **1d20** avec ce modificateur. C'est parfait quand tu veux écrire dans les attaques quelque chose de lisible comme :

- `Morsure +6`
- `Griffes +4`

### Jet pour toucher et dégâts

`Jet pour toucher et dégâts` est le lien le plus puissant pour la section **Attaques**.

Il est toujours disponible dans le sélecteur et ouvre un configurateur dédié où tu peux définir :

- le modificateur du jet pour toucher
- un éventuel seuil de critique
- jusqu'à trois formules de dégâts
- le titre de chaque composante de dégâts

C'est la meilleure manière de construire une attaque complète de monstre ou de PNJ, car un seul lien peut contenir :

- le jet pour toucher
- les dégâts principaux
- les dégâts secondaires
- les dégâts additionnels

En combat, ce lien est particulièrement utile, car le popover associé peut aussi servir à appliquer les dégâts aux cibles choisies.

## Exemple pratique pour les Attaques

Une façon très efficace d'écrire une attaque de monstre est de garder un texte lisible pour le MJ et de ne rendre cliquables que les points utiles.

Par exemple :

- `Morsure +6, allonge 1,5 m, une cible. Touché : 1d8+4 perforants.`

Tu peux ensuite transformer :

- `+6` en `Jet pour toucher`
- `1d8+4` en `Lancer les dés`

ou créer directement un seul lien `Jet pour toucher et dégâts` sur le nom de l'attaque ou sur une partie de la ligne.

## Lier lieux, personnages et autres références

Le système de liens ne sert pas uniquement pour les jets.

Dans les champs descriptifs, tu peux aussi créer des liens vers d'autres contenus de l'application, comme :

- un `Lieu`
- un autre `Personnage`
- un `Sort`
- un `Don`
- une `Règle`

Quand tu appuies sur `Lien`, le sélecteur peut aussi utiliser le texte sélectionné comme filtre initial :

- s'il trouve une vraie correspondance dans le nom des enregistrements, le sélecteur s'ouvre déjà filtré
- s'il ne trouve aucun résultat réel, le filtre initial est effacé et tu vois la liste complète

## Personnages d'aventure

Le **personnage d'aventure** est le niveau qui relie une fiche de base à une campagne précise.

Cet enregistrement sert à gérer les valeurs qui n'ont de sens **qu'à l'intérieur d'une aventure**, par exemple :

- points de vie actuels
- points de vie temporaires
- conditions
- état
- inspiration héroïque

En d'autres termes :

- la fiche de base dit **qui est** le personnage
- le personnage d'aventure dit **dans quel état il se trouve** dans cette campagne

## Présences dans les lieux

La **présence dans un lieu** est encore un autre type d'enregistrement. Elle sert à dire qu'un personnage ou une créature est présent dans un lieu précis, avec un nom et éventuellement un état local.

Dans le formulaire `Ajouter une présence au lieu`, il existe deux origines possibles :

- `Personnage d'aventure`
- `PNJ / Monstre`

### Présence issue d'un personnage d'aventure

Si tu choisis `Personnage d'aventure`, l'enregistrement du lieu est relié à un personnage déjà présent dans la campagne.

Dans ce cas :

- la présence reste liée au personnage d'aventure
- elle ne crée pas de copie autonome du personnage
- on ne peut pas ajouter deux fois le même personnage d'aventure dans le même lieu

### Présence issue d'un PNJ / Monstre

Si tu choisis `PNJ / Monstre`, le lieu crée une **présence locale clonée** à partir d'une fiche de base de type `PNJ` ou `Monstre`.

Ce nouvel enregistrement possède ses propres données locales, comme :

- nom affiché
- PV actuels
- PV temporaires
- conditions
- état
- disposition
- notes MJ

Le comportement dépend alors du type :

- les **Monstres** peuvent avoir plusieurs présences locales dans un même lieu
- les **PNJ** restent uniques dans un même lieu et ne sont pas reproposés plusieurs fois dans le sélecteur

Quand tu ajoutes plusieurs instances d'un même monstre, DnDino propose automatiquement un nom incrémental, par exemple :

- `Gobelin 2`

## Pourquoi le nom affiché existe

Les présences de lieu comme les participants au combat possèdent un champ `Nom affiché`.

Ce champ sert à conserver un nom **contextuel** sans renommer la fiche de base. C'est utile, par exemple, pour :

- distinguer des copies similaires d'une même créature
- donner à un PNJ un nom précis dans un seul lieu
- utiliser un nom différent en combat sans changer l'enregistrement source

## Participants au combat

Le **participant au combat** est le niveau opérationnel utilisé pendant l'affrontement.

Un participant peut provenir de trois sources différentes :

- un **personnage d'aventure**
- une **présence de lieu**
- une **fiche de base**

Chaque participant possède son propre enregistrement spécifique au combat, avec des données comme :

- nom affiché
- initiative
- CA
- PV maximum
- PV actuels
- PV temporaires
- conditions
- état
- jets de sauvegarde contre la mort
- ordre dans le round

### Participants issus d'un personnage d'aventure

Si le participant vient d'un personnage d'aventure :

- il reste lié à ce personnage de campagne
- à la fin du combat, les valeurs finales sont resynchronisées vers l'enregistrement d'aventure

### Participants issus d'une présence de lieu

Si le participant vient d'une présence de lieu :

- il reste lié à cette présence
- si cette présence utilise un état local, le combat peut resynchroniser les PV, conditions et état sur l'enregistrement du lieu

### Participants issus d'une fiche de base

Si le participant vient directement d'une fiche de base :

- l'enregistrement de combat utilise cette fiche comme source
- le comportement vis-à-vis des multiples instances dépend du type

Dans le sélecteur de combat :

- un enregistrement de type **Monstre** peut être ajouté plusieurs fois
- un enregistrement de type **PNJ** ou **Héros** n'est pas reproposé plusieurs fois dans le même combat

## Synchronisation entre les niveaux

Certaines valeurs sont synchronisées entre les niveaux, mais tout n'est pas toujours écrasé.

### De la fiche de base vers les contextes

La fiche de base fournit :

- l'identité du personnage
- les statistiques de référence
- les sorts
- les attaques
- les images

### Des contextes vers les enregistrements liés

Les niveaux opérationnels peuvent, eux, synchroniser les données de situation, notamment :

- les PV
- les conditions
- l'état
- certaines notes locales

En combat, par exemple, les valeurs finales peuvent revenir :

- sur le personnage d'aventure lié
- sur la présence de lieu liée, si cette présence utilise un état local

## Différence pratique entre les niveaux

Pour retenir plus facilement la logique :

- `Fiche de base` : le **modèle général** du personnage
- `Personnage d'aventure` : l'**état du personnage dans la campagne**
- `Présence dans un lieu` : la **présence contextuelle du personnage dans un lieu précis**
- `Participant au combat` : la **version opérationnelle du personnage dans l'affrontement**

## Quand utiliser chaque niveau

### Utilise la fiche de base quand :

- tu dois créer le personnage
- tu veux modifier les données structurelles
- tu dois lier images, sorts ou attaques

### Utilise le personnage d'aventure quand :

- tu veux lier un héros à la campagne
- tu veux suivre de façon persistante les PV, l'état, les conditions et l'inspiration dans l'aventure

### Utilise la présence dans le lieu quand :

- tu veux peupler un lieu avec personnages ou créatures
- tu veux donner des noms contextuels à des PNJ et des monstres
- tu veux créer des instances locales séparées dans un lieu

### Utilise le participant au combat quand :

- tu prépares ou gères un affrontement
- tu as besoin d'initiative, de PV et de conditions de bataille
- tu veux que le combat travaille sur des enregistrements contextuels sans salir directement la fiche de base

## En résumé

La section `Héros, PNJ et Monstres` n'est pas seulement une archive de fiches. C'est le **niveau source** à partir duquel toute la gestion contextuelle des personnages dans l'application prend vie.

La logique générale est la suivante :

- la **fiche de base** définit le personnage
- le **personnage d'aventure** l'insère dans la campagne
- la **présence dans un lieu** le contextualise dans un lieu
- le **participant au combat** le rend opérationnel dans l'affrontement

!!! tip
    Pour éviter la confusion, garde toujours cette distinction en tête : la fiche de base décrit le personnage, tandis que l'aventure, le lieu et le combat décrivent son état dans un contexte précis. Il n'est pas nécessaire de trop s'attacher à la séparation théorique : retiens surtout que certains champs n'existent que dans leur propre contexte.
