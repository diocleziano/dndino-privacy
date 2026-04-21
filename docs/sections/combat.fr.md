# Combat

Le mode **Combat** de DnDino est pensé pour être le tracker opérationnel principal d’un affrontement. Cette page décrit le mode de combat standard utilisé dans DnDino.

Le combat naît toujours dans le contexte d’un **lieu** et emporte avec lui les personnages, les présences locales et les éventuels monstres ou PNJ liés à cette scène.

Cette page explique tout le flux :

- préparation du pré-combat
- gestion des participants
- lancement de l’affrontement
- utilisation du tour en cours
- application des dégâts, soins, conditions et jets de sauvegarde
- intégration avec la **Fenêtre Joueurs**
- clôture de l’affrontement et résumé final

## Utilisation avec un ou deux écrans

Le combat de DnDino fonctionne très bien aussi sur **un seul écran** : toute la partie opérationnelle reste dans le panneau principal, et tu peux gérer normalement les participants, les tours, les dégâts, les conditions et le résumé final sans second moniteur.

Cela dit, si tu disposes d’une configuration à deux écrans, tu peux utiliser :

- un écran principal pour le panneau de contrôle du MJ
- un deuxième écran ou moniteur pour la **Fenêtre Joueurs**

Dans cette configuration, le flux devient encore plus confortable :

- sur l’écran du MJ restent visibles la liste des participants, les contrôles de round, le tour en cours, les textes d’attaque, les notes MJ et les modifications rapides
- sur l’écran des joueurs apparaît une présentation propre du participant actif, avec image et overlay contextuel

En pratique :

- sur un seul écran, tu utilises tout le combat depuis l’écran principal
- avec deux écrans, tu sépares le panneau technique du MJ de la présentation destinée aux joueurs

!!! tip
    Le second écran n’est pas obligatoire. C’est simplement un excellent confort lorsque tu veux montrer aux joueurs des images et les informations du tour en cours sans exposer le panneau technique du MJ.

## Fonctionnement de la Fenêtre Joueurs pendant le combat

Quand le combat démarre, DnDino peut ouvrir ou mettre à jour automatiquement la **Fenêtre Joueurs**.

Si la présentation joueurs est active :

- au début du combat, une courte **intro** peut apparaître avec les participants
- pendant le combat, la fenêtre se met à jour sur le **participant du tour en cours**
- à la fin de l’affrontement, un **résumé final** peut apparaître

Pendant le combat, la Fenêtre Joueurs n’affiche pas le panneau technique du MJ, mais une présentation visuelle avec :

- l’image du participant actif
- le nom affiché aux joueurs
- les informations d’overlay, si elles sont activées

L’overlay peut inclure :

- round en cours
- PV actuels, maximum et temporaires
- conditions
- prochain tour

Les informations sur les ennemis peuvent être gérées séparément de celles des héros.

## Réglages de la Fenêtre Joueurs et du second écran

Les options les plus importantes se trouvent dans **Réglages**, dans la section dédiée à la présentation du combat et à la fenêtre joueurs.

### Ouverture et comportement général

Les principaux réglages sont :

- `Ouvrir la fenêtre joueurs même avec un seul moniteur`
- `Afficher les contrôles de la fenêtre joueurs dans la topbar`
- `Afficher l’intro du combat aux joueurs`
- `Afficher le résumé final aux joueurs`

#### Ouvrir la fenêtre joueurs même avec un seul moniteur

Si cette option est active, DnDino peut ouvrir automatiquement la Fenêtre Joueurs même lorsque tu travailles avec un seul écran.

Si elle est désactivée :

- sur un seul écran, la fenêtre ne s’ouvre pas automatiquement
- si elle est déjà ouverte, elle continue malgré tout à se mettre à jour

#### Afficher les contrôles de la fenêtre joueurs dans la topbar

Si tu actives cette option, la barre supérieure de l’application affiche des boutons pour :

- ouvrir manuellement la fenêtre joueurs
- la fermer manuellement

#### Afficher l’intro du combat aux joueurs

Quand tu appuies sur `Démarrer l’affrontement`, la Fenêtre Joueurs peut afficher une courte introduction avec :

- titre de l’affrontement
- participants impliqués
- nombre de participants

Si tu désactives cette option, le combat passe directement à la présentation du premier participant actif.

#### Afficher le résumé final aux joueurs

Quand le combat se termine, la Fenêtre Joueurs peut afficher un résumé final.

Le résumé destiné aux joueurs ne montre que les données utiles pour eux, comme :

- dégâts infligés par les héros
- dégâts subis par les héros
- image du pire ennemi

