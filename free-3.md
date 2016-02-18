# Free project 3

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

Super Smash Brothers Melee (SSBM) is an extremely popular competitive fighting game (there were about 200,000 concurrent viewers for last years biggest tournament).  The game is very deep, and top players engage in a lot of "theory-crafting" (theorizing about hypothetical situations that could come up in the game).  Because there is no systematic way of notating scenarios in SSBM, theory-crafting discussions over the internet can be quite difficult to maintain.
My language would allow users to describe the details surrounding the hypothetical in-game scenario and it would decide who the "winner" (the opponent who is in an advantageous position at the end of the scenario) is based on the game's frame data.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate because it would allow users the control to precisely describe very frame-specific scenarios that often come up in the game.  It would address the need by parsing a file of "moves" used by each player and determining who would end up in an advantageous position.

### Why you?
_What excites you about this idea? How did you come up with it?_

I came up with it after reading through some theory-crafting posts about frame data in super smash bros.  This project is exciting because it'd be directly applicable to a hobby I'm passionate about.

### Domain
_Describe the project's domain in five words._

Super Smash Bros Theory Crafting

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

Users would interact with the program by defining two players, the characters they are using, and a list of moves that the characters would use in some hypothetical situation. 
Example:

Player A: Mario  
Player B: Falco

- A: Shield (full)
- B: Shine-grab (-2)
- A: Buffer spot-dodge
- B: SHFFL dair
- A: Shield
- A: Up-B OOS (-3)

Note: (-2) indicates that the user is 2 frames imperfect in his/her execution of the move.  
This is the right way to interact with the problem domain because it basically mimics the way people already theory-craft about SSBM.  It also uses a lot of jargon familiar to SSBM players, which greatly reduces the amount of time it would take to write a program.  The advantage with a DSL is that it can compute who the winner is without the theorist having to figure it out him/herself.


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program like the above example runs, the program would parse through the moves and, based off an internal store of the game's frama data, decide who the victor of the outcome is (usually the first player to get hit by a move).  Users would get an error if, for example, they try to use a Fox-specific move with Mario.  This might give an "illegal move" error that points users to the problematic line of code.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to figure out which character wins in very specific hypothetical situations in SSBM.  It should be impossible to decide the winner of an entire match, and it should also be impossible to input scenarios that involve more than two players (up to four people can play SSBM simultaneously, though 1v1 is the most popular mode).

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There aren't any other DSLs in this domain.  I know because I spend a decent amount of time on smash-specific subreddits and if a DSL existed in this domain I would've heard about it.  A DSL in this domain likely doesn't exist because there isn't a huge need for it.  Theory-crafting can be done without a DSL by manually going over frame data.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

Most of the time would be spent working on the language.  The game data that the DSL would use in the background is available online, and the algorithm for determining a winner involves only a few factors, such as "shield-stun" and "ending-lag".  My guess would be that around 60-70% of the time would be spent working on the language.

### Scope
_How big an idea is this? How ambitious is this project?_

The project is moderately ambitious.  Because there are so many characters in the game, each with a long list of unique moves that they can perform, it could take a while to catalog all the possible inputs.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This might be a good idea because it is largely about the language.  All of the game's frame data is readily available, so creating an algorithm to determine the winner of a scenario shouldn't be so time consuming.  It might not be a good idea because it's a super niche domain, meaning it might be hard to get proper feedback from my classmates/professor.