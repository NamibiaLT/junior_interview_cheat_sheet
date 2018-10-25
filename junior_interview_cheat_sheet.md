# Junior Tech Interview Cheat Sheet

### MVC
* Model View Controller
#### Model
* Contain the domain logic if an application, which tell you how records in database are retrieved, validated, or manipulated

#### View
* Define what the user sees in an application
* In the post page of a blog app, the view would define what the post button will look like, what the header to the post page will look like or even where the text box might be wihin the page.

#### Controller
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

### APIs:
#### What is an API:
* An interface that allows developers to interact with data, and one piece of software to interact with another piece of software
* Stands for Application Programming Interface

#### What are types of APIs

##### REST APIs
* Important Terms:

      __Resource__: an object representation of something, that can have methods to act on that objects (e.g. a Post resource can have a ".add" method act on it).

      __Collections__: Sets of resources (e.g. Blogs is a collection of Blog resources).

      __URL__: A path that locates a resource and enables actions to be performed on the resource. URLS should only contain resources, rather than actions (_methods_) or verbs (_HTTP methods_)

* What is an API endpoint?

      * When you have a link, the portion of the url after the first slash: www.something.com/ would be the endpoint. Think of it as an address, or "path", that leads you to the resources you are looking for.
      * The path should always contain the plural of the resources and the HTTP method will tell you the action performed on a resource.

* What is an HTTP method?

      * _Important_: These are sometimes referred to as `verbs`.

      * HTTP methods, or verbs, indicate what action will be performed on a resource. The main for RESTful APIs are:

HTTP Method | CRUD | Collection (ex: /users) | Specific resource (ex: users/123)
--- | --- | --- | ---
POST | Create | 201 (Created), ‘Location’ header with link to /users/{id} containing new ID.| Avoid using POST on single resource
GET | Read | 200 (OK), list of users. Use pagination, sorting and filtering to navigate big lists. | 200 (OK), single user. 404 (Not Found), if ID not found or invalid.
PUT | Update/replace | 404 (Not Found), unless you want to update every resource in the entire collection of resource. | 200 (OK) or 204 (No Content). Use 404 (Not Found), if ID not found or invalid.
PATCH | Partial Update/Modify | 404 (Not Found), unless you want to modify the collection itself. | 200 (OK) or 204 (No Content). Use 404 (Not Found), if ID not found or invalid.
DELETE | Delete | 404 (Not Found), unless you want to delete the whole collection — use with caution. | 200 (OK). 404 (Not Found), if ID not found or invalid.
##### Taken from [restfulapi.net](https://restfulapi.net/http-methods/), see webpage for a full explanation.



* How do Resources and URLs work together?
      * Resources are always plural in an API endpoint (e.g. Posts).
      * To access one instance of a resource, you just need topass an ID to the URL.

##### XML-RPC APIs
##### JSON-RPC APIs
##### SOAP APIs



## Practice Problem Resources:
#### Math + Coding resource: [Project Euler](https://projecteuler.net/archives)