Le résumé final des joueurs reste visible tant que tu ne changes pas le contenu de la fenêtre ou que tu ne la fermes pas.

### Informations affichées pendant le tour

Les réglages qui contrôlent l’overlay du participant actif sont :

- `Afficher le round dans la fenêtre joueurs`
- `Afficher les PV dans la fenêtre joueurs`
- `Afficher les conditions dans la fenêtre joueurs`
- `Afficher le prochain tour dans la fenêtre joueurs`

### Informations sur ennemis, monstres et PNJ

Pour les participants non héros, il existe des contrôles dédiés :

- `Afficher les détails des PNJ et monstres aux joueurs`
- `Afficher les conditions des ennemis aux joueurs`
- `Afficher les noms des ennemis aux joueurs`

Cela permet de décider si la Fenêtre Joueurs doit :

- montrer la créature de façon plus évocatrice
- ou afficher aussi des données plus techniques

## Où s’ouvre le combat

Le combat est créé depuis le contexte du **lieu**. Une fois ouvert, DnDino affiche un écran divisé en deux colonnes principales :

- à gauche, le tracker opérationnel du combat
- au centre, le panneau principal de la scène ou du tour en cours

Avant le début du combat, le panneau central affiche le **Résumé pré-combat**.

Quand l’affrontement est actif, ce même panneau devient la zone du **Tour en cours**.

Quand le combat est terminé, le panneau central affiche le **Résumé final de l’affrontement** pour le MJ.

## Structure générale de l’écran

### Colonne de gauche

La colonne de gauche contient :

- `Contrôle du combat`
- l’en-tête de la liste des participants
- la liste ordonnée des participants

La liste est encadrée par deux lignes décoratives et fonctionnelles :

- `Début du round`
- `Fin du round`

### Panneau central

Le panneau central change selon l’état du combat :

- **avant le démarrage**, il affiche le résumé pré-combat
- **pendant l’affrontement**, il affiche le participant du tour en cours
- **à la fin du combat**, il affiche le résumé final du MJ

## Pré-combat

Le pré-combat sert à préparer l’affrontement avant de lancer le premier tour.

C’est le moment où il est surtout utile d’ajuster trois choses :

- le nom des monstres, quand tu veux mieux les distinguer à la table
- les initiatives des héros, en les saisissant manuellement
- les initiatives des PNJ et monstres, en les lançant automatiquement ou en les écrivant à la main

## Résumé pré-combat

La carte initiale montre une vue rapide avec des indicateurs comme :

- participants
- héros
- alliés
- ennemis
- PV totaux des ennemis
- éventuels participants déjà dans un état critique

## Initiative des personnages

La section `Initiative des personnages` rassemble les héros principaux et permet de modifier rapidement l’initiative avant de trier l’affrontement.

Chaque ligne contient :

- nom du participant
- sous-titre contextuel
- champ initiative
- bouton `Supprimer`

## PNJ et monstres

La section `PNJ et monstres` est dédiée aux participants non héros.

Ici, tu peux :

- modifier rapidement l’initiative
- renommer à la volée monstres et PNJ pour mieux les distinguer
- utiliser `Init PNJ/Monstres` pour lancer automatiquement leur initiative
- saisir manuellement la valeur d’initiative si tu préfères utiliser un lancer fait hors de l’application
- retirer rapidement un participant avec `Supprimer`

## Actions principales du pré-combat

Dans le résumé pré-combat, les actions principales sont :

- `Ajouter`
- `Trier`
- `Démarrer l’affrontement`

Si au moins un participant a encore une initiative à `0`, DnDino demande une confirmation avant de démarrer.

## D’où peuvent venir les participants

Le panneau d’ajout de participants peut aller chercher des participants depuis trois origines :

- `Héros`
- `Présences du lieu`
- `Globaux`

### Héros

Ici, tu trouves les personnages d’aventure déjà liés à la campagne. Chaque héros ne peut entrer dans le combat qu’une seule fois.

### Présences du lieu

Ici, tu trouves les personnages déjà présents dans le lieu d’où naît le combat. Leur état local peut être réutilisé comme base pour l’affrontement.

### Globaux

Ici, tu trouves des fiches de base qui ne sont pas déjà liées comme héros de l’aventure.

Dans le cas des globaux :

- les `Monstres` peuvent être ajoutés plusieurs fois
- les `Héros` et `PNJ` globaux ne peuvent pas être dupliqués comme simples fiches globales

## Contrôle du combat

Une fois l’affrontement commencé, le panneau `Contrôle du combat` reste fixe au-dessus de la liste et contient les actions principales du round.

Les lignes de boutons sont :

