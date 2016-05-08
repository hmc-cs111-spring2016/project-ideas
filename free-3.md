
# Free project 3 - Simple Bot Creator

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

The project would make automatic trolling on social media more accessible to a wider audience. It would allow anyone to create a bot on social media websites and program it with simple functionality. A language would be a good way to meet these needs because the UI could be accessible to less technologically capable users.

The idea seeks to help those who want to create [bots](https://twitter.com/phasechase) on social media but might not have the technical expertise to do so. People could currently have clever (or incredibly annoying) ideas for bots but lack the knowledge to make them. If a language could help them by making the creation of bots more accessible, they could make their ideas into reality.


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

The primary benefit of a DSL in this situation would be to simplify bot creation. It addresses the need for a tool that is usable by people who do not have programming knowledge. The DSL would basically be a graphical overlay for bot creation APIs.


### Why you?
_What excites you about this idea? How did you come up with it?_

I have tried to create bots for social media in the past and ran into various errors throughout the process. Even as someone with a computer science background, it is difficult to get a bot running. I have seen a wide variety of novelty bots ranging from clever to annoying. My idea came from the desire to see more novelty bots without all of the pain involved in creating a custom bot.

### Domain
_Describe the project's domain in five words._

Easier social media bot creation.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

I could imagine the user choosing a site and then naming their bot. They would have to go through some basic set up information in a GUI and then would have the means to define the functionality of their bot. The most basic functionality for the bot could be to post something specific in response to a key phrase or to make random posts selected from a certain data set. In the interest of starting small and gradually growing the language, the user could select from a set number of bot types and add options to customize their bot. A program would then be the framework to create the bot, including the website, the setup information for the bot, and the basic behavior of the bot. This is a simpler (if not more limited) way to interact with the problem domain, which is suitable for the targeted user.


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, the bot would be created and it would begin to operate. Since this is a long and involved process, it could be better to split the program between bot creation and operation. The user could get errors if the bot was not created, which could be translated from the website's error messages into simple instructions for the user. Other errors that could occur involve the bot not functioning properly within the domain of the website (e.g. trying to post things longer than 140 characters on Twitter). This could be detected while the user "programs" the bot and display error messages. The developer would also need to make it easy for the user to run their bot, which would involve keeping it running on their computer or figuring out another solution with few complications for the user.


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to create a bot for a specific social media site with little effort on the user side. Users should be able to customize their bots to deal with different types of functionality, though it should be difficult to go beyond basic commands without intentional effort. In the language, it should be impossible to create a bot for unsupported social networks. It should be very difficult, if not impossible, to create a bot for multiple social networks at once due to conflicts between different bot creation APIs. 


### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

[MonsterSocial](http://monstersocial.net/) is a service that exists to manage repetitive social media tasks. However, it covers a wider domain than this idea. In some ways, it is good because it provides the user with a wider variety of functionality. However, it may get overwhelming for the user, especially if they have limited technical experience. I think that the language could do a better job of explaining itself and not overwhelming the user with too many options.


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I think that a decent amount of the project would involve translating between the various social media bot API services and the GUI of this language. That could involve a direction translation with many similar functions or it could involve clever software design and a lot of pattern matching. Depending on the implementation, the time allocations for the project could vary. The similarities between different social media APIs would determine how much of the project would involve writing functions specific to one type of bot.


### Scope
_How big an idea is this? How ambitious is this project?_

This project has the potential to scale out of control very quickly. It would be easiest to start with one social network and gradually add more. At this level, it's a fairly ambitious project but not too overwhelming. It would allow the developer to become familiar with bot creation and make a lot of decisions about user accessibility.


### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This would be a good idea for a project because it very good experience in considering the user. It would also cut down the time to create simple bots. On the flip side, it would cut down the time to create simple bots. The moral complications of this project are that the developer must live with the knowledge that they have introduced many terrible and annoying bots to the Internet.

