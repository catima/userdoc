An item type can have content that is common to all items (e.g. all movies have a director) but can also have conditional content (e.g. the "Period" field is relevant for *historical documentaries* but not for *action movies*). It is possible to create a **category** that is displayed only if a certain **choice** is selected. In our example, the option *Period* can be shown to the editor creating a new item only if the choice *Historical documentaries* is displayed and otherwise hidden.
This allows the *New item* page to remain uncluttered.  

Follow the next steps to create conditional content:  

### 1. Add a category

On the *Setup* page click on **Category > New category** in the left sidebar. It is possible to create multiple categories that are linked to different choices.  
The process of creating a new category is the same as creating a new item: chose a name and slug then add new fields.

### 2. Link it to a choice

In the left sidebar, select **Choices** and edit ![Edit button](assets/buttons/edit_btn.png) the choice set containing the choice that you want linked to the conditional content. In this example we will add conditional content to the choice *Other* in the first choice set.

![Choice set page](assets/choice/a-choice-set-page.png)

Edit the choice and the last option is to add conditional content; select the category that should be displayed when that choice is selected:

![add a category](assets/categories/a-add-category.png)

After updating the choice, the conditional content is displayed on the right side of the choice when editing the choice set:

![conditional choice set](assets/categories/a-conditional-choiceset.png)
