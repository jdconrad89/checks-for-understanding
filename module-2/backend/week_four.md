## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?
  A cookie is a piece of data that the server sends a computer to be able to use the browser and so that the server knows who   the user is (differentiates them from other users)
* What’s the difference between a session and a cookie?
  A session is n encrypted cookie
* What’s a flash and when do you want to use flashes?
  A flash is method in rails that allows you to "flash" messages on the screen (ie. successful/unsuccessful login, if           something was successfully deleted etc.)
* Why do people say “HTTP is stateless”?
  the connection between the server and browser is lost once the transaction is ended
* What’s authentication? Explain.
  Authentication is the proccess in which we have someone login so that we can verify thy are who they say we are.
* What’s the difference between authentication and authorization?
  Authentication lets them have access, Authorization dictates what they have access to.
* What’s a before filter?
  A before filter is a method we put at the top of the controller that we can put things that need to be completed before the   routes in that controller are ran. 
* How do we keep track of a user once they’ve logged in?
  in their session
* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?
* At a high level, what tools can you use to implement authorization? How would you use them?
  Bcrypt, it allows you to encrypt the password information so that you are never holding on to the specific password of a user.
* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?
   An enum type is a special data type that enables for a variable to be a set of predefined constants. The variable must already be set to on of the predefined types of that enum (depending on what it is you are looking for it could be an array of integers, strings etc). Yu declare them in the models
* What are some strategies you can use to keep your views DRY?
  Pull out things that are repeated in multiple views (like forms) and make their own view file, then reference that view file   in the other ones 'render partial: "form" ' 