1. `Ajouter` et `Trier`
2. `Démarrer/Pause` ou `Reprendre` et `Fin`
3. `Préc.` et `Suiv.`

S’il existe une dernière attaque annulable, un panneau supplémentaire apparaît aussi :

- `Annuler la dernière attaque`

## Liste des participants

La liste de gauche est le cœur du suivi tactique.

Chaque ligne repliée affiche :

- position dans l’ordre des tours, par exemple `1/8`
- nom du participant
- jusqu’à trois icônes de conditions
- badge `Tour` s’il s’agit du participant actif
- CA
- PV
- PV temporaires
- initiative

Le participant actif est mis en évidence bien plus fortement que les autres :

- bande colorée latérale
- bordure plus marquée
- fond plus chaud
- défilement automatique pour le garder visible

La ligne utilise aussi des effets d’impact quand le participant :

- subit des dégâts
- est tué
- est restauré par un undo

## Menu contextuel sur une ligne

Avec un **clic droit** sur la carte du participant, tu peux ouvrir le menu contextuel.

Pour le moment, l’action disponible est :

- `Supprimer`

## Déploiement d’une ligne participant

En cliquant sur une ligne, le participant se déploie et affiche ses contrôles rapides.

Dans la partie développée, tu trouves :

- nom modifiable
- champs numériques rapides :
  - initiative
  - PV
  - PV temporaires
  - CA
- boutons d’action
- bloc conditions
- accès aux capacités, capacités spéciales et sorts, si présents

## Boutons rapides de la ligne

Les actions rapides peuvent inclure :

- `Attaquer`
- `Dégâts`
- `Soins`
- `JS`
- `Notes MJ`
- `Modifier`
- `Conditions`

Certains boutons n’apparaissent que lorsqu’ils ont du sens pour ce participant.

## Attaquer

`Attaquer` ouvre un popover pour sélectionner :

- une ou plusieurs cibles
- les dégâts à appliquer

Le sélecteur de cibles utilise une liste compacte avec :

- nom
- CA
- PV
- conditions

L’ordre des cibles n’est pas aléatoire. DnDino essaie de proposer d’abord les participants les plus pertinents selon celui qui attaque.

En général :

- si un **Héros** attaque, les **ennemis** viennent d’abord, puis les alliés, puis les neutres, puis les monstres moins prioritaires
- si un participant non héros attaque, les **héros** viennent d’abord, puis les alliés, puis les neutres, puis les ennemis moins pertinents

À l’intérieur de chaque groupe, les noms sont ensuite triés par ordre alphabétique.

Le popover ne présélectionne jamais automatiquement une cible : le choix doit être fait manuellement.

Quand tu appliques une attaque à plusieurs cibles :

- les dégâts sont appliqués à toutes les cibles sélectionnées
- la bannière du haut affiche plusieurs lignes, une par cible touchée
- l’undo de la dernière attaque conserve tout le groupe

## Dégâts et Soins

`Dégâts` applique des dégâts directs au participant.

`Soins` applique des soins directs.

## JS

`JS` ouvre le popover du **Jet de sauvegarde** basé sur les caractéristiques du participant.

## Conditions

Le bouton `Conditions` ouvre le popover dédié à la gestion des états actifs.

Depuis là, tu peux :

- ajouter des conditions
- choisir la durée et les règles d’expiration
- lier la fin d’une condition au tour d’un autre participant

## Notes MJ

Le bouton `Notes MJ` est toujours visible.

Il ouvre un popover modifiable dans lequel tu peux écrire des notes contextuelles sur le participant. Le contenu est sauvegardé à la fermeture du popover.

## Modifier

`Modifier` ouvre le panneau d’édition du participant.

Il sert quand tu dois intervenir plus en profondeur sur :

- initiative
- CA
- PV maximum, actuels et temporaires
- rôle en combat
- données contextuelles liées

## Tour en cours

Quand le combat est actif, le panneau central se concentre entièrement sur le participant dont c’est le tour.

La carte supérieure montre :

- image du participant
- nom
- sous-titre
- CA
- PV
- PV temporaires
- initiative
- vitesse
- inspiration, si le participant est un héros de l’aventure
- conditions actives
- caractéristiques principales

## Panneaux centraux pendant le tour

Sous le résumé du tour, seuls les panneaux qui ont réellement du contenu s’affichent.

Les sections possibles sont :

- `Attaques`
- `Capacités spéciales`
- `Capacités`
- `Description`
- `Sorts`

Tous ces panneaux sont repliables.

Ils utilisent aussi un léger accent visuel :

- `Attaques` rouge
- `Capacités` jaune
- `Capacités spéciales` vert
- `Sorts` bleu clair
- `Description` gris

