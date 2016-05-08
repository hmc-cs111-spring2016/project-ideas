# No computer project


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

The game has a Wikipedia page at <https://en.wikipedia.org/wiki/Mafia_(party_game)>.

Mafia (also known as Werewolf) is a game which, at its core, is a fight between an informed minority of players (the mafia), and an uninformed majority (the town). The town have to try to figure out who the mafia are and eliminate them, and the mafia have to avoid being figured out. The game alternates between day and night phases. During the day, everyone votes on someone to kill, with the town hoping to kill a mafia member and the mafia hoping to avoid scrutiny. During the night, the mafia get to choose someone to kill, and other abilities can also be used.

It's a great game for people who enjoy that kind of trying to find hidden motivations. It's a very psychological game where town members have to try to figure out who would do what if they were mafia, and the mafia have to figure out what the town will be looking for in them.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

In mafia, besides alignment, players often have roles or abilities. For instance, the town might have a cop who gets to investigate players to see if they're mafia, or a tracker who can pick a player and see who they targeted that night. The mafia might have roles like a rolecop, who can target a member of the town to see what their ability is. Many of these roles can come with modifications, such as one-shot, which means that the ability can only be used once over the course of the game. These specific pieces of terminology essentially form a language.

At <http://wiki.mafiascum.net/index.php?title=Category:Roles_Main_Page>, you can see a small sampling of the roles that have been created for mafia. The way that all of these roles interact with each other to produce a game is tantamount to the functioning of a DSL.

### Why you?
_What excites you about this idea? How did you come up with it?_

I play mafia a lot and have for many years (I wrote my common app college entrance essay on the game) so I'm very familiar with all of the intricacies of the game, and it strikes me as very much like a DSL.

### Domain
_Describe the project's domain in five words._

A psychological player-elimination game.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

There are essentially two kinds of users.

* The designer can design a setup by choosing from these different roles and alignments and assigning what will be in the setup. They can design a very plain setup with very few roles that have abilities, or they might design something crazy where everyone has a power.
* The players each have a role and get to interact with the language in a number of ways. They can vote during the day, they can kill at night if they're in the mafia, and they can use their other abilities whenever applicable. The language responds in a couple of ways. It can respond by changing the internal model of the game (i.e., by changing a player from being alive to being dead). It can also respond by relaying information to the player (i.e., if a player is a cop and investigates someone, the language may respond by telling them that their target is in the mafia.)

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

Apart from those two kinds of users, there is typically a moderator who pulls the strings on how the game works and makes sure that everything is functioning as it should. This moderator takes the place of a computer. When a program (a game of mafia) runs (is played), the players are essentially each given an interface whereby they can do everything they are entitled to do: talk with other players and vote on who to kill during the day, and pick who to kill as mafia or carry out other actions at night. The moderator makes it so that all of these actions modify the model of the current game state and make sure that the game is up-to-date, checks if a side has won, and so on.

The program interacts with the user as I already said (by changing the game state or giving them information). There are a number of errors that could occur. For instance, a player could try to vote for another player who has already died; a mafia member might try to kill another mafia member at night; a cop might try to target two different players. These are relayed to the user by the moderator who tells them that what they've done is illegal, and that they must choose some different action. 

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

As a player, this is straightforward: it is easy and possible to carry out the actions that you are allowed to do, and impossible to do anything else. Or more broadly it's difficult to figure out the correct action to take, because the game has a lot of hidden information.

As a setup designer, it's easy to design a creative setup because there are so many different roles that have been created and added to the language. It is difficult to make a setup fair; that is, to make a setup that the town and mafia have a roughly equal chance of winning. There has been a lot of debate over how to make setups that are balanced. Another thing that's difficult but possible is designing more creative setups that don't just use that laundry list of roles. Many setups have been designed that use other mechanics, like allowing players to transfer their vote to another player when they die, thus making that other player more powerful. It's impossible (in a sense) to design an illegal setup, like one that starts with more mafia members than town members without some other strange mechanic.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are many other social hidden information games, and many also take the form of an informed minority against an uninformed majority. For example, The Resistance (<https://en.wikipedia.org/wiki/The_Resistance_(game)>) is a similar game with fewer possibilities for complex setup design, and without player elimination (i.e., all players play until the end of the game). One Night Ultimate Werewolf (<https://boardgamegeek.com/boardgame/147949/one-night-ultimate-werewolf>) is a very similar game which only lasts one night and one day. There are tons of different games and they all offer different modes of gameplay, but few have been developed as languages to the point of mafia. Mafia has so many different roles and modifiers, and generally more room for creativity in design. There are also many setups out there that have been designed to learn from (which sort of function as a code base).

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I don't think this is applicable.

### Scope
_How big an idea is this? How ambitious is this project?_

Again, not applicable but the language has been developed very thoroughly. It was invented as a sort of psychological teaching tool, and has evolved to become much larger than that.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

It isn't an idea for a project.
