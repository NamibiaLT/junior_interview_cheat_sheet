# Junior Tech Interview Cheat Sheet

### MVC
* Model View Controller
#### Model
* Contain the domain logic if an application, which tell you how records in database are retrieved, validated, or manipulated

#### View
* Define what the user sees in an application
* In the post page of a blog app, the view would define what the post button will look like, what the header to the post page will look like or even where the text box might be wihin the page.

### Controller
* Connects the View logic to the Model. It also defines what each element in the view will do.
* In the post page of the blog app you created, the controller will post the text once the post button is selected.

 _For a general overview check out this explanation by_ [Code Academy](https://www.codecademy.com/articles/mvc)

### Object Oriented Programming
* For the best explanation check out this [Medium Article](https://medium.freecodecamp.org/object-oriented-programming-concepts-21bb035f7260)

### Many Kinds of Variables
#### What is variable scope?
* Defines how to access a variable in a program: is the variale local, global, instance, class?


| symbols to know |	   Scope    |
|-----------------|-------------|
|        $        | global      |
|       @@        | class       |
|        @        | instance    |
| lowercase/ _    | local       |
| uppercase       | constants   |


#### Instance variable
* Global variables that can only be used within instance methods and defined with an initialize method outside of an instance method:
``` def initialize(@variable_name)
      @variable_name = variable_name
```
* [Instance Variable Resource](http://ruby-for-beginners.rubymonstas.org/writing_classes/instance_variables.html)

#### Class variable
* [Class Variable Resource](https://learn.co/lessons/ruby-class-variables-and-class-methods-readme)

#### Global variable
* Declared outside of methods, and can be manipulated by multiple methods.

#### Local variable


