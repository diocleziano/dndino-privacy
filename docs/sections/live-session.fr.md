# Session live

La **Session live** est le contexte opérationnel de la partie en cours. Ce n’est pas simplement un minuteur, mais un système qui tient ensemble :

- le temps de jeu de la session
- la timeline des événements importants
- les notes MJ rapides
- l’état des lieux visités
- les quêtes actives ou terminées
- les combats joués
- les statistiques agrégées de la session

En pratique, quand une session live est active, DnDino sait quelle campagne est en cours et utilise ce contexte pour relier entre elles plusieurs parties de l’application.

## À quoi elle sert

La session live est utile quand tu veux utiliser DnDino pendant une vraie partie à table, et pas seulement pendant la préparation.

Elle sert à :

- suivre le temps de la session
- garder une timeline ordonnée des événements principaux
- noter rapidement des informations de MJ
- marquer les lieux en visite ou déjà visités
- voir un résumé dynamique de la session
- récupérer automatiquement les données venant du combat

## Où elle se lance

La session live se lance depuis le contrôle au centre de la **topbar** quand tu es dans une page de l'aventure, par exemple dashboard, lieux ou combat.

S'il n'existe aucune session active, le contrôle affiche l'action de démarrage. Quand tu l'utilises, DnDino demande confirmation puis crée une nouvelle session live pour l'aventure courante.

Tu n'as donc pas besoin de revenir à la dashboard uniquement pour lancer la session : la commande reste disponible là où tu travailles.

## Une seule session live à la fois

DnDino ne gère qu’une seule session live active à la fois.

Si une session est déjà ouverte dans une autre aventure :

- la nouvelle aventure ne peut pas en lancer une deuxième
- la dashboard montre un avertissement signalant que la session active appartient à une autre campagne

## Ce qui se passe lorsqu’une session live est active

Quand une session live est en cours :

- la barre supérieure affiche son état
- le minuteur continue à se mettre à jour
- les lieux suivent ce contexte
- la timeline commence à collecter des événements
- le combat peut lui aussi envoyer des données à la session

La session live devient donc le fil conducteur de la partie en cours.

## État de la session

La session live peut être dans trois états :

- active
- en pause
- interrompue

### Active

C’est l’état normal pendant que la session est en cours. Le minuteur continue d’avancer et les événements sont enregistrés avec le bon temps écoulé.

### En pause

La session peut être mise en pause depuis la topbar.

Quand elle est en pause :

- le minuteur s’arrête
- la session reste malgré tout ouverte
- elle peut être reprise plus tard

### Interrompue

Si l’application est fermée alors que la session est encore active, DnDino la rouvre comme `interrompue` au prochain lancement et enregistre un événement dédié dans la timeline.

Cela permet de :

- ne pas perdre la session
- comprendre qu’une interruption a eu lieu
- reprendre le travail manuellement

## Contrôle Session live dans la topbar

Dans les pages de l'aventure, la topbar affiche le contrôle de session live au centre.

Si la session appartient à l’aventure ouverte, le contrôle affiche :

- titre de la session
- minuteur en temps réel
- état (`En cours` ou `En pause`)
S’il n’y a pas de session live active :

- la commande pour lancer la session live de l'aventure courante apparaît

Si une session est active mais appartient à une autre aventure :

- le contrôle indique que la session live est déjà utilisée ailleurs

## La session live dans la topbar

Quand une session live est active, la barre supérieure de l’application affiche un indicateur dédié.

Pour la description complète de la topbar, consulte la page `Topbar`.

![Session live active dans la topbar](../images/en_sessionelive_attiva_topbar.png){ .img-shot }

## Le panneau rapide de la session live

Depuis le panneau rapide de la session, tu peux effectuer des actions très rapides sans quitter l’écran actuel.

Tu y trouves :

- `Pause` ou `Reprendre`
- `Fermer et sauvegarder`
- éditeur rapide de `Note MJ`
- timeline de la session
- actions rapides sur le lieu actuellement en visite
- résumé live compact

## Note MJ rapide

Dans le popover de la session live, tu peux écrire une **Note MJ** et l’ajouter immédiatement à la timeline.

Cela est utile pour noter rapidement :

- les décisions des joueurs
- des pistes narratives
- des conséquences à retenir
- des idées improvisées apparues pendant la partie

Les notes MJ sont enregistrées comme événements de la timeline.

## Timeline de la session

La timeline est le journal chronologique de la session live.

Chaque événement mémorise :

- titre
- détail
- moment de la session où il s’est produit

La timeline peut contenir des événements système et des notes MJ.

## Types d’événements enregistrés

Les événements les plus importants enregistrés automatiquement par DnDino incluent :

- `Session démarrée`
- `Session mise en pause`
- `Session reprise`
- `Session interrompue suite à la fermeture de l’application`
- `Entrée dans le lieu`
- `Sortie du lieu`
- `État du lieu mis à jour`
- `Quête activée`
- `Quête terminée`
- `Combat commencé`
- `Combat terminé`
- `Note MJ`

## Lien avec les lieux

La session live est directement liée aux lieux de l’aventure active.

Quand tu mets à jour un lieu dans le contexte de la session :

- le changement d’état est enregistré
- la timeline se met à jour
- le résumé live change en conséquence

Les données les plus importantes suivies côté lieux sont :

- lieux en visite
- lieux visités
- quêtes actives
- quêtes terminées

## Fermeture automatique du lieu précédent en visite

