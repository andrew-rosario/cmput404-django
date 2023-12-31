#### Question Answers.

##### Question 1
https://github.com/andrew-rosario/cmput404-django

##### Question 2
It gives me a webpage that says "The install worked successfully! Congratulations!"

##### Question 3
At the root ```/```, it says that the page cannot be found (HTTP response code 404).

At the ```/polls``` directory, it shows the line, "Hello, world. You're at the polls index."

##### Question 4
Django migrations synchronizes the changes by your models to your database. We need them because the website is expecting certain fields from the database. Thus, Django migrations handle the database schema modifications for you, regardless of what database you choose.

##### Question 5
I'm assuming you create your model in the models.py file, then you go into the admin.py file and register your new model. (I think a Django migration is needed for this to work, to add the new model to the DBMS).

##### Question 6
It shows "You're looking at Question 38." Then, "You're looking at the results of question 38." Then, "You're voting on question 38."

To allow alphanumeric characters, change the accepted content type to string. (```<str:question_name>```)

##### Question 7
We might change the name of the polls. Or the resource might not exist in that location anymore.

##### Question 8
Let's be real, the benefit is... why not?

But seriously. Some views are generic as is. Question fields are question fields. Voting fields are voting fields. Detail fields are detail fields. And so on. I don't see a need for 'reinventing the wheel' if it already exists in some form. 

We shouldn't use a generic view if the generic view will not suffice for our usecase, or if we want to extend the capabilities of the views beyond overriding their attributes. 