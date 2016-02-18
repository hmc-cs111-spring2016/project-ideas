# Ingredients to Dish

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

This language seeks to provide a way for people to know what dish they can create based off of the ingredients they have. You can think of it as the quintessential cook book. The users will be able to choose from a variety of dishes they can actually make, rather than havin to query through several recipes they may not have the ingredients for. A language would be a good way to meet their needs as they could make the most out of their ingredients rather than settling for a dish missing ingredients.

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This idea makes it significantly easier to decide on what to make for a particular meal by eliminating most recipes. This idea helps people who don't have a large variety of ingredients to still make delicious dishes. As of now, the person either finds a recipe that they do not have all the ingredients for, spend a long time finding a recipe they actually have all the ingredients for, or completely forgo a recipe and try to throw together a dish. With this DSL, they could actually find usable recipes.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate for the users because deciding what to cook is a pretty specific domain. It addresses the need by enumerating all possible choices. 

### Why you?
_What excites you about this idea? How did you come up with it?_

As someone who doesn't own a small nursery of herbs, it's disappointing to find a particularly appetizing recipe, only to realize it requires some obscure herb (I'm looking at you tarragon). I'm also realizing more just how important some of these missing ingredient can be (e.g. I didn't add ginger to a Chinese dish and it tasted super bland). It would be nice to be able to just see what I can actually make given my ingredients rather than waste time looking at every possible chicken recipe.

### Domain
_Describe the project's domain in five words._

Cooking with all your ingredients

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user will provide the ingredients they have to the language and will receive a list of potential recipes. The user can also have additional fields that categorize the dishes, potentially by ethnic region, by allergies, among others. The program would probably have some request object that has several fields including ingredients and additioanl search query fields. 

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, the user is given a truncated list of recipes they can make given their ingredients and potentially their categorization details. Some errors that might occur include no recipe existing in the intial database, improperly filled fields, misspelled ingredients, among others. It feels most errors will probably come form the use of natural language in the DSL.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

The scope of this language is pretty limited, so it should be easy to find a recipe to cook for a meal, and difficult/very difficult/impossible to do much of anythign else.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

I didn't realize this before hand, but a quick Google-ing of the idea and [this](http://www.supercook.com/) comes up. It is similar, and seems to execute the idea rather well. I'm actually surprised this is not used more often as it seems like a pretty useful idea. It has a good database of existing recipes as well as user submitte recipes. The interface is a little slow and unresponsive though, which would be one area of improvement.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

This project seems to be more about the "systems" aspect, such as finding an efficient way to store all these recipes and ingredients, finding a good way to fetch these recipes given a list of ingredients, amongst other implementation details. The language aspect seems to pale in comparison to the aforementioned problems.

### Scope
_How big an idea is this? How ambitious is this project?_

This seems like a potentially very large idea. Implementing the features as described above would probably be impossible to complete well in half a semester. It seems also difficult to implement the features mentioned above even with a team of people.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This would probably not be a great idea for the project as the implementer can easily get too absorbed in the "systems" aspect. This idea would be good if given more time and because it actually seems like a great and useful service.
