Catima offre la possiblité de récupérer les informations en format JSON d'une manière dynamique avec une API. *Il faut que cette option soit activée par un administrateur système. Si elle ne l'est pas, prendre contact avec les responsables.*

<a id="accesdonnes">
### Qui a accès au données

Pour pouvoir utiliser les données avec l'API, il faut soit avoir un compte Catima et accès au catalogue dont on souhaite récupérer les données (méthode mot-de-passe), soit avoir une clé API de ce catalogue (méthode clé API). Les données accessibles avec la méthode d'authentification par mot-de-passe sont les mêmes que celles auxquelles l'utilisateur a accès alors que la méthode clé API permet un accès complet au catalogue. **Ne jamais partager une clé API publiquement.**.

Créer ou supprimer une clé API depuis la rubrique **API** en mode "Set Up". Plusieurs clés peuvent exister en même temps. 

L'ensemble des requêtes disponibles sont consultables [dans la documentation](https://catimalb.unil.ch/api-docs/index.html).

<a id="mode-data">
### Mode data only

Avec cette option activée, Catima est utilisé uniquement pour stocker les données et ne générera pas de site pour voir les fiches et naviguer entre elles.

**En mode data only:**

- les fiches ne sont pas accessibles via un navigateur par des visiteurs (pas de site)
- pas d'options de visualisation (menu, pages, statistiques)
- l'accès au catalogue par statut (editeur, reviewer, administrateur) est toujours possible

Ceci est utile si le catalogue est utilisé uniquement comme base de données et ne nécessite pas de site pour leur visualisation. 

*Il faut que cette option soit activée par un administrateur système. En cas d'intérêt, prendre contact avec les responsables.*