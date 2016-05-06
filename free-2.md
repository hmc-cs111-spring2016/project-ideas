# Free project 2 -- Wine pairings


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

This project would help wine enthusiasts choose wines that pair well with the food that they are eating or making. A language would be nice because wine pairings seem like something of a closed set of terms, which could be implemented in various ways.

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

Lots of people like wine and food and consider themselves to be foodies. However, lots of people probably don't know be heart exactly which foods and wines go well togther, and want to improve their eating and drinking experiences. I could imagine a person who is eating a steak with potatoes, and wants to pair a wine with it but isn't sure which wine they want; perhaps they could even input to the program a list of wines that they are choosing between and the program/language could then help them choose the most appropriate choice. 

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL seems like a good choice because wine pairing is a fairly narrow domain, and users could use the language in order to educate themselves without having to go through too much other information. A language devoted strictly to this topic could be really helpful in assisting users expand their tastes for wine and food.

### Why you?
_What excites you about this idea? How did you come up with it?_

My whole family are huge wine snobs, yet I find that I am often lacking in the taste refinement that they have. I feel like I would totally use an app like this to improve my own experiences with food and wine, and I feel like even experienced wine drinkers could learn some new things about the way they experience wine.

### Domain
_Describe the project's domain in five words._

Pairing foods with appropriate wines

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

I think there are two ways one could go about this. One option is that the user inputs specific foods or recipes - spaghetti marinara, grilled fish with soy sauce, etc - and then the program would provide either wine categories or specific wines that would work well with that food/recipe. This could be a tuples of wines/wine categories, and the amount between 0 and 1 that that wine is a good match. As such, programming in that language would look something like searching through a list of foods and then calling a findPairings on that food. This would be nice because it would be easiest for the user to get exactly the desired result.

Another option (probably the easier to program) would be to have the user input flavors or ingredients that are dominant in the food they are eating, and then have those inputs evaluated in order to produce the best matching wines. This seems like what would be happening under the surface anyway in the first case, and would require more work from the user. This would possibly be more versatile, however, if the user wants to pair with a food that isn't well known or perhaps doesn't even have a well known name.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

Once the program receives the inputs from the user, it would then aggregate the flavors/recipes and use the dominant tastes/textures/whatever else in those foods in order to match them up with the best wine. I imagine it would create some sort of coefficient for each wine or wine category, which would describe how good of a fit that wine is. The highest scoring wines would then be returned to the user.

Errors would occur if foods or ingredients are not recognized. I imagine the user would be prompted to add those foods to the DB, or otherwise to try something else.


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

If should be easy to check which wines go with well known / common foods, and it should be more difficult to pair wines with foods that don't yet exist, or otherwise need to be described. It should be impossible or very difficult to suggest food based on wine (at least at first), and all other variants/activities that are far from the ultimately quite narrow domain.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

[This website](http://www.matchingfoodandwine.com/) seems to do exactly what this DSL describes, but I played around with it and it seems really clunky and limited in the food options. It also simply links to individual blogger opinions on various wines, and doesn't do any sort of "objective" calculation of which flavors in the food would go well with different wines.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I think this would be a systems-heavy project. A lot of back-end work would have to be done, in order to create a list of wines that are suggested, and to create a way to rank wines based on specific attributes of various foods.

### Scope
_How big an idea is this? How ambitious is this project?_

I think a good version of such a project would be a massive undertaking. That said, a working (if imperfect) version seems like something that could be doable in the time we have available.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This would be a cool project because I think it wouldn't require too many changes in the language, but would still have enough logical work that would have to be done that it would be significant. The algorithm by which the best wine is determined would be of paramount importance, however.

I think the biggest challenge with this is that there would have to be a massive database of wines or wine categories, and the qualities of these wines (and the foods they'd go well with) would have to be prepopluated / agreed upon by some wine expert(s). This makes the whole nature of the prograem rather subjective which is not ideal.
