# No computer project


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

Many people enjoy playing card games and many strategies have been developed for optimizing your chances to win, especially in gambling games such as Black-Jack and online poker, but people often have trouble keeping track of what move they should make next to grant them the highest probability of winning. I would like to help gamblers determine the best move so that they can optimize their chances of winning, by creating a language with simple, systematic rules based on a probability maximizing strategy. This would give them an unemotional, rational way to make their decisionsso that they could maximize profit and minimize loss, rather than just depending on their luck and feelings.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL would give the users a simple, logical set of rules they could follow and base their playing decisions on, rather than allowing them to make irrational decisions based on how they feel at any given point in the game. Many gamblers who are beginning to win big, bet it all in a subsequent game and lose any profit they made. A DSL in this limited and specific domain would easily address this issue without requiring them to become experts in statistics or any broader domain.

### Why you?
_What excites you about this idea? How did you come up with it?_

I love playing cards, I tend to try to analyze the game and then decide what to go for based on my probability of success. Freshmen year I took Math of Games and Puzzles with Prof. Arthur Bejamin and enjoyed it immensely, but I have many friends who aren't as good at doing probability calculations or estimations on the fly who are consistently frusterated when their luck lets them down. I was talking to Prof. Bejamin this week about some of his card counting strategies and realized how easy it would be to put those strategies into a DSL.

### Domain
_Describe the project's domain in five words._

Probabilistic card game strategy optimization.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

A program would look like a conditional tree, where each branch ends in an instruction. THe user would move down through the tree, evaluating the conditional at each branch to decide the correct path to take until the reach the end of a branch and it tells them what move to make next. This allows the user a simple, intuitive way of considering the state of the game and using it to determine what move they should.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When the program runs, it begins by asking the user a simple question about the state of the game, based on this conditional, the program will branch. This step will be repeated until the program has enough information from the user to determine what move they should make and gives them the appropriate instruction. An error would occur if the user was in a novel situation and the conditional could not be answered or if the user chooses not to act in accordance with the given instructions and thereby decreases their likelyhood of winning.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to maximize your chances of winning a game. It might be hard but not impossible to keep track of every card that has been played, or to make a program that can actually take all that input and still advise you on your next move quickly enough. It should be impossible to use the conditional tree for anything besides a card game.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

[This website](https://www.pagat.com/poker/software.html) provides links to a wide variety of software programs designed to tell you probabilities or assist you while playing online poker, I think a more simplified version, perhaps using a tree that could be printed out by a user would be more fun and more helpful for the average player and easier for them to memorize the logic flow so that they could quickly run the program in their own minds while playing poker with other people in person.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

Most of the time someone spent on this project would be spent learning the probabilities, designing the conditional tree to determine what conditions should determine each branch. The biggest struggle would be in finding the best balance between detailed complexity which would allow the program to give the player the exact best move every time, and in keeping the program small and simple enough that the average user can keep track of what has been played, correctly answer the conditionals, and perhaps even memorize the conditional tree so that the can run the program in their own mind when they are playing in person with other people.

### Scope
_How big an idea is this? How ambitious is this project?_

I think this could be done within the given timeframe. This would be enough work for the full time and could be completed and then edited several times to make it better.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This seems like a cool idea for a project, it would be useful to game players who want to develope better game playing strategies, almost all of the time would be spent determining what conditionals should be used and optimizing between the best strategy and the easiest to remember strategy to best serve our users.
