## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb. 
  Post- used to send data to the server (Create in CRUD)
  Get- used to retrieve information from a given server (Read in CRUD)
  Put- used to replace the current version of the data in the server (Update in CRUD)
  Patch- modifies the data on the server (Update in CRUD) 
  Delete- deletes the data from the server (Delete in CRUD)
2. What is Sinatra? 
  Sinatra is a DSL (Domain Specific Language) used as a web application framework.
4. What is MVC?
  Model View Controller. or the convention of how you set up a web application.
5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
  Makes it easier for others to read and understand.
6. What types of variables are accessible in our view templates without explicitly passing them?
  instance variables
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  get '/horses' do
    @count = 1
    erb :index
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed`?
   ```ruby
  get '/horses' do
    name = "Mr Ed"
    erb :index, :name
  end
  ```
9. What's the purpose of ERB?
  allows you to use ruby and show results of ruby methods in an html format.
10. Why do I need a development AND test database?
  So you can make changes to one database to test functionality and design before implementing it in the one one people will be using.
11. What's responsive design?
  designing a webpage to be responsive to the size of the screen that you are viewing a site on
12. What is CRUD and why is it important?
  CRUD stands for Create Read Update and Delete, the purpose of this is to signify the basic functionality that a 
13. What does HTTP stand for? 
  Hyper Text Transfer Protocol
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
  <%= ruby %> and <% ruby %> the first one shows the result of the ruby action while the second only performs the ruby action.
15. What's an ORM?
  an Object Relation Mapper it wraps data in Ruby objects to make interacting with the information easier.
16. What's the most commonly used ORM?
  ActiveRecord
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
 get '/restaurants' do - shows you all the restaurants
 get '/restaurants/new' do - takes you somewhere to create a new restaurant
 post '/restaurants' do - posts the new restaurant
 get '/restaurants/:id' do - allows you to look as specified restaurant
 get '/restaurants/:id/edit' do - allows you to edit a specified restaurant
 put '/restaurants/:id' do |id| - posts the edited restaraunt
 delete '/restaurants/:id' do |id| -deletes the specified restaurant
18. What's a migration? 
  it allows you to update your database
19. When you create a migration, does it automatically modify your database?
  Yes
20. How does a model relate to a database?
  It creates a standard forthe data and how it can be processed and interacted with
21. What's the difference between agile workflow and waterfall method?
  waterfall is doing all of one thing at a time (for instance going through and doing the entire controller CRUD before you go and do the views for all of those actions) Agile would be doing the Create function to completion, then moving on to the Read and so on.
22. What is the difference between `#new` and `#create`?
  new doesn't save the entered data, create does.
