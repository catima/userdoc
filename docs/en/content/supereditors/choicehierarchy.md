When creating a choice, it is possible to associate a **parent** with it.
![Parent choice](assets/datation/parentchoice.png)

The hierarchy of choices is visible in the **Set up** mode of the choice set. To modify the order, select the item and use the cross icon to move it to the desired location in the hierarchy.
![Hierarchy of choices](datation/hierarchie.png)

**CAUTION:** It is not recommended to create multiple levels of choice hierarchy as it can lead to confusion when searching by parent choice. During a search by choice set, children of children are not included.

**Example**
![3 levels of choices](assets/datation/3levels.png)

- The choice 20th century
  - The choice World War II is a child of 20th century
    - The choice year 1940 is a child of World War II

### Impact on search

Searching for objects dated in the 20th century without including children

![20th century without children](assets/datation/20thnochildren.png)

> No children are included in the search results

![Search results](assets/datation/20thresults.png)

Searching for objects dated in the 20th century including children

![20th century with children](assets/datation/20thwithchildren.png)

> The first level of children is included

![Search results](assets/datation/20thwithresult.png)

Searching for objects dated in World War II without including children

![WW2 without children](assets/datation/ww2nochildren.png)

> The parent choice is no longer included

![Search results](assets/datation/ww2noresult.png)

Searching for objects dated in World War II including children

![WWW2 with children search results](assets/datation/ww2withresult.png)

> The child of the child choice is included but not the parent choice

Searching for objects dated in the 20th century including children **OR** objects dated in World War II including children

![Search 20th century or world war 2](assets/datation/20thorww2.png)

> All 3 levels are included

![Search results](assets/datation/20thorww2result.png)

#### In summary

The hierarchy of choices in standard or date type choice sets has a significant impact on search results. The lower in the hierarchy the choices are, the harder it becomes to find them during a search by choice set.
