# No computer project - Recipe Book

## The user and a language

My "no computer" language in this scenario is a recipe book. The user of this language is a person who wants to make food for themselves or others. It would teach a person to make a dish, which is particularly helpful if the person in question does not know how to make the dish that they want. If they are unsure of what they want to cook, the recipe book can give suggestions for dishes and then provide instructions once the user has selected their desired dish.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

The idea meets the need of people who don't know how to make recipes they want to cook. The language would serve everyone from first-time cooks to experienced chefs who do not have the recipes memorized. Each recipe they would make from the book would help to increase their experience. If they were to make all recipes from the book multiple times, presumably their cooking skills would improve and they would use their new experience to perfect the dishes.


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate for the users because it could provide a recipe in a helpful, readable format. Additionally, if the language was an entire recipe book, users could browse recipes by categories depending on the type of thing that they want to cook. If the user is completely inexperienced with cooking, it would be possible for them to open the book to the first recipe and follow along with each instruction.


### Why you?
_What excites you about this idea? How did you come up with it?_

I am excited about this idea because I think it has a lot of potential as a DSL even though it's technically the "no computer" language. I really enjoy cooking and use recipe books (though mainly online recipe sites) quite frequently. The idea would be very interesting to implement as a DSL, especially if I could include novel features.

### Domain
_Describe the project's domain in five words._

Step by step food preparation.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user can interact with the language by searching for a recipe and then executing that recipe. A program would involve opening the book, turning to a desired recipe page, and following the sequential instructions on that page in order to achieve a final product. It is the right way to interact with the problem design because otherwise a user might try to cook without having a recipe. They could also try to follow the steps out of order, or somehow end up with the wrong type of recipe if they did not search for the right category. 


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

I discussed various sources of error in the last response, but when a program runs, the user searches for and flips to a desired recipe and then executes the instructions given by that recipe. The program interacts with the user by providing a list of recipe choices based on the categories the user searches for. The individual recipes then interact with the user by telling them what to do in each step. Some recipes describe the way that dishes should look after certain steps, which would be a method of error-checking for the user. If the recipe includes pictures, the user can determine whether their food resembles those pictures or not.


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to search for a particular type of recipe and determine whether one exists in the given recipe book. If there are multiple recipes that match the category, it should be easy to view a list of these recipes and select one. It should not be possible to select two recipes at once. Depending on how much control the user wants over the book (whether this is a compendium of their recipes or a book distributed by someone else), they should not be able to delete or add recipes. As for something possible but difficult, I would think that the actual cooking part falls into that category :)


### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

If we think of DSLs in the domain to be recipe books, then there are a lot of DSLs in this domain. I think that the domain can span multiple types of recipe collections, so several different examples are [Mastering the Art of French Cooking](https://en.wikipedia.org/wiki/Mastering_the_Art_of_French_Cooking) and [AllRecipes.com](www.allrecipes.com). I think that both examples are good for recipe searching, though the ease of use really depends on the background of the user. The book form of the language could be improved by being more easily changed, though the digital form of the language could be improved by being put into print (since some people may find it more difficult to cook with a computer in the kitchen).


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

Time would mainly be spent on the language aspects of the project. I think that the main goals would be to design and optimize language commands for efficiently searching through recipes. I don't envision many complicated semantics, especially if the DSL boils down to various operations on a database of recipes.


### Scope
_How big an idea is this? How ambitious is this project?_

I don't think that this is a very ambitious project unless it tries to do something very novel. It would be interesting to think of new ways to implement features. The project could instantly be more ambitious if new technologies such as voice recognition were added. I would be interested to attempt this project from a hands-free cooking angle, since I think it would combine features of digital and physical cookbooks with the added excitement of verbal DSL commands.


### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This would be a good idea for a project because it helps to design an entirely new experience for the user in the kitchen. There is a risk that people would not like this experience, but that would hopefully be mitigated through interviews and user feedback. Unless the scope of the idea were more focused, the project might be too general and end up exactly like an existing online recipe site.
