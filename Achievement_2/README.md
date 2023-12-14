# Table of Contents

# Achievement 2

1. [Exercise 1](#exercise-1)
2. [Exercise 2](#exercise-2)
3. [Exercise 3](#exercise-3)
4. [Exercise 4](#exercise-4)
5. [Exercise 5](#exercise-5)
6. [Exercise 6](#exercise-6)
7. [Exercise 7](#exercise-7)

# Exercise 1

## Table of Contents

1. [Check Python Version](#check-python-version)
2. [Set Up a Virtual Environment](#set-up-a-virtual-environment)
3. [Install Django](#install-django)

## Check Python Version

Run command python3 -V to check for version 3.8.0

![Step_1](./exercise_2.1/step1.png)

## Set Up a Virtual Environment

Create a new virtualenvironment called achievement2-practice. Confirm it's active in the terminal.

![Step_2](./exercise_2.1/step2.png)

## Install Django

While in virtual environment achievement1-practice, pip install django and check version after install.

![Step_3](./exercise_2.1/step3.png)

# Exercise 2

1. [Create A2_Recipe_App Folder](#create-a2_recipe_app-folder)
2. [Create a2-ve-recipeapp Virtual Environment](#Create-a2-ve-recipeapp-virtual-environment)
3. [Install Django in Virtual Environment](#install-django-in-virtual-environment)
4. [Create Django Project Named recipe_project](#create-django-project-named-recipe_project)
5. [Rename recipe_project Project Directory src](#rename-recipe_project-project-directory-src)
6. [Run Migrations and Run Rerver](#run-migrations-and-run-sever)
7. [Create SuperUser and Sign In](#create-superuser-and-sign-in)

## Create A2_Recipe_App Folder

![Step_1](exercise_2.2/screenshots/step1.png)

## Create a2-ve-recipeapp Virtual Environment

![Step_2](exercise_2.2/screenshots/step2.png)

## Install Django in Virtual Environment

![Step_3](exercise_2.2/screenshots/step3.png)

## Create Django Project Named recipe_project

![Step_4](exercise_2.2/screenshots/proj_contents_before_renaming.jpg)

## Rename recipe_project Project Directory src

![Step_5](exercise_2.2/screenshots/proj_contents_after_renaming.jpg)

## Run Migrations and Run Rerver

![Step_6_1](exercise_2.2/screenshots/step6p1.png)
![Step_6_2](exercise_2.2/screenshots/step6p2.png)

## Create SuperUser and Sign In

![Step7](exercise_2.2/screenshots/admin-dashboard.jpg)

# Exercise 3

## Table of Contents

1. [Create App Schema](#create-app-schema)
2. [Establish Project Structure](#establish-project-structure)
3. [Migrate Models](#migrate-models)
4. [Test Models](#test-models)

## Create App Schema

Identify the desired attributes of each entity and their relation with other entities.

![Step_1](./exercise_2.3/screenshots/schema.jpg)

## Establish Project Structure

Create the apps drawn out in the schema and include links to projects in settings.py

![Step_2](./exercise_2.3/screenshots/project-structure.jpg)

## Migrate Models

After building models within each app, register the models in their respective admin.py, then migrate.

![Step_3](./exercise_2.3/screenshots/run-migrations.jpg)

## Test Models

Build tests for all apps, respectively; run tests.

![Step_4](./exercise_2.3/screenshots/Test-Report.jpg)

# Exercise 4

## Table of Contents

1. [Create Welcome Page](#creat-welcome-page)

## Create Welcome Page

Modify URLs to send user a welcome page with a basic outline.

![Step_1](./exercise_2.4/src/screenshots/welcome.jpg)

# Exercise 5

## Table of Contents

1. [Update Models](#update-models)
2. [Add Records](#add-records)
3. [Welcome Page](#welcome-page)
4. [Recipe Details](#recipe-details)
5. [Test](#test)

## Update Models

Update neccessary models.py to facilitate url paths.
Update neccessary url.py for path logic.
Update neccessary views.py for path and view logic.

makemigrations, migrate, runserver

## Add Records

Download food images to a new media/recipes directory.
Go into admin panel to update recipes with corresponding images.

## Welcome Page

Create Static directory, set up static routing is settings.py.

Update welcome page for better UI/UX, add a button to route to recipe list view with recipes_list.html template.

## Recipe Details

Create recipes_details.html to display recipe details.

## Test

Test all links and ensure they pass.

# Exercise 6

## Table of Contents

1. [Provide Authentication](#provide-authentication)
2. [Protect Views](#protect-views)
3. [Implement Logout](#implement-logout)
4. [Run Server and Capture Output](#run-server-and-capture-output)

## Provide authentication

Create a login feature for your application. The login page should be accessible from your homepage via the link directly at “http://127.0.0.1:8000/login/”. To achieve this, you need to:
Create a login view.
Create a login template.
Register a view and map URL.
Provide a clickable login link or button on the homepage that routes to the authentication form.
Identify which page you want to protect via authentication and redirect the user to that page after a successful login.

## Protect Views

Identify which views or pages you want to protect via authentication. Then go ahead and add the necessary code at all relevant views to ensure that the page isn’t called if the user isn’t logged in. Access the URLs of the protected views in your browser and make sure that you’re redirected to the login page.

## Implement Logout

Provide a logout link or button on each protected page.
Create a new view and template for your application with the message “You’ve successfully logged out.” Call this success.html.
Provide a link to log back in to success.html.
Create the view and template for logging out.
What other information or feature do you want to place on the success.html page? Go ahead and add it to the template. Be creative!

## Run Server and Capture Output:

Toggle the terminal ON in VSCode and follow the steps to run the server:
Navigate to A2_Recipe_App/src.
Activate the virtual environment: a2-ve-recipeapp.
Execute runserver.
Head to the browser and follow a typical user journey:
User lands at homepage.
User clicks login button.
Authentication form is shown.
User enters username and password.
Information is authenticated and user is redirected to sales page.
User logs out and returns to successful logout page.

# Exercise 7

## Table of Contents

1. [Implement Search For Recipes](#implement-search-for-recipes)
2. [Data Visualization](#data-visualization)
3. [Write Tests](#write-tests)
4. [Run Server and Capture Output](#run-server-and-capture-output)

## Implement Search for Recipes

    - Take some time to think of what you want users to search for, the criterion for search, and format of output. Create a new empty document and call it “Task-2.7”. Place your thoughts in this document. Save the document.
    - Create a user form to allow your user to input the search criteria.
    - Extract the data as QuerySet using the search criteria.
    - Convert the QuerySet to pandas DataFrames (Ensure you have pandas installed).
    - Display search results as a table.
    - Ensure that the recipes returned by the search criteria are clickable and lead to the details page of the recipe.
    - Bonus: Allow users to search on the basis of wild cards and partial search queries. For example, in the Bookstore application, this will mean that searching for “Pride and” will also return “Pride and Prejudice” book results.

## Data Visualization

    - In your “task-2.7” document, add a new heading named “Data Analysis”, and note down at least one visualization using a bar, pie, and line chart (at least one for each). For each of the scenarios, identify the x- and y- axes and labels (if any). Also determine if you want charts to be displayed based on user input or simply to provide them at your own discretion.
    - Head to VSCode and ensure that you have matplotlib installed.
    - Implement the charts that you shortlisted in 3a.

## Write Tests

    - Follow the same testing process (that you previously used for models and views) to test your new forms and views. For this, you can create classes like `RecipeFormTest`. Testing will need to include checking the fields for values, formats, or lengths, ensuring login protection of views, appropriate pagination, and any other checks you feel are relevant. As specified earlier, for smaller projects all your tests can be placed in the same file, but feel free to create separate files for each of them if you prefer. In each case, you’ll need to import the form or view that you want to test, create a class, specify the `setUp` and `setUpTestData` methods, and write tests.
    - Run the tests with verbosity set to 2, and take a screenshot of the outcome in the terminal. Save the screenshot as “test-outcome.jpg”, or similar.

## Run Server and Capture Output:

    - Open “Task-2.7” and add a heading called “Execution flow”.
    - Think of the user’s journey from the moment they land on the homepage, considering all the different navigation possibilities and search options. For example, a user lands on the homepage, logs in to the account, searches for a recipe based on a recent date, sees the plots, checks details, and then logs out. Represent this journey as a flow chart.
    - Toggle the terminal ON in VSCode and do the following to run the server: Navigate to `A2_Recipe_App/src`, activate the virtual environment (`a2-ve-recipeapp`), and execute the `runserver` command.
    - Head to the browser, and follow the user journey noted in 5b. At each step, note the URL and take a screenshot. Paste the screenshots in the “Task-2.7” document. Alternatively, you can create a screencast recording the journey using your favourite screen-recording tool. Save it by the name “user-journey.mp4” (or any other movie extension of your choice).
