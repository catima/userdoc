
#### Rappel: différences entre les champs "Date" et "Datation" 

Le champ **Date** permet l'entrée d'une date précise sur une fiche. Cette date est unique. Cela peut être par exemple la date de naissance d'une personne, l'année de construction d'un bâtiment ou l'heure et la date d'une représentation, lorsque celle-ci est connue.

Le champ de **Datation** accepte une date de début et une date de fin, permettant la création de périodes et la recherche sur toutes les dates contenues dans cette période. Ce champ est approprié quand la date est incertaine ou inconnue.

> Le champ datation est un champ très complexe pour lequel a été réalisé un [catalogue d'exemple](https://catima.unil.ch/datation-exple/fr) permettant de mieux comprendre comment utiliser ce champ et comprendre son comportement lors des recherches.


### Chercher par date avec la recherche simple

Rechercher une date dans la barre de recherche retournera uniquement les fiches dans lesquelles les caractères recherchés figurent tels quels dans un des champs. 

>Note: Ainsi, entrer deux dates dans la barre de recherche ne calculera pas une période mais retournera les fiches dans lesquelles figurent textuellement les deux dates.


### Rechercher par date avec la recherche avancée

La recherche avancée est optimale pour effectuer des recherches précises sur les dates (de type "Date" simple ou "Datation"). 

Grâce aux listes déroulantes, il est possible de préciser des périodes de diverses façons. 

![](assets/datation/recherche_avancee.png)

Les listes déroulantes sur la droite permettent de préciser:
- si la recherche se fait sur une date exacte (1),
- après une date (2) 
- ou avant une date (3).

#### Spécificités liées au champ ***"Date"***

La recherche par date est également possible en spécifiant une période (choisir 'entre les dates') ou en l'excluant (choisir 'en dehors des dates')

#### Spécificités liées au champ ***"Datation"***

La liste déroulante (4) permet d'effectuer des recherches par ensemble de choix.

Le critère ***Exclure*** (5) permet d'exclure l'un ou l'autre des types de datation. Exclure les fiches avec **datation manuelle** ne retournera que les fiches avec une **datation par ensemble de choix** et inversement.

Les critères peuvent être cumulés à l'aide des opérateurs de recherche "et" (6), "ou" (7) et "sauf" (8) qui se trouvent sur la gauche. De nouvelles lignes (et, ou , sauf) peut être ajoutée à l'aide du bouton **+**.

L'opérateur qui se trouve avant la première ligne (6) se réfère aux autres champs de recherche. Les opérateurs suivants permettent de faire entrer en interaction plusieurs critères de type "datation".

>  **Rappel:**
> 
> **ET** (6): tous les critères doivent être remplis
> 
> **OU** (7): l'un ou l'autre des critères doit être rempli
> 
> **SAUF** (8): le critère doit être exclu