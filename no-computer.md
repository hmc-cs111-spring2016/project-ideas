# No computer project


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

Explaining game rules can be pretty hard. A lot of people strugle to explain game rules to each other and it only gets harder when explaining them to something like a computer. By creating a DSL for game rules, we can standardize game rule formate and maybe even help game AI makers in the process if the syntax is rigorous enough.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

Describing games and the rules to play them does not require a lot of different terminology for many board games. Thus, a limited-scope DSL could fit this purpose. The DSL would standardize how game rules are described and enourage clarity so that users can understand them better.

### Why you?
_What excites you about this idea? How did you come up with it?_

What would be really really cool is if the rules are specific enough that you could automatically generate a computer version of the game and/or an AI for the game. This idea was inspired by my idea to write up a board game (like Monopoly) for the no computer project and by a [previous final project](https://github.com/AriHC/RuleBook/blob/master/documents/final.md) from DSLs.

### Domain
_Describe the project's domain in five words._

Standardized game rule description language.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user would simply consume the "programs" in the language to learn about the game described. Readability will be key as this would technically be aimed at people, but it would be acceptable to make it more strict so that computers can parse it as well.

Programming would involve taking a game (existing or theoretical) and expessing all the rules of the game (as well as some metadata) in the DSL. There isn't currently a "right way" to interact with the domain, but many games have rule books that are at least somewhat similar to each other. Looking at these could be a good starting point.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

It's not entirely clear what a "program" in this language should do, but it should be clear what someone can do after reading in a "program." People should be able to play the game in question as well as perhaps detect logic errors in the game's rules description. They should even be able to act as a host for the game and make sure all players are following the rules.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

Ideally, it would be easy to describe the rules for major board games. It may also be possible to describe rules for different kinds of games (like card games), although it should be clear that it will be hard to make a DSL that can describe _any_ game's rules well. There will be some games that are just way to different from board games that will not work well with this DSL. Obviously, it should be difficult to describe stuff that is not game rules in this language.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

Other than the DSL mentioned earlier, I am not aware of standardized ways of describing game rules. Certain game publishers might have specific rules or formatting guides for rule books, but these aren't what this DSL would be about. People have been able to get away with expressing rules in English, so there probably has not been enough of a need for something like this.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

This would be very focused on the language, especially since there doesn't have to be a computer involved at all.

### Scope
_How big an idea is this? How ambitious is this project?_

I'm not entirely sure. Since not much like this has been done before to my knowledge, it could turn out super easy to describe game rules or (as I expect) it could potentially get quite hard once you really start to consider a lot of the different play styles that are out there, even for board games.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

It would be pretty unique and involve working with board games, which could be really fun. If you work to make the language good enough for computers to parse, this could open the door for a lot of automation in producing electronic games and game AIs.

However, this could also get very complicated and turn out to be undoable. Describing games can already be hard enough, so standardizing that could be even harder.