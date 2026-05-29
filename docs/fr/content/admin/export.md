Depuis Catima, il y a trois formats d’export possibles : **JSON**, **SQL** ou **CSV**.

En fonction des besoins, choisir l’un ou l’autre des formats:
- **Json et Sql** - à privilégier pour partager les données d'un catalogue avec un.e développeur.euse. Le choix entre le format SQL ou JSON dépend de la préférence personnelle du développeur ou, si la base de données est recréée dans un nouvel environnement, de la base de données cible.
- **Csv** - pour partager les données avec des utilisateurs, par exemple dans Excel ou équivalent. Les fichiers csv exportés peuvent également servir de modèle pour importer de nouvelles données en masse dans Catima.


### En résumé

> Quelques exemples d'utiliation de ces trois formats


|  | Catima (JSON)                       | SQL          | CSV          | 
|--------------| ------------------------------------|--------------|--------------|
| **Cas d'usages** | Partager les données du catalogue avec un développeur, Recréer la base dans un autre système | Partager les données du catalogue avec un développeur, Recréer la base dans un autre système  | Partager avec des utilisateurs, Import de données en masse|
| **Applications compatibles**|  PostgreSQL, etc ... |  MYSQL, MariaDB, etc ... | Excel, Numbers | 
| **Utile pour réimport?**| Oui, pour les *ensemble de choix*   | Non  | Oui, comme modèle d'import de données des fiches |

