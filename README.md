#Sinatra Todos
A todo list application built using Sinatra and Puma with data persisting to a Postgres database.

##Installation
Prerequisites: Make sure to have Ruby and PostgreSQL installed

From the RB185-sinatra-todos directory:

1. Install all Ruby gem dependencies: run "bundle install" in the shell.
2. Create the todos database: run "createdb todos" in the shell.
3. Upload the database schema: run "psql -d todos < schema.sql" in the shell to upload the schema from "schema.sql" file into the "todos" database.
4. Start the application: run "ruby todo.rb" in the shell. By default the application will run on port 4567.

##Usage
###Creating a New List

1. Navigate to the home page of the application.
2. Click the "New List" button.
3. Enter the desired name for your new list and confirm to create it.

###Viewing and Managing Tasks in a List

1. On the home page, click on the list you want to manage. This will display all tasks related to that list.
2. To add a new task, use the provided input field and submit your task.
3. To mark a task as complete, click on the specific todo item.
4. To delete a task, use the delete option next to the todo item.
5. To mark all tasks as done, click the "Complete All" button.

###Navigating Between Lists

1. To return to the home page and view all lists, click the "All Lists" button.
2. On the lists page, you can see the number of completed tasks and the total number of tasks for each list.

###Editing a List

1. While viewing a list, click the "Edit List" button.
2. From the edit page, you can either delete the list or change its name.

##Features

- User-Friendly Interface: Easily create and manag e multiple todo lists.
- Task Management: Add, complete, delete, and bulk complete tasks within any list.
- List Overview: Quickly see progress with a summary of completed vs. total tasks for each list.
- Edit Capabilities: Modify list names or delete lists as needed.
- Persistent Data: All data is stored in a PostgreSQL database, ensuring your lists and tasks are saved between sessions.
