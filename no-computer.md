# No computer project


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

People are always looking for fun ways to exert dominance over their peers.  Sports, video games, and board games are all activities that can satisfy this need.  Sports are especially popular due to their added benefit of involving aerobic exercise, and two great sports to play are badminton and ping-pong.  Both are great because they are one-on-one (if you win, you are simply better than your opponent - they have no team to blame) and they involve hitting things, which further emphasizes dominance over one's opponent (it'd be even better if you could directly hit your opponent, but then they might be considered martial arts rather than sports).  However, each has its cons, as follows:
- Ping pong requires a ping-pong table, which is expensive and takes up a lot of space.
- In both games, unless you are an experienced player, hitting the ball/birdie with any notable amount of force will cause it to go flying out of the playing field.  This is no fun.
- Badminton rackets look dumb.

My DSL, pingminton, combines both sports to create a truly electrifying experience that lacks the downsides of either parent sport.  It takes the paddles from ping-pong and the birdie/net from badminton.  When playing pingminton, you don't need a table, you don't have to carry around dumb-looking badminton rackets, and (most importantly) you can whack the birdy with a large amount of force without it going too far.  This combination of ease-of-play, looking not lame, and getting to use lots of force creates the perfect environment in which to exert dominance over a peer.


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate because it allows users 

### Why you?
_What excites you about this idea? How did you come up with it?_

I came up with this idea many years ago with my brother.  We were in a competitive spirit and wanted to play badminton, but found that we'd always hit the birdie too far when using badminton rackets.  We tried using different objects that wouldn't send the birdie so far (books, slabs of wood, etc), and eventually settled on ping-pong paddles.  This DSL excites me because I spent a large portion of my childhood playing it.

### Domain
_Describe the project's domain in five words._

Exert dominance over your peers

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

Users interact with the language (the sport + the opponent) by hitting the birdy over the net with their ping-pong paddle.  If the birdie returns over the net, they must continue hitting it over the net until the desired outcome is achieved (e.g. athletic dominance has been exerted).  In terms of programming, the syntax of a single hit consists of the angle of the ping-pong paddle, the speed at which contact is made, and various other factors like wind speed and the material of the paddle.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When the program runs (ie a game is played), both users are interacting with the program at the same time.  For each user, the program consists of the game + their opponent, and the program runs until the match has ended and one player has won.  The program interacts with the user by accepting "hits" as input, and it reports errors (such as hitting the birdie into the net) by having the opponent laugh at the player.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

With this program it should be easy to exert athletic dominance over your peers, unless you're bad.  It should be easy to play games of pingminton as defined by the rules of the game (essentially hitting the birdie over the net).  It should be difficult to run programs (games) that are too long, since players will grow physically tired.  It should also be difficult to run the program with more than one "birdie" object.  It should be impossible to do things from other sports like dunk, slide-tackle, or hit home runs.  I don't think pingminton is Turing complete (volleys always go back and forth), so most computational tasks should also be impossible.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are many DSLs in this domain, such as soccer, Monopoly, volleyball, and Super Smash Brothers. Melee.  These all address the needs of users relatively well (except for Monopoly) by providing a skill-based manner in which people's competitive tendencies can be appeased.  An admirable quality that many of these DSLs have is that they have well-defined rules, which is something that pingminton could learn from.  Most could be improved by making them more accessible (i.e. involving less equipment).

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

A major language aspect of this project if defining what types of inputs, or hits, are valid.  For example, spiking is illegal in volleyball.  Should spiking be legal in pingminton?  How exactly do users input a spike (ie what constitutes a spike)?  These questions need to be answered in order for users to be able to run a "syntactically correct" program of pingminton.  Because all the development time for the project would be spent on defining these types of rules, almost 100% of the project would be language-focused.

### Scope
_How big an idea is this? How ambitious is this project?_

Given that pingminton has already been implemented (by me and my brother) it is not a very ambitious project.  However, the rules could definitely be defined more precisely.  Depending on how detailed we want pingminton's rules to be, this could greatly expand the time frame of this project.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This might be a good idea because, as stated above, it's a very language-focused.  It might not be a good idea because it doesn't involve any programming and would therefore probably net me a zero on the project.