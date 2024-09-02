# A Completed Task Manager

This rails app is meant to suplement the [Task Manager](https://github.com/turingschool-examples/task_manager_rails/blob/master/README.md) tutorial.  If you have not already started that tutorial, please do that before diving in to this repo - much of the file structure will not make sense if this is your first time looking at a Rails app!

## Setup

To get this repository cloned down and set up locally:

```
$ git clone git@github.com:turingschool-examples/task-manager-7-complete.git
$ cd task-manager-7-complete
$ bundle install
$ rails db:{drop,create,migrate}
```

## Running Locally

After completing the setup, you can now start your server with `$ rails s` and navigate to [http://localhost:3000/](http://localhost:3000/).

## Checks for Understanding
1. Define CRUD. Create, Read, Update, Delete.  This is the work flow for operating and dynamically updating, managing and maintaining databases.
2. Define MVC. Model-View-Controller. The back-end creates and maintains the Model. The Model contains the functionality, logic and manages the data. The View is what the user sees(UI) and interacts with(e.g a webpage). The Controller acts as a bridge between the Model and View.  Having these three seperate things working together to create an application or page that a user is able to interact with.
3. What three files would you need to create/modify for a Rails application to respond to a GET request to /tasks, assuming you have a Task model. config/routes.rb, app/controllers/tasks_controller.rb, and the models/task.rb.
4. What are params? Where do they come from? Params(or parameters) are the values passed to the methods in the tasks_controller.rb file.  In web development, they can come from end-uer interations, like filling out a form or entering data that the back-end will then take in and manipulate a result object.
5. Check out your routes. Why do we need two routes each for creating a new Task and editing an existing Task? Each route serves a purpose to generate a response based on user input. The user input will, behind the scenes, get/post/patch/or delete data based off of methods defined in the tasks_controller file.
