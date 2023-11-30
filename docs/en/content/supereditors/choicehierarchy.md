When creating a choice, it is possible to associate a **parent** with it.
![](assets/datation/parentchoice.png)

The hierarchy of choices is visible in the **Set up** mode of the choice set. To modify the order, select the item and use the cross icon to move it to the desired location in the hierarchy. 
![](datation/hierarchie.png)

**CAUTION:** It is not recommended to create multiple levels of choice hierarchy as it can lead to confusion when searching by parent choice. During a search by choice set, children of children are not included.

**Example**
![](assets/datation/3levels.png)

- The choice 20th century
  - The choice World War II is a child of 20th century
    	- The choice year 1940 is a child of World War II

### Impact on search

Searching for objects dated in the 20th century without including children

![](assets/datation/20thnochildren.png)

> No children are included in the search results

![](assets/datation/20thresults.png)

Searching for objects dated in the 20th century including children

![](assets/datation/20thwithchildren.png)

> The first level of children is included

![](assets/datation/20thwithresult.png)

Searching for objects dated in World War II without including children

![](assets/datation/ww2nochildren.png)

> The parent choice is no longer included

![](assets/datation/ww2noresult.png)

Searching for objects dated in World War II including children

![](assets/datation/ww2withresult.png)

> The child of the child choice is included but not the parent choice

Searching for objects dated in the 20th century including children **OR** objects dated in World War II including children

![](assets/datation/20thorww2.png)

> All 3 levels are included

![](assets/datation/20thorww2result.png)

#### In summary
The hierarchy of choices in standard or date type choice sets has a significant impact on search results. The lower in the hierarchy the choices are, the harder it becomes to find them during a search by choice set.