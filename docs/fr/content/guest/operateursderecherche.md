Une recherche avancée s'effectue en entrant un ou plusieurs critères de recherche puis : en les cumulant (par défaut, opérateur "**ET**"), en les excluant (opérateur "**SAUF**") ou en élargissant (opérateur "**OU**").

> **Note** : une recherche cohérente devrait inclure au moins un critère avec l'opérateur "**ET**". La seule exception possible est l'utilisation de l'opérateur "**SAUF**" seul, qui fonctionne comme le pendant inverse de "**ET**".


**Opérateur "ET" (par défaut):**

Ici les critères se **cumulent**, c'est-à-dire que les fiches doivent correspondre à tous les critères entrés pour être incluses dans les résultats. Il s'agit de l'opérateur proposé par défaut pour chaque critère, car il correspond aux situations de recherche les plus fréquentes. 

> **Exemple** : Pour obtenir la liste des bâtiments de **l'Université de Lausanne** contenant l'expression "**Amphi**" (à savoir "**Amphi**max" et "**Amphi**pole"), la recherche consiste à entrer "Amphi" comme "Nom du bâtiment" et choisir "Université de Lausanne" comme "Université".

![](assets/search/adv_search_ex_AND.png)


**Opérateur "SAUF" :**

Lorsqu'un critère de recherche est accompagné de l'opérateur "**SAUF**", seuls les résultats ne **correspondant pas** à ce critère seront affichés.

> **Exemple** : Pour obtenir la liste des bâtiments de l'Université de Lausanne ne **contenant PAS** l'expression "***nef***" (pour exclure "Internef" et "Extranef"), la recherche consiste à entrer "nef" comme "Nom du bâtiment" avec l'opérateur "SAUF" et choisir "Université de Lausanne" comme "Université".

> **Note** : l'opérateur "**SAUF**" se combine avec tous les autres opérateurs "**ET**" et "**SAUF**" quelle que soit la position des critères.

![](assets/search/adv_search_ex_NOT.png)


**Opérateur "OU" :**

En choisissant l'opérateur "OU", on souhaite obtenir une liste de résultats contenant toutes les fiches pour lequelles au moins un des critères est vrai. 

> **Exemple** : Pour obtenir la liste des bâtiments correspondant soit au critère "Université de Lausanne" soit "Université de Genève" comme "Université", entrer ces deux critères (en ajoutant une ligne *via* le bouton "+") et les accompagner de l'opérateur "OU".


![](assets/search/adv_search_ex_OR.png)


**Utilisation combinée des opérateurs "ET", "SAUF" et "OU"**

Il est possible d'utiliser les trois opérateurs dans une recherche. L'ordre dans lequel les critères sont saisis n'a pas d'incidence sur les résultats. C'est le type d'opérateur qui détermine comment chaque critère est traité. Les règles suivantes s'appliquent dans cet ordre :
1. Tout d'abord, les critères "**ET**" déterminent l'ensemble de base de résultats
2. Ensuite, les critères "**SAUF**" s'appliquent sur cet ensemble de base pour en retirer certains résultats.
3. Finalement, les critères "**OU**" ajoutent des fiches supplémentaires au résultat final, indépendamment des critères ET et SAUF.

> **Exemple** : Si l'on cherche les bâtiments de l'UNIL (ET), ou de l'UNIGE (OU), ne contenant pas dans le nom "bio" (SAUF), le résultat sera : les bâtiments de l'UNIL dont le nom ne contient pas "bio" (Biophore n'apparaît pas) et tous les bâtiments de l'UNIGE, même ceux contenant "bio" (Campus Biotech est bien présent dans les résultats).

![](assets/search/adv_search_ex_AND_NOT_OR.png)