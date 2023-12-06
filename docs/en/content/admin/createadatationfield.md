Several questions need to be addressed before starting to create a **datation** field.

1. What is the level of precision: by period, by year, by day/month/year?
2. Are the dates/periods exclusively AD (Anno Domini), or are dates/periods BC (Before Christ) also possible?
3. What input methods should be offered?
    - Manual input by date/time only (skip directly to step 2 to create the datation field)
    - Selection from a predefined set of choices (start with step 1 to configure a datation choice set before creating the datation field itself)
    - Both options (start with step 1 to configure a datation choice set)

> Field modifications are possible later on but may lead to the loss of certain data.

#### Step 1: Creating a datation choice set

This step is necessary for choosing dates through a predefined set of choices and must be done prior to creating the datation field.

In **Setup** mode, select **Choice set** from the left column and click on *+ New Choice set*. Choose the *datation* type, decide whether dates before BC are allowed or not, and select the format.

*The format and the choice set type (Date or Standard) cannot be modified once the choice set is created.*

> It's recommended to choose the widest possible format. For a datation by century, choose **Y** (years) only instead of a finer format that includes months and days, as it can lead to conflicts during searches. If date/day/month/year precision is required, choose **YMD** and do not include hours and seconds.

![](assets/datation/allowBC.png)

Edit the newly created choice set and click on *+ New Choice* to add a new period or specific date. There are several possibilities:

- The *Start Date* and *End Date* fields are filled with two different dates. They define a period from one date to another, including all dates between them.
- Only the *Start Date* field is filled. It defines a period after the indicated start date (included).
- Only the *End Date* field is filled. It defines a period before the indicated end date (included).
- Filling both fields with the same information sets a fixed date. For example, *Start Date*: 1990 and *End Date*: 1990.

![](assets/datation/bcornot.png)

> Start and end dates are **inclusive**. A period defined with a start date of **1990** and an end date of **1999** includes the years 1990, 1991, 1992, 1993, 1994, 1995, 1996, 1997, 1998, and 1999. Searching for any of these years will return records from this period.

<a id="hierarchy-choice"></a>
##### Choice hierarchy

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

###### Impact on search

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

##### In summary
The hierarchy of choices in standard or datation choice sets has a significant impact on search results. The lower in the hierarchy the choices are, the harder it becomes to find them during a search by choice set.

#### Step 2: Creating the datation field

In **Set Up** mode, select the record type from the left column and click on *+ Add > Datation Field*. In addition to the name, plural name, and slug, along with display options, the last parameter defines the format(s) used for data entry:

1. **Manual**: Check this box to allow manual entry of dates and periods. The data format is defined by selecting an option from the dropdown menu. *To enable the use of dates before BC, check the box below the dropdown menu*.
2. **Through a choice set**: Check this box and select a choice set **of date type** to allow the selection of dates or periods based on a previously created choice set. The acceptance or rejection of negative dates is defined directly in the choice set settings under *Set Up > Choice Set*.

**CAUTION!** If both input types are enabled (manual and through a choice set), it is recommended to choose the same date format.
Otherwise, ensure that you have defined **consistent** formats. The widest date format should always be included in the finer format. For example, if the choice set is in years, manual input could be in month-years format but not exclusively in months.

![](assets/datation/config_datation.png)