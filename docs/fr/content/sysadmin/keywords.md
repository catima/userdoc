
Un-e administrateur-ice système a la possibilité d'ajouter des mots-clés pour qualifier des groupes de catalogues spécifiques. 

Voir des exemples ci-dessous:
1. Un catalogue CATIMA peut avoir plusieurs mots-clés qui s'affichent dans la colonne ***Keywords***
2. le *crayon* permet d'éditer le catalogue et d'ajouter un mot-clé (voir ci-après)
3. Il est possible avec ***CMD + F** d'identifier tous les catalogues de la section HART (exemple ci-dessous) 
4. et d'avoir le nombre d'occurence des catalogues HART (exemple ci-dessous)).

![](assets/admin/admin-list-keyword-hart.png)

**Ajouter un mot clé**

Comme indiqué en (2) ci-dessus, cliquer sur le **Menu édition** correspondant.

Dans la page d'édition du catalogue, ajouter les mots-clés dans le champ **'comments'**.

Les mots-clés doivent suivre toutes ces **régles de formatage** pour être interprétés comme mot-clé:
- commencer par #
- ne contenir que des lettres, en minuscule, en masjucules ou le caractère _ (*underscore*)
- ne pas contenir d'espace entre les mots

![](assets/admin/admin_catalog_add_kwd.png)

**Utilité des mots clés**

Les mots-clés peuvent servir plusieurs objectifs, par exemple:
- identifier la section à laquelle le catalogue est affilié (*ISH, HART, FRA*, etc...)
- identifier les catalogues utiles dans le cadre de: *DEMO* , *TEST* ou *SIER*
- identifie une action à entreprendre, avec un mot clé de type *supprimer*


| Mots-clés                      | Formatage             | Signification                                        |
|--------------------------------|-----------------------|------------------------------------------------------|
| ISH , FRA , HART , ...         | #ISH, #FRA , #HART ...| catalogue lié à la section ISH, FRA ou HART (etc....)|
| DEMO                           | #DEMO                 | catalogue de DEMO, pour valoriser les usages         |
| TEST                           | #TEST                 | catalogue de test, validitée potentiellement limitée |
| SIER                           | #SIER                 | catalogue du SIER                                    |
| voir_si_supprimer              | #voir_si_supprimer    | catalogue à *peut-être* supprimer(selon analyse)     |
| Supprimer                      | #Supprimer            | catalogue à supprimer                                |
| Supprimer_apres_tests          | #Supprimer_apres_tests| catalogue à supprimer (après les tests)              |

**Catalogues à supprimer**

les catalogues identifiés comme étant *à supprimer* ne doivent pas être supprimés de suite, mais seront préalablement désactivés pour une durée à déterminer (par exemple 6 mois). 

Le moment adéquat pour désactiver un catalogue est determiné par :
- une discussion avec le *propriétaire* si possible, ou une analyse plus poussée confirme l'obsolescence du catalogue pour l'UNIL 
- les tests pours lesquels le catalogue a été construits sont terminés