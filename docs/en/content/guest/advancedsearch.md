The advanced search is for searching within **elements of a specific item**. To access the advanced search page, click on the *Advanced* link on the right side of the search button; you will be redirected to a new page.

> Note: all examples in this help section are from catalog [DEMO - Universités et bibliothèques](ttps://catima.unil.ch/catmanual2/fr), which is openly accessible to all.

![Advanced search - item types](assets/search/g-search1.png)

By default, the item searched is the first one in alphabetical order. This can be changed by clicking on *Default search by item type* and choosing a different item. Then each field can be searched using a keyword or exact wording. It is also possible to filter elements by name or category.

### Boolean operators

It is possible to use advanced search with boolean operators:

- Operator "**AND**" (default) is used to combine search words and narrow results. This tells the database that *all* search terms must be present in the results.  
- Operator "**OR**"; two search terms linked with **OR** will return all results that match with either one or the other
- Operator "**EXCLUDE**" is used to excludes results that match a given term.  

#### Examples

> To display all buldings from the University of Lausanne that have "Amphi" in their name:

![Operator AND](assets/search/g-search_and.png)

> To display the list of all buildings from the University of Lausanne and from the University of Geneva:

![Operator OR](assets/search/g-search_or.png)

> To display the list of the buildings from the University of Lausanne, except the ones that have "*nef*" in their name:

![Operator EXCLUDE](assets/search/g-search_exclude.png)


**Utilisation combinée des opérateurs "ET", "SAUF" et "OU"**

You can use all three operators in one search. The order in which criteria show has no impact on search results. Only the type of operator is relevant to determine how each criteria is applied. In the end, the following rules apply in the bewlow specific order:
1. First "**AND**" criteria determine the base result list
2. Then, "**EXCLUDE**" criteria filter out some results of that base list
3. Finally, "**OR**" criteria apply and additional results are added to the base result list, noting that the "**EXCLUDE**" criteria is not relevant at this stage.

> **Example** : if you are looking for all buildings of UNIL (AND) or those of UNIGE (OR) which do not contain the term 'bio' in their name (EXCLUDE), the result will be the following, and not the one you would intuitively expect : results will include all UNIL buildings which name does not contain "bio" (Biophore will not show in the results) and all UNIGE buildings, even those which contain "bio" (campus Biotech will thus show in the results).

![Operators AND OR EXCLUDE](assets/search/adv_search_ex_AND_NOT_OR.png)