# Free project 1 - Flavor Pairings

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This DSL would help users learn more about flavor pairings and make suggestions if given specific foods. The users would be able to figure out foods or beverages that would pair well with a given item. For example, if a person were hosting a dinner party and didn't know what to serve with the main dish, they could receive suggestions about flavors or dishes that would be good accompaniments. 


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

Flavor pairing is a unique domain and a DSL would help to educate users about successful pairings. It is appropriate for users because they would be able to interact with pairings in various ways (learning about more pairings, getting pairing suggestions, etc).


### Why you?
_What excites you about this idea? How did you come up with it?_

I am very interested in food science and flavor combinations. I talked with one of my friends who has similar interests and she said that she didn't always know what flavors would pair well together when trying to create a meal or dish. I had looked for similar pairing services in the past and was not satisfied with my findings.


### Domain
_Describe the project's domain in five words._

Flavors that go well together.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user could interact with the language by typing in a food or dish as well as what they wanted with it. They could specify that they wanted pairing suggestions in a certain category or they could ask for a random suggestion. The categories could be anything from dish vs. flavor to certain type of food. Perhaps the user wants a certain number of suggestions, perhaps the only want to know about beverages that would pair well. Since the language is designed for people to gain more information about food pairings, it makes sense for a program to revolve around a central object or dish. This way, the user could learn more about that specifc object. A more advanced feature of the language could be the ability to list multiple foods and receive suggestions common to all foods in the list.


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

The program would run and output all pairings in a database that fit the given criteria. It would interact with the user by listing suggestions. Depending on the scope of the project, the suggestions could all be images or links to more information. The user could get errors in which no flavors exist for a given criteria. In this case, the language could suggest related searches. It is possible that the user would try to search for a food not in the database, though this could be limited by selection from a UI. 


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to enter the name of a food and learn about flavor pairings. It should be easy to refine those results based on number or category. It should be possible but difficult to categorize each of those foods and to get information on multiple dishes or flavors at once. It should be very difficult, if not impossible, for users to add their own flavor pairings. This would depend on the separation between users for the DSL, since it is not optimal to enable any user to create a pairing for mustard and chocolate.


### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

A similar service, [Foodpairing](https://www.foodpairing.com/en/home) already exists. However, it requires users to sign up and pay. I signed up for the free trial and it allows users to receive pairings based on foods they input. However, it also tries to let users create their own pairings. All of this is done through a confusing graph interface, where each node in the graph is a different type of food. I think it has a good database of foods and flavor pairings but the interface could definitely be improved.


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

The developer's attentions would probably be distracted by creating flavor pairings and figuring out a method of efficient searching through a connected graph. It would get particularly confusing to introduce categories (potentially in the form of attribute tags) for each different flavor or food. It would be easy to spend too much time focusing on this setup instead of the actual language for the user.


### Scope
_How big an idea is this? How ambitious is this project?_

As discussed in the previous question, this is potentially a huge project. It would be very ambitious to create a flavor pairing graph, especially if users were allowed to define their own pairings. It has the potential to be an incredible service, but it would be difficult to implement much functionality over such a complex data set in the timeframe of this project.


### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This would be a good idea for a project because it could be a great DSL to present users with a lot of food pairings tailored to their specific needs. However, as previously discussed, the scope of the project could end up being very significant and the focus might shift off of the DSL itself.