Dans les réglages, il existe aussi une logique liée à la session live : lorsqu’un lieu passe en `En visite`, le lieu qui était auparavant en visite peut être marqué automatiquement comme `Visité`.

Cette fonction ne vaut que lorsqu’une session live active existe et elle est très utile pour garder un suivi cohérent de l’exploration.

## Recréer une session live déjà jouée

Si tu as oublié de lancer la session live pendant la partie, tu peux la recréer manuellement depuis la carte **Sessions** du tableau de bord de l’aventure.

La session recréée n’est pas une simple note : elle est sauvegardée comme session live et utilise les données réelles déjà présentes dans l’aventure.

Lors de la création, tu peux indiquer :

- l’heure de début et l’heure de fin
- les lieux visités pendant la session
- les notes de session

DnDino inclut automatiquement les combats terminés qui ont commencé dans l’intervalle choisi. Les statistiques de la session peuvent ainsi utiliser les dégâts, les ennemis vaincus, la durée des combats et les temps moyens des tours déjà enregistrés par les combats réels.

Cette fonction sert à récupérer une session jouée sans perdre la valeur des statistiques.

## Supprimer une session

Dans la liste des sessions, chaque ligne dispose d’un bouton de suppression. Avant la suppression, DnDino affiche une confirmation, car l’opération supprime définitivement la session sauvegardée.

## Résumé live

![Résumé de session live](../images/en_sessionelive_riepilogo_1.png){ .img-shot }
![Graphiques de session live](../images/en_sessionelive_riepilogo_2.png){ .img-shot }


Le résumé live agrège les données les plus importantes collectées pendant la session.

Parmi les principales valeurs, on trouve :

- lieux visités
- lieux en visite
- quêtes actives
- quêtes terminées
- combats joués
- ennemis vaincus
- héros tombés
- durée totale des combats

La session live conserve aussi deux résumés très utiles pour les personnages :

- dégâts infligés par les héros
- dégâts subis par les héros
- temps moyen des tours, lorsqu'il provient de combats terminés

## Intégration avec le combat

La session live et le combat sont étroitement liés.

Quand tu démarres un combat pendant une session live, DnDino enregistre :

- `Combat commencé`

Pendant le combat, il peut collecter :

- les données agrégées utiles au résumé et aux statistiques

Quand tu fermes le combat, il enregistre :

- `Combat terminé`
- durée de l’affrontement
- ennemis vaincus
- héros tombés

## Dégâts infligés et dégâts subis

La session live suit les dégâts à travers deux classements séparés :

- `Dégâts infligés par les personnages`
- `Dégâts subis par les personnages`

Ce comptage est pensé uniquement pour les héros de l’aventure, et non pour tous les participants du combat.

Le détail de session sauvegardée peut aussi afficher des graphiques dédiés aux combats terminés pendant cette session :

- dégâts infligés par combat
- dégâts subis par combat
- temps moyen des tours par combat

Chaque combat reste sur l'axe horizontal en ordre chronologique. Les personnages qui ont participé apparaissent même lorsqu'ils ont infligé ou subi `0` dégât dans un combat, afin de conserver une série lisible. Si un personnage n'a pas participé à un combat, il n'est pas ajouté à ce point.

Ces graphiques permettent de comprendre qui a le plus pesé pendant la session et qui a absorbé le plus de dégâts.

Le graphique des temps de tour aide à voir combien de temps les héros et le MJ prennent en moyenne pendant les combats de la session.

## Héros tombés

Quand un combat se termine, le résumé de la session live peut aussi augmenter le compteur des **héros tombés**.

Cette donnée est alimentée directement par le résultat final du combat.

## Session live et Fenêtre Joueurs

La session live ne se confond pas avec la **Fenêtre Joueurs**, mais les deux sont liées.

La session live fournit le contexte général de la partie, tandis que la fenêtre joueurs est le canal de présentation visuelle.

En particulier :

- pendant le combat, la fenêtre joueurs peut montrer l’intro, le tour en cours et le résumé final
- hors combat, la fenêtre joueurs peut quand même servir à montrer des images et des contenus du contexte actif

## Fermeture et sauvegarde

Quand tu choisis `Fermer et sauvegarder`, DnDino :

- finalise la session
- sauvegarde les données collectées
- persiste la timeline dans la session liée à l’aventure
- ferme le contexte live global

Après fermeture, la session reste consultable comme session sauvegardée.

## Affichage d’une session sauvegardée

Une session live déjà terminée peut être rouverte comme vue de détail.

Dans le panneau de détail, tu trouves :

- résumé et timeline
- durée enregistrée
- lieux visités
- combats joués
- ennemis vaincus
- héros tombés
- classements des dégâts infligés et subis par les personnages
- graphiques des dégâts infligés et subis dans les combats de la session

## Quand il est pertinent d’utiliser la session live

La session live est particulièrement utile quand tu veux :

- garder DnDino ouvert pendant la partie
- noter rapidement ce qui se passe réellement à table
- savoir quels lieux ont été visités
- avoir une timeline ordonnée des événements clés
- faire remonter automatiquement le combat dans le résumé de session

## En pratique

La session live est le pont entre :

- préparation
- gestion opérationnelle de la partie
- mémoire finale de la session

Bien utilisée, elle réduit fortement le risque de perdre des informations importantes pendant le jeu et rend beaucoup plus simple la reconstruction, après coup, de ce qui s’est réellement passé dans la campagne.
