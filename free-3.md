# Free project 3


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.
 

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This language would serve people playing board games or card games who want to know what decision to make. The idea of doing this in a language is to enable the users to specify their own games, with their own rules and win conditions. Thus, the user would be able to both query the language for what decision to make, as well as specify the game they are playing.

Card games and board games are very serious among some people, and arguments among these people take place pretty often. Having a tool that can be run hypothetically in many different scenarios would be very useful. As of now, the player would have to do things like approximate probability calculations in their heads. This tool would make that a little bit simpler, just by automating the things that can be automated with the information the player has.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL for this seems pretty natural, as languages are often the best way to specify a new type of thing. Additionally, once this exists, a game object, or class, or data file can simply be queried in some familiar language syntax to get results. The domain can be very specific, as its literally just for specifying games and asking questions about them. 

### Why you?
_What excites you about this idea? How did you come up with it?_

Card games was on the list of suggested domains, and since I like card games a lot, I figured it would be interesting to think about DSLs that could make card games either easier or more interesting. This sort of would do both, as it would be a way to assist decision making, as well as consider interesting scenarios in an arbitrary game.

### Domain
_Describe the project's domain in five words._
Game specification and decision making

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

There would be two main interactions with the language. First, the user would write what a game looks like, probably using object oriented notation, as it makes the most sense for this domain. Second, the user would select a game, input all of the known information, and ask questions (like, my hand is (x,y,z), what should I play to maximize my chances of Q). 

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program is run, it should basically do some simple AI techniques (probably just an expectimax search) with the parameters specified by the user in both the game and the current query. In terms of errors, the obvious case for an error is when there isn't enough information for the engine to run a search. In this case, there are two options. First, the program should tell the user this, and ask for any additional information. Second, if the user cannot give any, it should let the user know that it can't answer the question, and terminate "gracefully".

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be as easy as possible to specify the game rules for whatever game you want. This has already been done, so I think its reasonable. It should also be as easy as possible to specify the current game state. Things that are possible but difficult probably include very advanced inference, where the user asks the game to make a decision based on his/her own strategies/playstyle. This would have to somehow be included in the values for different plays, so it would be hard to do, but theoretically possible.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

In terms of the game creation step, there is one DSL called [zillions of games](http://www.zillions-of-games.com/) that lets users specify the rules for board games. I'd plan on looking at their documentation for ideas, and extending it to card games. In terms of decision assistants, there are certainly bots that do this kind of thing in different games (e.g. Hearthstone, and more recently Dota 2), but its not really publicly available as a language, and is mostly for video game versions of specific games (like checkers, since its solved).

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I suspect, but am not sure, that the bulk of this project would be the language decisions. Giving users the flexibility to design their own games, but also making an engine that works for all of these specifications would be very tricky. The engine itself would be fairly simple, expectimax is pretty easy to write. 

### Scope
_How big an idea is this? How ambitious is this project?_

The main issue is here. This project feels like 2 different DSLs. I'm not sure exactly how much work each one would take, but it does seem like it might be too ambitious.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

The main reason this would be a good idea is that its an interesting exercise in making something with a ton of flexibility have enough specificity that an engine can run queries on it. This would be a perfect exercise in design decisions. However, like I said, the scope might be a little much, and I'm not sure its feasible. 
