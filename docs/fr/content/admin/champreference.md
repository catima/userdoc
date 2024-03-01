Ce champ permet de créer une référence à un autre type de fiche.  

**Exemple:**  
Pour lier les *Bâtiments* aux *Universités*, créer un champ référence dans la fiche bâtiments. Lors de la saisie des données d'un bâtiment, il faudra donc choisir une université à laquelle il est lié. 

Lors de la consultation des fiches, l'université référencée apparaît de la même manière que les autres champs dans la fiche du bâtiment. 

![Fiche annexe Mouline](assets/setup/reference_mouline.png)

Les fiches *Bâtiments* qui font référence à une univeristé sont listé en bas de la fiche Université en question. Ci-dessous la fiche de l'université de Lausanne avec liste des fiches *Bâtiments* qui lui font référence:

![Fiche université de Lausanne - références](assets/setup/fiche_uni_reference.png)

> Si plusieurs types de fiches font référence à une autre fiche -comme ici *Bâtiments* et *Bibliothèques* ont les deux un champ référence à la fiche *Universités*, les fiches qui lui font référence sont listées par type de fiche.