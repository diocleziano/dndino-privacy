# FAQ

Cette section regroupe des réponses rapides aux questions les plus fréquentes sur DnDino.

Si vous avez besoin d'une explication complète d'un écran précis, il vaut mieux ouvrir ensuite la page dédiée du guide. Cette FAQ sert surtout pour les cas pratiques les plus courants.

## Comment reprendre immédiatement ma dernière campagne ?

Ouvrez l'écran `Accueil` et utilisez la carte de la **dernière aventure**.

Depuis cette carte, vous pouvez :

- ouvrir directement le tableau de bord de l'aventure
- revenir au dernier lieu visité, s'il est disponible

C'est la façon la plus rapide de reprendre votre préparation sans repasser à chaque fois par la liste complète des aventures.

## Quelle est la différence entre une fiche de base, un personnage d'aventure, une présence de lieu et un participant au combat ?

La **fiche de base** est l'enregistrement général du personnage ou de la créature.

À partir de cette fiche, DnDino peut créer des enregistrements contextuels distincts :

- le **personnage d'aventure**, utilisé dans une campagne
- la **présence de lieu**, utilisée dans les lieux
- le **participant au combat**, utilisé pendant un affrontement

Ce système permet de séparer :

- les noms contextuels
- l'initiative
- les PV actuels
- les notes du MJ
- l'état local du lieu ou du combat

Autrement dit, la fiche de base reste la référence générale, tandis que les enregistrements contextuels servent au travail pratique en partie.

## Comment ajouter un héros à l'aventure ?

Ouvrez le `Tableau de bord de l'aventure`, puis allez dans le panneau `Personnages`.

Depuis là, vous pouvez :

- ajouter un personnage existant
- créer un nouveau personnage avec `Créer un personnage`

Si vous créez un personnage depuis le sélecteur, l'enregistrement vous ramène au panneau de sélection et la liste se met à jour immédiatement.

## Comment ajouter une présence à un lieu ?

Ouvrez le lieu puis allez dans le panneau `Présences`.

Depuis là, vous pouvez ajouter :

- un héros déjà lié à l'aventure
- un `PNJ`
- un `Monstre`

Gardez en tête cette différence importante :

- un `PNJ` reste unique dans ce lieu
- un `Monstre` peut être ajouté plusieurs fois

Cela permet d'avoir plusieurs occurrences du même monstre dans un même lieu, tout en évitant les doublons non voulus de PNJ.

## Puis-je changer le nom d'un monstre sans modifier sa fiche de base ?

Oui.

C'est justement l'une des raisons pour lesquelles DnDino utilise des enregistrements contextuels.

Vous pouvez renommer un monstre :

- en pré-combat
- dans les présences des lieux
- dans d'autres contextes locaux où le nom utilisé en jeu doit être plus pratique

Cela ne modifie pas le nom de la fiche de base d'origine.

## Comment lier rapidement un personnage ou un lieu dans une description ?

Dans les champs de texte qui prennent en charge les liens internes, utilisez la commande `Lien`.

Depuis ce menu, vous pouvez créer des liens vers :

- des personnages
- des lieux
- des sorts
- des règles
- des dons

C'est particulièrement utile :

- dans `Lieux`, pour relier d'autres lieux ou personnages mentionnés dans la description
- dans `Personnages`, surtout dans `Attaques`, pour relier des jets ou des références utiles

## À quoi servent les liens dans les Attaques des monstres ?

Ils transforment un texte descriptif en outil de jeu.

Dans les champs rich text des attaques, vous pouvez insérer des liens comme :

- `Attaque complète`
- `Jet libre`
- `Lancer les dés`
- `Jet d'attaque`

Cela permet de :

- lancer rapidement les dés
- appliquer les dégâts aux cibles
- relier d'autres entrées de l'application

C'est l'une des meilleures façons de rendre une fiche de monstre réellement utile pendant le combat.

## Suis-je obligé d'utiliser les jets automatiques en combat ?

Non.

