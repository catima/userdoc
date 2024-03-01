Lors de la création d'un choix, il est possible de lui associer un **parent**.
![](assets/datation/choix_parent.png)

La hiérarchie des choix est visible dans le mode **Set up** de l'ensemble de choix. Pour modifier l’ordre, sélectionner l’élément en cliquant sur la croix et le déplacer à l’emplacement désiré de la hiérarchie. ![](datation/hierarchie.png)

**ATTENTION** il n'est pas recommandé de créer plusieurs niveaux de hiérarchisation des choix car cela entraîne de la confusion lors de la recherche par choix parent. Lors d'une recherche par ensemble de choix, les enfants d'enfants ne sont pas inclus.

### Exemple

![](assets/datation/3niveaux.png)

- Le choix 20ème siècle
  - Le choix Seconde Guerre Mondiale est l'enfant de 20ème siècle
                - Le choix année 1940 est l'enfant de Seconde Guerre Mondiale

#### Incidence sur la recherche

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

![](assets/datation/secondeguerreavec.png)

> Le choix enfant ressort mais pas le choix parent

On recherche les objets datés du 20ème siècle en incluant les enfants **OU** les objets datés de la Seconde Guerre Mondiale en incluant les enfants

![](assets/datation/20emeouseconde.png)

> Les 3 niveaux ressortent

![](assets/datation/20emeouseconderesultat.png)

### En résumé

La hierarchie des choix dans les ensembles de choix standard ou de type datation a un impact important sur la recherche. Plus les choix sont bas dans la hiérarchie plus il sera difficile de les faire ressortir lors de la recherche par ensemble de choix.