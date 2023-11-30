> The datation field is a very complex field for which [a complete manual](assets/datation/exampledatation.pdf) has been produced, as well as an [example catalog](https://catima.unil.ch/datation-exple/en) showing how the field is used and how it behaves when searched.

The datation field is a field that allows for **flexible datation** of an item. It differentiates itself from the date/time field by offering the ability to consider periods in addition to specific dates.

Subsequently searches by date can be performed based on predefined periods, user-defined periods, or based on a specific date.

This field accepts two types of formats for entering dates when creating new items:

- Manual entry by date/time: for each added item, manually enter the start and/or the end of a period.
- Entry through a choice set: Select a choice from a predefined choice set when creating the item.

> Both options can be offered for the same item type. It is then possible to choose between a predefined period or to create one manually when entering a new record. **However, it's not possible to enter both formats in the same item.**

#### Manual Entry

With manual datation, there are several input possibilities:

- The *Start Date* and *End Date* fields are filled with two different dates. They define a period from one date to another, including all dates between them.
- The *Start Date* and *End Date* fields are filled with the same information. They define a fixed date. For example, *Start Date*: 1990 and *End Date*: 1990.
- Only the *Start Date* field is filled. It defines a period after the indicated start date (included).
- Only the *End Date* field is filled. It defines a period before the indicated end date (included).

![](assets/datation/manualentry.png)

> Start and end dates are **inclusive**. A period defined with a start date of **1990** and an end date of **1999** includes the years 1990, 1991, 1992, 1993, 1994, 1995, 1996, 1997, 1998, and 1999. Searching for any of these years will return records from this period.

#### Through a Choice Set

Select one or more choices from the dropdown list. datation through a choice set allows assigning one or more different periods to the same record.

![](assets/datation/choiceentry.png)
