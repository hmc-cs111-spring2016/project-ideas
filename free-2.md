# Free project 2 - Brewing Simulator*

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

This project would serve brewers (amateur and professional alike) who do not know what outcome a specific type of recipe would yield. Brewing is an uncertain process and depends on a wide range of variables. Changing one small step in the brewing process could impact the entire result. A simulation language might be a good way for users to get a rough idea of their end product before starting the brewing process.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

I am helping anyone who wants to try their hand at brewing. Maybe a first-time brewer would use this simulation to start their very first recipe. Maybe an experienced brewer would try to create a completely different end product and would want to test their ideas before starting. This idea is a response to the uncertainty in brewing and aims to increase the experience of the user so that they gain a greater awareness of how each unique variable in the brewing process impacts the final brew.


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate for this scenario because it allows the user to do a specific set of tasks related to a brewing simulation. It would not require users to be technical and it would not try to do more beyond addressing this need. It has a very clear purpose and the commands would need to be very specific depending on the variables entered by the user. 


### Why you?
_What excites you about this idea? How did you come up with it?_

I have recently been doing research on homebrewing and am only beginning to discover all of the factors that affect the outcomes of the product. Drawing on many different sources, I attempted to craft my own recipe to achieve the end result that I want. I think that this language would be very helpful for someone like me who knows what they want from an end product but can't find a specific recipe to suit their needs. Also, one batch of brew is a significant time investment and it would be helpful to have more of an idea of the end product before putting weeks into the process.


### Domain
_Describe the project's domain in five words._

Simulated outcomes for brewing conditions.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

Since the language would be aimed at users with a wide variety of technical backgrounds, I think that a GUI (or something similar) would be optimal. The GUI could contain multiple fields or a series of questions in which users input their brewing conditions. These parameters are adjustable by the user and comprise a program. As stated before, this is correct for the domain because it will allow a wide variety of users to construct simulations.


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, the GUI would output the result of the brew. This could provide a variety of information depending on what would be brewed. It might include the sweetness/dryness of the end product and the amount of carbonation. The language could possibly simulate the brew over time and show the state of the brew (give statistics and the aforementioned information) at any time step in the process. This may involve an animation or graphs of certain variables over time. Any errors in compiling the program would be communicated in boxes prompting the user to input valid values for a certain field. A different type of error would be if the brew would explode with the user's given conditions, which could be shown in an animation or a visual message.


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy for users to input values and to choose the conditions under which they want to brew. It should also be possible to view the results over time. However, it should be impossible for the user to enter nonsensical values (e.g. negative brewing time). Potentially, it might be difficult but possible for the user to add their own conditions to the simulation. If they would be trying something new and could enter accurate information about the impact on brewing conditions, the user might be able to grow the language simply by interacting with the GUI. 


### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are several DSLs in this domain in the form of games. One such example is [Fiz](http://brewfiz.com/) in which you are in charge of running your own brewery. There are also other tools available online such as the Brewer's Friend [ABV Calculator](http://www.brewersfriend.com/abv-calculator/). This allows users to enter information about their brew and determine the alcohol-by-volume at that point in the process. I think that each of these examples has good qualities. The game is more user-friendly and serves a very different purpose than the calculator. I think that the calculator could be improved to have more functionality and that the game is not very helpful to someone looking to get quick information for brewing.


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I think that the project would be split between language design and systems work. It would entail the construction of a formula that takes many different parameters and can simulate behavior over time. There would ideally be a non-trivial graphical display portion of the project. The language would need to allow for the creation of new variables and parameters. The DSL could be made more complex if it gave users more options (i.e. the ability to choose different variables to graph against one another). 


### Scope
_How big an idea is this? How ambitious is this project?_

This is a big idea and an ambitious project, though I think that it's achievable in the timeframe of the class. It involves a lot of different UI and language design components and has the potential to be a very useful tool.


### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This project could appeal to a wide variety of people and be expanded to different types of beverages. It would be user friendly and technically challenging for the developer. It might not be a good project because the DSL might be relatively simple and overshadowed by the brewing formula. This would depend on the implementation of the DSL and the end capabilities of the project.


\* Disclaimer: I am over 21, though the simulator could be constructed for non-alcoholic beverages such as [Kombucha](https://en.wikipedia.org/wiki/Kombucha).
