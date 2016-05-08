# Free project 1

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

I originally thought of this idea over a year ago. While I have previously 
made some effort with a few friends to make this idea a reality, a majority
of the work, especially the design and implementation of the DSL, remains
completedly untouched beyond a few inital thought experiements.

This idea, which I was calling Binary Star, involves a video game where
the player controls an increasingly large fleet of space ships through a
variety of missions. The interesting catch is that the only way to
control a ship is through a DSL coding interface. Although plans included
different types of ships having coding styles (i.e. human ships being a
controlled with something similar to C, Python, or JavaScript while various
alien ships might use derivatives of Lisp or heavily parallel language,
like Go), for the context of this course's project, only one of these should
reasonably be targeted.

Thus, this project targets meeting a need for expressiveness in the context of
a video game. This means this language should be helping those who play the
game express their controls. Although the game I envision is closest related to
a genre of games called real time strategy (RTS), my thoughts are that by
exposing a programming interface to players, a gamer can theoretically control
more ships through careful coding than otherwise through the conventional 
controls of a mouse and keyboard.

Currently, although professional RTS gamers have impressive control over their
units using only a mouse and keyboard, as seen in
[this Starcraft video demonstration](https://www.youtube.com/watch?v=YbpCLqryN-Q),
this type of game play is only achievable after countless hours of practice.
Furthermore, the game is balanced around a theoretical limit of human control.
For instance, in Starcraft II it is common knowledge that 66 Terran Siege Tanks
will defeat 800 Zerglings if charged blindly into the enemy, as shown in
[this video](https://www.youtube.com/watch?v=SS6totiGZik) -- please ignore the
voices and low frame rate. That being said, modders, using bots superhuman CPU
reaction times, have shown that it is possible for 100 Zerglings to defeat
20 Terran Siege Tanks if individually controlled with enough persision, as
seen in [this video](https://www.youtube.com/watch?v=IKVFZ28ybQs). Although
tools to script commands do exist, they are usually done by programmers after
the fact for fun and are not core functions of the game. In fact, most games
would consider any kind of computer aided control tool to be a form of cheating
since it provides users with an unfair advantage. This advantage is made very
clear in
[this comparison video](https://www.youtube.com/watch?v=DXUOWXidcY0)
between a top tier professional player and a bot designed to do the same task.

Furthermore, although compititions exist to design AIs to play the games,
one such is UC Berkeley's "Berkeley Overmind" (as seen in 
[this video](https://www.youtube.com/watch?v=fWtpTu9gB20)) which plays
Starcraft with a superhuman average actions per minute (APM) of 3397 and a
peak performance over 7000 APM, no game to my knowledge incorperates coding
natively for fine grained unit control.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

Since this language aims to allow gamers to control units beyond the bounds of
a typical human reaction time, there must be some coding interface to allow
users to express their desired behaviors in game. Thus, by allowing users
to express a controls in code form, they can be sped up to superhuman speeds.

### Why you?
_What excites you about this idea? How did you come up with it?_

Although this concept makes for an interesting game idea, the real reason I
am excited about designing this game is because of its educational value. I
started playing Starcraft back in 4th grade and its modding tools 
were my original introduction to programming. Although this game should be
ideally enjoyable to all programmers, I imagine if the levels are designed
well with a good progression in difficult, this game could be used to introduce
completely novice programmers to coding. I've always been amazed with how
even the most monotonous tasks can be made "fun" in the context of a video
game by occasionally adding some flashing lights and a "level-up" screen.
Although I personally think programming is fun to begin with, I think by
wrapping core coding skills within a enteraining game will help coding
become more accessable to gamers.

### Domain
_Describe the project's domain in five words._

Hardcore gamers teach novice programming.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

As mentioned above, I planned to implement a number of "languages" in the game.
Originally, I thought making a language that resembled C, Python,
or JavaScript would be the most "useful" to students since a majority of
introductory programming classes start with these languages. That being said,
I have also seen languages like
[Scratch](https://scratch.mit.edu/) and
[Blockly](https://developers.google.com/blockly/) which are more targeted
towards novice coders. In reality, any of these will work and I will probably
implement some varient of them all.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, it is interpreted by the game and executed. Thus, the
program interacts with the user by carrying out their commands in game. If an
error occurs in the code, in addition to providing users with a typical error
message, it would be awesome if a character in the game says something to the
player like, "Ahh, our onboard computer just segfaulted! Take a look at this
line of code!" This creates an more personal relationship with the code and
also adds to the immersive experience. Ideally, we want the users to forget
they are learning to code!


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to issue commands to ships and provide reactive decision
making based on a variety of "onboard sensors." Although it might be useful
to allow the game to output debugging data to files for the player (especially
when the code gets more complex), game should have a very restricted
interactions with the overall file system. There should not be any way to
create a program that would be harmful to the overall computer system the
game is running on.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

As mentioned above, scripting languages inside game engines as development
tools but generally do not exist natively within the game. Additionally,
things like the Berkeley Overmind are built upon third party APIs like
Starcraft's Brood War API ([bwapi](https://github.com/bwapi/bwapi)).

In terms of educational coding, languages and interfaces such as
[Scratch](https://scratch.mit.edu/) and
[Blockly](https://developers.google.com/blockly/) do exist, but these
are made to closer resemble a general purpose language for novices.
Similarly, Prof Lewis has introduced me to an educational CS game called
[The Foos](http://thefoos.com/), which while very cool, is 
undoubtedly targeted towards a younger audiance.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

If I was starting from complete scratch, the game design aspects of this
project would eat up a solid amount of time. That being said, since I have
started this project some time ago, I already have a lot of ideas and 
beta code for displaying grpahics, getting input, etc. At this point,
although I will still need to work on how the parsed DSL is interpreted
within the game environment, a lot of the typical game aspects have been coded.
Because of this, I think a vast majority of my time will be spent directly
engaging with the language aspects of this project.

### Scope
_How big an idea is this? How ambitious is this project?_

The overall scoping of this game is far to ambitious for a CS111 project. In
fact, after I graduate, I plan to see this idea to some type of completion and
would like to even distribute it. That being said, I think by looking at this
project as a way to develop a prototype of some early tutorial levels will
make it a very reasonable project.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This project might be a good idea because I am essentially developing an entire
external DSL from scratch that will be interpreted by game code! I will
certainly learn a lot by undertaking this project plus I'm super excited
about it.

On this other hand, this project might not be a good idea because it is certain
on the larger project that is likely too ambitious even if carefully scoped.