## Attaques et liens internes

La section `Attaques` est l’un des points les plus forts du combat flat.

Si tu as préparé des liens internes dans les attaques de la fiche de base, tu peux les utiliser directement pendant le combat.

En particulier, le lien **Attaque complète** est très utile parce qu’il :

- exécute le jet d’attaque et les dégâts dans le même popover
- permet de sélectionner une ou plusieurs cibles
- propose automatiquement `Dégâts à appliquer`
- te laisse exclure certaines lignes de dégâts si tu as lancé plusieurs composantes et ne veux en appliquer qu’une partie
- ferme le popover dès que les dégâts sont appliqués

Cela rend les attaques de monstres très rapides à utiliser à la table.

## Personnages à 0 PV ou moins

En combat, les **Héros** suivent une règle différente de celle des PNJ et monstres.

### Héros

Les héros peuvent descendre sous `0` PV.

La règle est :

- entre `0` et `-(PV max - 1)`, le personnage est **Inconscient**
- à `-PV max` ou moins, le personnage meurt définitivement

Quand un héros est à `0` PV ou moins mais n’est pas mort définitivement :

- il reste dans l’affrontement
- le panneau central affiche la carte `Jets de sauvegarde contre la mort`

Cette carte suit :

- réussites
- échecs

et permet d’enregistrer rapidement :

- `Réussite`
- `Échec`

À 3 réussites, le personnage revient à `1` PV. À 3 échecs, il meurt.

### PNJ et Monstres

Pour les non-héros, le comportement est plus simple :

- à `0` PV ou moins, ils sont morts

## Tours, rounds et participants exclus du cycle

Dans le cycle des tours :

- les héros morts définitivement sont exclus
- les PNJ et monstres à `0` PV ou moins sont exclus

Cela signifie qu’un héros **Inconscient** peut encore avoir un tour, justement parce qu’il doit pouvoir gérer ses jets de sauvegarde contre la mort.

## Bannières d’impact et feedback visuel

Quand une attaque touche, DnDino affiche une grande bannière en haut avec un résumé immédiat.

Par exemple :

- qui a frappé
- qui a été touché
- combien de dégâts ont été appliqués
- si le coup a tué la cible

S’il y a plusieurs cibles, la bannière affiche plusieurs lignes dans le même encadré.

La **Fenêtre Joueurs** peut aussi montrer l’animation du coup, en incluant toutes les cibles impliquées dans la même attaque multi-cible.

## Annuler la dernière attaque

Quand tu appliques une attaque, le panneau

- `Annuler la dernière attaque`

apparaît.

Sous le bouton, tu vois un petit résumé de ce qui vient de se passer.

Si la dernière attaque a touché plusieurs cibles, le panneau montre la liste complète des lignes qui seront restaurées.

Quand tu confirmes l’annulation :

- les cibles reviennent à leur état précédent
- une notification de restauration apparaît
- le feedback visuel des cartes se met aussi à jour

## Résumé final de l’affrontement

Quand le combat se termine, le panneau central passe au **Résumé final de l’affrontement** pour le MJ.

Cet écran montre :

- rounds totaux
- durée
- ennemis tués
- dégâts infligés
- dégâts subis

## Ce qui est synchronisé à la fin

Quand tu fermes le combat, DnDino enregistre le résultat dans les enregistrements liés.

Pour les héros de l’aventure, il synchronise :

- PV actuels
- PV temporaires
- conditions manuelles
- état final

Pour les présences du lieu avec état local, il synchronise :

- PV actuels
- PV temporaires
- conditions manuelles
- état final

Le combat met aussi à jour les données liées à la **session live**, y compris :

- dégâts infligés
- dégâts subis
- héros tombés

## Quand le combat donne le meilleur de lui-même

Le combat de DnDino donne le meilleur de lui-même quand tu l’utilises ainsi :

1. tu prépares bien le pré-combat
2. tu utilises le double écran avec la **Fenêtre Joueurs**
3. tu exploites les liens dans les `Attaques` pour monstres et PNJ
4. tu gardes le MJ sur le tracker et les joueurs sur la présentation

!!! tip
    Même si le combat offre beaucoup d’automatisations pour les jets, les attaques complètes et l’application rapide des dégâts, DnDino laisse toujours de la place à une utilisation plus classique des dés. Tu peux continuer à lancer physiquement ou gérer le lancer hors de l’application, et utiliser surtout le combat pour appliquer les valeurs de manière rapide et cohérente, en évitant la partie la plus pénible : recalculer à la main les variations et mises à jour des points de vie à chaque fois.
