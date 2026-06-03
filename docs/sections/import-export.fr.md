# Import et export

DnDino permet d'exporter et d'importer du contenu pour le déplacer entre plusieurs installations, créer des copies de travail ou partager du matériel avec d'autres Maîtres du Donjon.

Les importations ne remplacent jamais automatiquement les données existantes : avant l'enregistrement, tu peux vérifier ce qui sera ajouté, remplacé ou ignoré.

## Sorts

Les sorts peuvent être exportés dans un fichier JSON.

Pendant l'importation, DnDino distingue :

- les nouveaux sorts
- les sorts portant le même nom déjà présents dans la base

Pour chaque sort, tu peux choisir de :

- l'importer comme nouvelle fiche
- remplacer une fiche existante
- l'ignorer

Lorsqu'un sort du même nom existe déjà, l'écran de révision affiche une comparaison entre la fiche présente et celle importée. Tu peux ainsi contrôler le niveau, l'école, le manuel, les classes, le temps d'incantation et la durée avant de décider.

Des actions groupées permettent aussi de gérer plusieurs conflits à la fois, par exemple ignorer tous les sorts déjà présents ou les importer tous comme nouvelles fiches.

## Personnages

Les personnages sont exportés dans un paquet ZIP qui peut contenir :

- la fiche du personnage
- les images liées
- les liens vers les sorts
- les données nécessaires pour reconstruire la fiche dans une autre installation

Pendant l'importation, les personnages portant le même nom ne sont pas remplacés automatiquement. Tu peux les importer comme nouveaux, remplacer une fiche existante ou les ignorer.

Si le personnage importé possède des sorts liés, DnDino essaie de les associer aux sorts déjà présents en utilisant le nom. Si plusieurs sorts correspondent, tu peux choisir lequel utiliser.

Lorsque tu importes des personnages dans une base déjà riche, vérifie toujours les liens vers les sorts : deux sorts peuvent avoir le même nom mais venir de manuels ou de versions différentes.

## Aventures

Les aventures sont exportées dans un paquet ZIP avec les données nécessaires pour reconstruire l'aventure.

Une aventure importée est toujours créée comme **nouvelle aventure**. DnDino ne remplace pas une aventure existante, afin d'éviter toute perte de lieux, personnages ou sessions d'une campagne active.

Le flux conseillé se fait par étapes :

1. importer ou relier les sorts
2. importer ou relier les personnages
3. importer l'aventure

Dans la révision de l'aventure, DnDino sépare les parties principales :

- sorts inclus dans le paquet
- personnages inclus dans le paquet
- structure de l'aventure

Pour les sorts et les personnages, tu choisis comment gérer les fiches déjà présentes. Ensuite, l'aventure est importée en reliant les bons personnages aux lieux, présences et autres contenus du paquet.

## Équipement, dons et glossaire

L'équipement, les dons et les entrées du glossaire peuvent aussi être exportés et importés séparément.

L'export crée des fichiers JSON dédiés, utiles pour partager seulement une partie du matériel sans exporter toute une aventure.

Pendant l'import, DnDino sépare les nouveaux enregistrements de ceux qui ont déjà une correspondance dans la base de données. Pour chaque enregistrement, vous pouvez l'importer comme nouveau, remplacer l'existant ou l'ignorer.

Pour l'équipement, la correspondance utilise le nom et la catégorie, afin de garder séparés armes, armures, outils et matériel. Pour les dons, le type de don est également pris en compte. Pour le glossaire, la référence principale est le nom de l'entrée.

Lorsqu'un enregistrement similaire existe déjà, l'écran de vérification compare le contenu présent avec celui qui est importé. Utilisez les actions groupées pour ignorer, importer ou remplacer plusieurs enregistrements à la fois lorsque le fichier contient beaucoup d'éléments.

## Contrôles avant l'importation

Avant d'importer des paquets contenant des images, DnDino vérifie que le fichier est lisible et qu'il y a assez d'espace libre pour copier les médias dans le conteneur de l'app.

Si le fichier est endommagé, incomplet ou incompatible, l'importation s'arrête avec un message d'erreur au lieu de créer des données partielles.

## Bonnes pratiques

Avant d'importer du contenu important :

- crée une sauvegarde de l'app
- importe d'abord les sorts si beaucoup de personnages les utilisent
- vérifie les fiches portant le même nom avant de les remplacer
- utilise la comparaison ancien/nouveau quand tu hésites
- importe les aventures comme nouvelles, puis vérifie les liens, lieux et images

L'importation est conçue pour protéger la base de données : en cas de doute, choisis `Importer comme nouveau` ou `Ignorer` plutôt que de remplacer.
