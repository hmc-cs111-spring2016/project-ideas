# Free project 3

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

There are many people who have an interest in making logic puzzles. There are plenty of magazines that feature them regularly, other games that feature them as more baked-in features (like a game with an expansive world with a puzzle element to it), and the people who casually enjoy those publications and may have an interest in making their own in a more casual way. These puzzles may be hard to generate: you have to come up with all of the variables involved and all of the rules you impose and meticulously check that their solution works and is unique.

I'd hope to be able to automate those processes. It would make constructing puzzles, testing them for having unique solutions, modifying them, and so on simpler. You'd be able to tinker with one rule that you imposed on a puzzle at a time until you get something that you think is interesting. 

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

Doing this programmatically is very natural, as many of these problems can be formulated as constraint satisfaction problems and CSPs have been well studied algorithmically. A general purpose PL is way too broad of a thing to learn for someone who has a casual interest in this domain and just wants to play around with things to get something interesting.

### Why you?
_What excites you about this idea? How did you come up with it?_

I sat down in my suite to write this up and saw my friends playing a video game called Doors. It's a really simple logic puzzle game where there are doors that say different statements about which ones are telling the truth or lying, and you have to figure out which one you're supposed to go through. It seemed like automatic puzzle generation like that would be nice (and looking around a bit online I think puzzles for this game were actually crowdsourced, so it could be very different). 

I think a lot of similar tools exist, but focusing on the fact that they can be formulated as CSPs would give a unique angle that would allow different kinds of puzzle generation - you could generate Doors puzzles, or you could generate classic fill-in-the-grid puzzles (if you're unfamiliar with them you can see examples on <http://www.logic-puzzles.org/>). Or you could make up your own kind of puzzle and make a bunch of them.

### Domain
_Describe the project's domain in five words._

Creating CSP-based logic puzzles.

(or if "CSP" is cheating, "different kinds of logic puzzles.")

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

In a CSP, there are variables which can take on possible values and constraints that specify what combinations of variables are possible. There would be two basic commands for specifying a logic puzzle: specify a variable, or specify a constraint. You'd be modifying a file that contains information about all of the variables and constraints that your puzzle has.

An alternative way of using the language would consist of specifying formulas that could generate rules. For instance, you might say "if x is p then y is q" is a valid rule (given variables x and y, and values p and q that they could take on). The program would use these as molds to generate specific rules, generating and removing rules until it finds a valid puzzle and then showing that puzzle to the user. The user could specify these rules both in natural language and in formal language - for instance "if x is p then y is q" might have a few different ways to phrase in English, and the user might want the program to spit out rules that say "in the case that x happens to be p, then y would have to be q." The user could specify any syntax for these rules that they want.

The program would also be able to display information about the puzzle - i.e., "37 solutions currently possible" or "problem is overconstrained" if none are possible. It could show which variables are particularly underspecified so that the user would know which variables to write more constraints on. It could potentially even suggest rules to add that would constrain the problem more, but not overconstrain it.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

It creates a model of a logic puzzle and checks properties of that model, and makes suggestions about how that puzzle could be altered based on the model. I can't imagine many other errors apart from syntactic errors. 

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to make logic puzzles and change them. It should be hard to make other kinds of puzzles (you might be able to work some way out to do them if you're creative, i'd imagine, but everything would be running on the model of a CSP.) It should be impossible to do anything other than specifying aspects of a puzzle, so there is a certain limit to how creative the user can be.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are tools like <http://www.mensus.net/brain/logic.shtml>. The way that that tool specifies kinds of clues is very similar to what I'd be looking for but I would want the user to have a higher degree of interactivity with the program, so that they could add and remove rules and look at what happens to the puzzle in "real time." The only feature that tool has is generating puzzles with certain types of rules. The workflow I have in mind would be more back-and-forth between the user and the language, and I don't know if any tool like that exists. There are tons of other tools to generate puzzles for solving that don't give the user even that much freedom.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

This might be a problem with this idea - the systems might be very difficult to get right here. The language design would also be a difficult aspect of it, however.

### Scope
_How big an idea is this? How ambitious is this project?_

It's more risky than ambitious, I think - risky in the sense that I'm not sure if the idea for the underlying model is sound, and it's very important. It would proably simply either work or not work in the end.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

It's a bad idea for the couple of reasons listed above. It's a good idea because it's very naturally a problem for which I think a DSL is really the right way to solve it. It seems very natural that people desigining these puzzles would want a DSL-like interface for their design, and I think a DSL could offer a lot in a lot of different ways. 
