
# Food Recipe App

This task is for testing some basic concepts in React JS, and to show your capabilities to work with such technology.

---

## Practice

0.  The task is to fetch a list of recipes from an external resource (API) and display them to the user depends on categories.

1.  First page will show a list of static categories. like image below.

    ```javascript
    const categories = [
      "chicken",
      "spaghetti",
      "chocolate",
      "fish",
      "rice",
      "meat",
    ];
    ```

    ![categories page](../illustrations/W12D02/recipe_app_homepage.png)

1.  When the user clicks on the recipe's category or the image, the categories page will disappear and a component containing the connected recipe list will be shown like image below

    ![recipe page](../illustrations/W12D02/list_of_recipe.png)

1.  At the end of the current list of recipes, there is a **Explore More Recipes** button that will render more recipes on screen as the image describe.

    ![explore more](../illustrations/W12D02/show_more_recipe.png)

1.  When the user clicks on the recipe's title or the image, the recipe list will disappear and a component containing the connected recipe details will be shown. Inside the recipe details component, you will be shown **details** as the image.

    ![recipe detail](../illustrations/W12D02/item_deatail.png)

1.  Additionally, you will add a **Back** button to hide the recipe details component and show the recipe list component.

1.  Add a **Home** button that will show the categories page and hide the other pages.



---

## Extra

- add new button **Add To Favorite** to the recipe details component when clicked will mark the recipe as favorite.
  > **Note**: `local storage`
- Add a button to display the list of favorite recipe from local storage,and display the recipes name and button to remove the recipes from the list.
- create a search input that will search inside the recipes array and display them to the user.

---

## Resources

- [themealdb](https://www.themealdb.com/)


  
```javascript
const URL = `https://www.themealdb.com/api/json/v1/1/search.php?s=${CATEGORY_NAME}`;
```
