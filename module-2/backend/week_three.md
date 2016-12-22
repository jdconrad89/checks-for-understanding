## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What is the entry at the command line to create a new rails app? 
  rails new whatever the app name is (you can specify more things in this command line like what sql database you want to use etc.)
2. What do Models generally inherit from in rails? 
  ApplicationRecord
3. What do Controllers generally inherit from in a rails project?
  ApplicationController
4. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
  resources :horses, only[:show]
5. What rake task is useful when looking at routes, and what information does it give you?
  rake routes it gives you all the available path names, url names, and what method it needs in the controller
6. What is an example of a route helper? When would you use them?
  in our routes file we can specify what we want the actual route name to be, so if we wanted to do a login we would set it as a login as opposed to it being create(it's more indicative of what we are trying to do and that way it is easier for users to use)
7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?
  _path is how we are able to refer to the different path names inside of our program. _url is the link that you would see in the nav bar
8. What are strong params and why are the necessary?
  it helps us protect our application by limiting what people can enter as parameters for what we are creating. It's another form of security. 
9. What role does `form_for` play in helping us create our forms?
  it's a method in rails to help us create a basic form and where the user input needs to be sent
10. How does `form_for` know where to submit the user's input?
    we tell it "form_for @horse"
11. Create a form using a `form_for` helper to create a new `Horse`. 
 in new.html.erm
    <h2> Create a new Horse </h2>


    <%= render partial: "form" %>
 
 
 
  in _form.html.erb
 
 <%= form_for @horse do |f| %>
    <%= f.label :name %>
    <%= f.text_field :name %>

    <%= f.label :breed %>
    <%= f.text_field :breed %>

    <%= f.label :age %>
    <%= f.text_field :age %>

    <%= f.submit %>

  <% end %>

12. Why do we want to validate our models?
  Too make sure that we can't create them with missing data (makes it easier for tracking down errors and failures later on in the program)
