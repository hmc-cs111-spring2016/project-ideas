# Free project 1


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This DSL would have two main user bases: people who play DOTA 2, and people who are trying to develop and test new heroes (characters in the game) and items for the game. Ideally, the second group would be a subset of the first group, since to use the tool would require a good amount of knowledge of the game. The idea is to provide an text interface with very low overhead to allow people to test different hero/item combinations, givng stats like damage potential, tankiness, disable duration, etc for these combinations, as well as allowing people to test new heroes/items in the same way. 

I think a language is the best way to accomplish this, as there is already a GUI for it (namely, the game itself in practice mode), but its very slow. To test things, you need to start up the game, and try a bunch of different things, all of which take time. If there were a text interface, you could save an item combination, then just loop over the heroes you want to test and produce output for all of them instantly. Further, if there were a way to save a test set (for example, damage at X level, pushing power, mana usage, farming speed) one could do mass testing using these, without having to worry about forgetting anything. Additionally, having a text interface would let you run this while in game, if there's a quick thing you need to check (you could even pause the game, check something, then unpause).

DOTA 2 is a very, very hard game. There are 120+ heroes to learn, all with 4+ unique abilities, and over 100 items. As a result, when making balance changes, there are millions of interactions between abilities and items that contribute to its balance, so having a test suite of things to check (like, X hero should do more damage but have less health than Y hero) would help the developers of the game a lot to make sure that a new change doesn't mess things up. To be fair, I'm not sure what their current process looks like, its entirely possible that they already have something like this, but this would help the community be more involved, and have more informed debates about changes. 

Additionally, to just the average user, this could be a great learning tool. If you want to learn how strong a certain hero is against another hero, you could use this to run damage calculations. You could also use this to test different builds (like, if I get X item before Y item, I'll farm faster but be easier to kill). As of now, the way to do this is literally just to play the game. You test different item builds, and try them in the game, most of the time leading to your death as you learn what things work and don't work. This could simoplify that process. 

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_
As described above, the need is essentially to provide an interface that lets people test ideas in DOTA 2 quickly and easily. A GUI could work for this, but would effectively just be a GUI on top of a language that's doing all the backend computations. Thus, a first step is to make a DSL for it. Additionally, the language does not need to be turing complete, it can focus entirely on its domain. It might have batch testing and things that make use of more elaborate control flow, but these should all be in the backend. The goal is to make the interface as simple to use as possible. 

### Why you?
_What excites you about this idea? How did you come up with it?_

I'm excited about this first and foremost because I play the game, and think it would be awesome to have something like this. I also know lots of people who play the game as well, and would love this. Second, it would be very helpful with respect to the constant debates about things in the game that are always hard to fact-check due to the difficulty of testing these things. I came up with it just by thinking of an interesting domain, and immediately thought of DOTA 2. 

### Domain
_Describe the project's domain in five words._

DOTA Hero/Item Balance Testing

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user would interact with this language just by writing scripts in either the shell, or a text editor. I'm imagining commands like:
Hero {item1, item2, item3, item4, item5, item6} level 15;
printing out the relevant stats for that hero. The core issue seems to be text or GUI as the core interaction. I claim that text is probably faster, as you could much mroe easily copy and paste the same 6 items into different heroes, rather than having to reselect everything every time. Text makes things like standard batch testing much easier than a GUI on its own.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

I sort of answered this with the section above, but the core idea is that you input some data:
Hero (items) (level) (buffs/debuffs)
and get as output some stats. You can then combine these things however you want (ie Hero1 damage > hero2 damage)
or (at what level is Hero1 health > hero2 health). Finally, you could create a new hero, where you could input all of its base stats and abilities, and then treat it like a hero in the game already.

Errors would generally just occur if the user inputs something that doesn't exist in the game (like giving a hero an item that doesn't exist).

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

The most important thing to be easy in the language is to specify discrete combinations of heroes and items in DOTA 2 and compare their stats in various ways. Second, it should be relatively easy to make changes to the hypothetical game, and see how those change these interactions. 

It should be possible, but probably difficult to use this to make predictions or serve as a guide for what to do. There are too many factors at play to be able to reccomend things to the player, but if the user were to define some important features, then it should be possible to find builds/heroes that maximize those features, so it should be technically possible.

Impossible things should be anything unrelated to the game.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

To be completely honest, if this thing exists, I would have heard about it. I follow the dota2 reddit, so if there was a community accessible tester for the game, either as a DSL or a GUI, I'd know. Its possible that one exists for developers of the game, but it would be internal, so of no use to the general population.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I think the time spent would be evenly split between figuring out how to make this into a comprehensive language, and doing user studies to figure out what's important to people that's also feasible to calculate outside of the game. The actual calculations the game uses are fairly well-known, so its pretty clear how to make the backend work. However, there would be a good amount of time spent inputting all of the data for the existing heroes, but it would be a one-time setup cost, not a thing to continue devloping over time. 

### Scope
_How big an idea is this? How ambitious is this project?_

I think its fairly ambitious. There's a lot of raw data I'd need to collect, as well as a bunch of research that would go into the backend, and the frontend needs to be very, very user-friendly for the average person to be willing to learn it. However, all of this seems very doable, there's nothing in it thats like "wow, I actually don't know how I would do that". Its just a lot of work to be done. 

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This would be a very useful tool for a very specific domain. Also, while its a lot of work to input the basic data for the backend, it would also be very easy to just set it up for a subset of the heroes/items. The language could be developed modularly, starting with some data and some output (like just hero damage at first), and then the implementation could grow naturally over time.

However, the domain is possibly too specific. The majority of people don't know DOTA 2, and of the people who do, many just play it casually, so wouldn't care too much about something thats intended to make them better at the game. There's also a large amount of data that needs to get collected for the thing to even work. 

