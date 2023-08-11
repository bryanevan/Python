# Table of Contents
# Achievement 1

1. [Exercise 1](#exercise-1)
2. [Exercise 2](#exercise-2)
3. [Exercise 3](#exercise-3)

# Exercise 1

## Table of Contents

1. [Install Python](#install-python)
2. [Set Up a Virtual Environment](#set-up-a-virtual-environment)
3. [Create a Python Script](#create-a-python-script)
4. [Set Up IPython Shell](#set-up-ipython-shell)
5. [Export a Requirements File](#export-a-requirements-file)

## Install Python

First, install Python 3.8.7 on your system. Check your Python version by using the command `python --version` from your terminal.

![Step 1](./exercise_1.1/step1.png)

## Set Up a Virtual Environment

Set up a new virtual environment named “cf-python-base”.

![Step 2](./exercise_1.1/step2.png)

## Create a Python Script

Install Visual Studio Code or another text editor of your choice and create a Python script named “add.py”. This script will take two numbers from the user input, add them, and print the result. Here's the template for your Python script:

![Step 3](./exercise_1.1/step3.png)

```python****
# Prompt the user to enter the first number
a = int(input("Enter the first number: "))

# Prompt the user to enter the second number
b = int(input("Enter the second number: "))

# Add the two numbers and store the result in variable c
c = a + b

# Print the value of c
print("The sum of", a, "and", b, "is:", c)
```

## Set Up IPython Shell

Set up an IPython shell in the virtual environment "cf-python-base". An IPython shell is similar to the regular Python REPL with additional features like syntax highlighting, auto-indentation, and robust auto-complete features. Install it using pip.

![Step 4](./exercise_1.1/step4.png)

## Export a Requirements File

Generate a “requirements.txt” file from your source environment. Next, create a new environment called “cf-python-copy”. In this new environment, install packages from the “requirements.txt” file.

![Step 5](./exercise_1.1/step5.png)

# Exercise 2

## Table of Contents

1. [Create the Data Structure](#create-the-data-structure)
2. [Create recipe_1](#create-recipe_1)
3. [Create Outer Structure](#create-outer-structure)
4. [Create 4 More Recipes](#create-4-more-recipes)
5. [Print Ingredient Lists](#print-ingredient-lists)

6. ## Create the Data Structure

  - Create a structure named recipe_1 that contains the following keys:
  - name (str): Contains the name of the recipe
  - cooking_time (int): Contains the cooking time in minutes
  - ingredients (list): Contains a number of ingredients, each of the str data type

![step 1](./exercise_1.2/step1.png)

_A dictionary is suitable because it provides a key-value structure to associate recipe attributes. It allows easy access to specific information using keys. Dictionaries support different data types, accommodating strings, integers, and lists for recipe name, cooking time, and ingredients, respectively. The structure maintains organization and consistency, particularly useful when storing multiple recipes in a container like a list. Overall, using a dictionary facilitates convenient manipulation and structured access to recipe data, enabling further operations and analysis._

## Create recipe_1

![step 2](./exercise_1.2/step2.png)

## Create outer Structure

Create an outer structure called all_recipes, and then add recipe_1 to it.

![step 3](./exercise_1.2/step3.png)

_Using a list provides a sequential and dynamic structure, allowing easy modification and retrieval of recipes based on their order. Lists support iteration and indexing, enabling convenient operations on individual recipes or the entire collection. The versatility of lists accommodates recipes of varying lengths and complexities, making it suitable for a diverse range of recipe structures. Overall, a list provides the flexibility, scalability, and ease of access required for managing and modifying multiple recipes._

## Create 4 More Recipes

Generate 4 more recipes as recipe_2, recipe_3, recipe_4, and recipe_5, and then add them as well to all_recipes.

![step 4](./exercise_1.2/step4.png)

## Print Ingredient Lists

Print the ingredients of each recipe as five different lists, inside the IPython shell.

![step 5](./exercise_1.2/step5.png)

# Exercise 3

## Table of Contents

1. [Create a New Python Script](#create-a-new-python-script)
2. [Initialize Two Empty Lists](#initialize-two-empty-lists)
3. [Define a Function](#define-a-function)
4. [Get The Number of New Recipes](#get-the-number-of-new-recipes)
5. [Check Ingredients and Add Recipes](#check-ingredients-and-add-recipes)
6. [Assign Difficulty Levels and Display Recipes](#assign-difficulty-levles-and-display-recipes)
7. [Display All Ingredients](#display-all-ingredients)

## Create a New Python Script
## Initialize Two Empty Lists

Open a Python script in an editor of your choice and name it “Exercise_1.3.py”.
Initialize two empty lists: recipes_list and ingredients_list.
![step 1](./exercise_1.3/step1&2.png)

## Define a Function

Define a function called `take_recipe`, which takes input from the user for the following variables:

- `name` (str): Stores the name of the recipe.
- `cooking_time` (int): Stores the cooking time (in minutes).
- `ingredients` (list): A list that stores ingredients, each of the string data type.
- `recipe` (dictionary): Stores the `name`, `cooking_time`, and `ingredients` variables (e.g., `recipe = {'name': name, 'cooking_time': cooking_time, 'ingredients': ingredients}`).

![step 3](./exercise_1.3/step3.png)

## Get the Number of New Recipes

Ask the user how many recipes they would like to enter. Their response will be linked to a variable n.

![step 4](./exercise_1.3/step4.png)

## Check Ingredients and Add Recipes

Run a for loop, which runs n times to perform the following steps:

- Run `take_recipe()` and store its return output (a dictionary) in a variable called **recipe**.
- Run another for loop inside this loop, which iterates through recipe’s ingredients list, where it picks out elements one-by-one as ingredient. It will run the following step inside: if the chosen ingredient isn’t present in ingredients_list, add it to this list.
- Once finished adding ingredients, append recipe to recipes_list.

![step 5](./exercise_1.3/step5.png)

## Assign Difficulty Levels and Display Recipes

Run another for loop that iterates through the recipes_list and assign a difficulty level based on the following criteria:

- If cooking_time is less than 10 minutes, and the number of ingredients is less than 4, set a variable called difficulty to the value of **Easy**.
- If cooking_time is less than 10 minutes, and the number of ingredients is greater than or equal to 4, set a variable called difficulty to the value of **Medium**.
- If cooking_time is greater than or equal to 10 minutes, and the number of ingredients is less than 4, set a variable called difficulty to the value of **Intermediate**.
- If cooking_time is greater than or equal to 10 minutes, and the number of ingredients is greater than or equal to 4, set a variable called difficulty to the value of **Hard**.

Display each recipe in the following format:

- Recipe:
- Cooking Time (min):
- Ingredients:
- Difficulty level:

![step 6](./exercise_1.3/step6.png)

## Display All Ingredients

Display all the ingredients that you’ve come across so far in all of the recipes that you’ve entered.

![step 7](./exercise_1.3/step7.png)
