Quelques questions doivent être résolues avant de commencer la création d'un champ **Datation**.

1. Quel est le niveau de précision: par période, par année, par jour/mois/année ?
2. Est-ce que les dates/périodes sont exclusivement après JC ou des dates/période avant JC sont aussi possibles ?
3. Quelles méthodes de saisie doivent être proposées ?
    - Saisie manuelle par date/heure uniquement (passer directement à l'étape 2 pour créer le champ datation)
    - Entrée par ensemble de choix (commencer par l'étape 1 pour configurer un ensemble de choix avant la création du champ datation lui-même)
    - Les deux (commencer à l'étape 1 pour configurer un ensemble de choix de type datation)

> Des modifications du champ sont possibles par la suite mais peuvent entrainer la perte de certaines données.

#### Étape 1: Création d'un ensemble de choix de type datation

Cette étape est nécessaire pour la saisie de dates par ensemble de choix et doit être effectuée préalablement à la création du champ datation.

En mode **Setup**, sélectionner **Ensemble de choix** dans la colonne de gauche et cliquer sur *+ Nouvel ensemble de choix*. Sélectionner le type *Datation*, choisir si les dates avant JC sont autorisées ou non ainsi que le format.

*Le format, ainsi que le type d'ensemble de choix (Datation ou Standard) ne peuvent plus être modifiés une fois l'ensemble de choix créé.*

> Il est recommandé de choisir le format le plus large possible. Si la datation se fait par siècle, choisir **Y** (années) uniquement et non un format plus fin  qui incluerait des mois et jours sans quoi cela peut poser des conflits lors des recherches. Si une datation par jour/mois/année est nécessaire, choisir **YMD** et ne pas inclure les heures et secondes.

![](assets/datation/creation_ens_choix.png)

Editer l'ensemble de choix nouvellement créé et cliquer sur *+ Nouveau choix* pour ajouter une nouvelle période ou date précise. Il y a plusieurs possibilités:

- les champs *Date de début* et *Date de fin* sont remplis par deux dates différentes. Ils définissent une période allant d'une date à une autre, toutes les dates entre les deux étant aussi incluses.
- uniquement le champ *Date de début* est rempli. Il définit une période après la date de début indiquée, date de début incluse.
- uniquement le champ *Date de fin* est rempli. Il définit une période avant la date de fin indiquée, date de fin incluse.
- Remplir les deux champs avec les mêmes informations permet de définir une date fixe. Par exemple *Date de début*: 1990 et *Date de fin*: 1990.

![](assets/datation/avantJCvsnon.png)

> Les dates de début et de fin sont **inclusives**. Une période définie avec la date de début **1990** et la date de fin **1999** comprend les années 1990, 1991, 1992, 1993, 1994, 1995, 1996, 1997, 1998 et 1999. Faire ensuite une recherche sur une ou plusieurs de ces années retournera les fiches datées de cette période.

<a id="hierarchie-choix"></a>
##### Hiérarchie des choix

Lors de la création d'un choix, il est possible de lui associer un **parent**.
![](assets/datation/choix_parent.png)

La hiérarchie des choix est visible dans le mode **Set up** de l'ensemble de choix. Pour modifier l’ordre, sélectionner l’élément en cliquant sur la croix et le déplacer à l’emplacement désiré de la hiérarchie. ![](datation/hierarchie.png)

**ATTENTION** il n'est pas recommandé de créer plusieurs niveaux de hiérarchisation des choix car cela entraîne de la confusion lors de la recherche par choix parent. Lors d'une recherche par ensemble de choix, les enfants d'enfants ne sont pas inclus.

**Exemple**
![](assets/datation/3niveaux.png)

- Le choix 20ème siècle
  - Le choix Seconde Guerre Mondiale est l'enfant de 20ème siècle
    - Le choix année 1940 est l'enfant de Seconde Guerre Mondiale

###### Incidence sur la recherche

On recherche les objets datés du 20ème siècle sans inclure les enfants

![](assets/datation/20emesansenfants.png)

> Aucun enfant ne ressort dans la recherche

![](assets/datation/20emeresultat.png)

On recherche les objets datés du 20ème siècle en incluant les enfants

![](assets/datation/20emeavecenfants.png)

> Le premier niveau d'enfants ressort

![](assets/datation/20emeavecresultat.png)

On recherche les objets datés de la Seconde Guerre Mondiale sans inclure les enfants

![](assets/datation/secondeguerresans.png)

> Le choix parent ne ressort plus

![](assets/datation/secondeguerresansresultat.png)

On recherche les objets datés de la Seconde Guerre Mondiale en incluant les enfants

> Le choix enfant ressort mais pas le choix parent

![](assets/datation/secondeguerreavec.png)

On recherche les objets datés du 20ème siècle en incluant les enfants **OU** les objets datés de la Seconde Guerre Mondiale en incluant les enfants

![](assets/datation/20emeouseconde.png)

> Les 3 niveaux ressortent

![](assets/datation/20emeouseconderesultat.png)

##### En résumé
La hiérachie des choix dans les ensembles de choix standard ou de type datation a un impact important sur la recherche. Plus les choix sont bas dans la hiérarchie plus il sera difficile de les faire ressortir lors de la recherche par ensemble de choix.

#### Étape 2: Création du champ datation

En mode **Set Up**, sélectionner le type de fiche sur la colonne de gauche et cliquer sur *+ Ajouter > Champ de datation*. En plus du nom, nom au pluriel et slug ainsi que des options d'affichage, le dernier paramètre définit le ou les formats utilisés pour la saisie des données:

1. **Manuelle**: cocher cette case pour permettre l'entrée manuelle de dates et périodes. Le format des données est défini en choisissant une option dans le menu déroulant. *Pour permettre l'utilisation de dates avant JC, cocher la case sous le menu déroulant*.
2. **Par ensemble de choix**: cocher cette case et sélectionner un ensemble de choix **de type datation** pour permettre la sélection de dates ou périodes selon un ensemble de choix préalablement créé. L'acceptation ou non de dates négatives est définie directement dans les paramètres de l'ensemble de choix dans *Set up > Ensemble de choix*.

**ATTENTION !** Si les deux types de saisie sont activés (manuelle et par ensemble de choix), il est recommandé de choisir le même format de date.
Le cas échéant, veiller à avoir défini des formats **cohérents**. Le format de date le plus large doit toujours être inclus dans le format le plus fin. Par exemple, si l'ensemble de choix est en années, la saisie manuelle peut-être en mois-années mais pas uniquement en mois.

![](assets/datation/config_datation.png)