DnDino propose beaucoup d'automatisations, mais ne vous oblige pas à les utiliser.

Vous pouvez toujours :

- lancer les dés physiquement à la table
- lire les résultats de manière classique
- appliquer les dégâts manuellement

L'application vous aide surtout à éviter les mises à jour répétitives des PV et les calculs mentaux.

## Le combat fonctionne-t-il bien avec un seul écran ?

Oui.

Le `Combat Flat` fonctionne très bien sur un seul écran.

Le double écran avec la `Fenêtre Joueurs` est très pratique pour la présentation, mais ce n'est pas obligatoire. Sur un seul moniteur, vous pouvez utiliser le combat sans problème et définir dans les réglages le comportement de la fenêtre joueurs.

## Puis-je choisir combien d'informations les joueurs voient pendant le combat ?

Oui.

Dans `Réglages > Combat`, vous pouvez notamment décider si les joueurs voient :

- le numéro du round
- les PV
- les conditions
- le prochain tour
- le vrai nom des ennemis
- les détails des PNJ et des monstres

Cela vous permet de choisir entre un combat plus transparent ou une présentation plus proche d'un écran de MJ.

## Comment fonctionne le résumé final du combat ?

À la fin du combat, DnDino clôt l'affrontement et synchronise les données contextuelles avec les enregistrements liés.

En plus :

- le MJ voit le résumé final dans l'écran de combat
- les joueurs peuvent voir un résumé dans la `Fenêtre Joueurs`, si l'option est activée

Le résumé public est centré sur les personnages, pas sur les ennemis.

## Que se passe-t-il si un héros tombe en dessous de 0 PV ?

Les héros peuvent descendre en négatif.

La règle gérée par l'application est la suivante :

- entre `0` et `-(PV max - 1)`, le héros est `Inconscient`
- à `-PV max` ou moins, le héros meurt définitivement

Pendant le combat, lorsqu'un héros est inconscient, DnDino affiche aussi le panneau des **jets de sauvegarde contre la mort**.

## Comment montrer une image aux joueurs ?

DnDino utilise une fenêtre dédiée pour l'affichage côté joueurs.

Vous pouvez l'utiliser :

- pendant le combat
- pour les images de l'aventure
- dans d'autres flux qui prennent en charge la présentation

Le comportement de cette fenêtre se règle dans `Réglages > Médias` et, en partie, dans `Réglages > Combat`.

## Comment sauvegarder mes données ?

Allez dans `Réglages > Base de données`.

Depuis là, vous pouvez :

- voir où se trouvent les données de l'application
- ouvrir le dossier des données
- ouvrir le dossier des sauvegardes
- créer manuellement un instantané
- restaurer un instantané
- restaurer depuis iCloud, si configuré

Dans la même section, vous pouvez aussi choisir :

- la fréquence des sauvegardes automatiques
- le nombre maximum d'instantanés conservés

## Où trouver des informations techniques sur la base si quelque chose semble anormal ?

Allez dans `Réglages > Diagnostic`.

Là, vous pouvez vérifier :

- le chemin de la base de données
- la présence du fichier
- sa taille
- sa date de dernière modification
- la version de SQLite
- les tables détectées et le nombre d'enregistrements

C'est la bonne section à consulter si vous voulez savoir si un problème est seulement visuel ou s'il touche réellement les données enregistrées.

## Comment contacter le support ?

Ouvrez `Réglages > Support`.

Depuis là, vous pouvez :

- envoyer une demande de support
- envoyer une suggestion
- copier l'adresse e-mail de référence

Utilisez `Support` quand quelque chose ne fonctionne pas ou n'est pas clair. Utilisez `Suggestion` quand vous voulez proposer une amélioration ou une nouvelle fonctionnalité.

!!! tip
    Si une réponse ici vous semble trop brève, utilisez la FAQ comme point de départ puis ouvrez la page dédiée du guide, par exemple `Personnages`, `Lieux`, `Combat` ou `Réglages`.
