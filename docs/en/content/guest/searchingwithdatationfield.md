#### Reminder: differences between "date" and "datation" fields

The **Date** field allows the entry of a specific date on a record. This date must be unique. For example, it could be a person's birthdate, a building's construction year, or the date and time of a performance.

The **Datation Field** accepts a start date and an end date, allowing the creation of periods and searching for all dates within that period.

> The datation field is a very complex field for which [a complete manual](assets/datation/exampledatation.pdf) has been produced, as well as an [example catalog](https://catima.unil.ch/datation-exple/en) showing how the field is used and how it behaves when searched.

### Using the simple search to search by dates

Entering a date in the search bar will only retrieve items that contain that exact date as entered in the date field. It will not calculate or understand periods (eg. between date 1 and date 2). 

>Notice: entering two dates in the search bar won't calculate a period but will return items in which both dates are textually present.

### Searching dates with the advanced search

The advanced search is the optimal way to perform searches by dates (searching both 'date' and 'datation' fields) and allows to specify a period in various ways.

Thanks to the dropdown lists available for date/datation fields, periods of time can be specified very precisely as detailed below.

![Advanced search](assets/datation/advancedsearch.png)

Dropdowns on the right allow to specify whether the search should retrieve results:
- for an exact date (1), 
- after a date (2), 
- or before a date (3).

### Options available for the field "date" 

In this case, options such as "between the dates" and "outside the dates" will also be available in the dropdown. 

### Options available when the date is a “Datation” field

The dropdown (4) enables searches through a choice set.

The ***Exclude*** criterion (5) allows excluding one or the other of the datation format. Excluding records with **manual datation** will only return records with **choice set datation** and vice versa.

Criteria located on the left can be combined using the search operators "and" (6), "or" (7) and "exclude" (8).


> **Reminder:**
>
> **AND** (6): all criteria must be met
>
> **OR** (7): one criteria at least must be met
>
> **EXCLUDE** (8): contents with the provided date must be excluded from the list of search results
