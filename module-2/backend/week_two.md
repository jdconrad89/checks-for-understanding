## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do? 
  It is a Ruby Library that allows you to work with relational SQL/
2. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.
  They are associations (would they be considered class methods? An example would be that a car belongs to one driver but a     driver could have many cars.
3. What do they allow you to do?
  It allows you to call on the relationship between to tables and call methods on them to find the different objects from both   ends of the relationship
4. What's the difference between agile workflow and waterfall method?
  Waterfall is a very incremental form of development Where you would develop, then test, then fix any errors, then finalize     for customers, then release. In an Agile workflow is a more iteration driven approach where they get a single functionality   created and tested, prepared and launched and then move onto the next iteration.
5. What is the difference between `#new` and `#create`?
  New doesnt save the new instance of the object it only makes it. Create makes the new object AND saves it
6. At a basic level, what does cURL allow you to do?
  it allows you to send information using URL syntax?
7. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
 Students have many teachers and teachers have many students. See picture down in comments
9. Describe the relationship between a foreign key on one table and a primary key on another table.
  A foreign key is a reference in a table to the primary key in another table. It is how the key with the foreign key has       access to the information in the other table where the primary key is.
10. What are the parts of an HTTP response?
    status line, message, body
11. Describe some techniques to make our Sinatra code more DRY. Give an example of when you would use these techniques.
  I'm not quite sure I know/remember what you mean by DRY...


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
  db:drop - it drops your database and tables(there are times i make a bunch of errors and rather then creating a bunch of new              migraitons to fix the tables it's easier just to drop it and try again)
  db:rollback - Rolls the schema back to the previous version
  db:"Whatever you put in the tasks file" - any commands you create in the task file you can run with rake.
4. What can you expect from a group as you begin working together? As you continue working together?
5. What two columns does `t.timestamps null: false` create in our database?
    Created At and Updated At
6. What cURL flag can you use to send a `POST` request?
7. What case does JSON (and JavaScript) use for multi-word variables?
8. What case does Ruby use for multi-word variables?
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
  schools will have many teachers but a teacher will belong to only one school.
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
11. Give an example of when you might want to store information besides ids on a join table.
12. Describe and diagram the relationship between patients and doctors.
13. Describe and diagram the relationship between museums and original_paintings.
14. What are some examples of acceptable values for the parts of an HTTP response?
15. What types of output do we want to test when we test our controllers?
16. What could you see in your code that would make you think you might want to create a partial?
17. Why might you use a helper method?
