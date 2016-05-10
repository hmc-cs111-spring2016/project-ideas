# Free project 1

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

I don't know if "need" is the right word, but this DSL would let people (programmers or otherwise) make text adventure games. The current experience involves using a general-purpose programming language, or a DSL or other development system that already exists for this purpose. For the most part using the systems designed for this purpose saves time and effort, specialized as they are. While they are reasonably effective, the ones I've seen are English-heavy, very C-like, or not a
language. As I'll say below, the English-heavy one I have in mind actually seems pretty effective as it is, but C-like syntax can be prohibitive to non-programmers, and the non-language system is slower to use, as such things are. In any case, with the project I have in mind, users would have an option similar to the English-heavy language, but less English-heavy. If we've been on the right track in our class discussions, this could reduce user frustration over syntax
errors.


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A library could certainly do the same job, but a DSL would be more accessible to people who aren't that familiar with programming in general. Also, it would be nice to make the DSL look declarative even if semantically it isn't, for reasons I've discussed in various places in this response.


### Why you?
_What excites you about this idea? How did you come up with it?_

I really like games in general, and I think it's unfortunate that people don't really make text adventures anymore. I had fun making one in CS60, but using Prolog was... less than ideal. In some respects, though, even that was easier to work with than I sort of imagine using Java or C++ or even Python would be; I think the declarative style is very well suited to making text adventures.


### Domain
_Describe the project's domain in five words._

It makes text adventure games.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

Generally speaking, the user would describe the layout of the world, what is in it and where, and what actions the player is allowed to take. I conjecture (based entirely upon my own intuition) that many people would find it easier to create a world by describing it and letting the computer do the rest rather than by telling the computer how to set everything up. I would want to ask as many people as possible whether this is true for them before actually committing to this
design decision. I do expect it to be true, though, because what I just described is pretty much exactly how normal (non-interactive) fiction works.


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

The person interacting with the language might not be the person interacting with the program itself. In any case, whoever is using the program plays the text adventure, typing at a command line sort of thing in the usual style for a text adventure. I think it might be best for this DSL to be compiled so that any actual errors in the code could be communicated to the writer at compile time. Any errors that would occur at runtime would be the result of the player trying to do something
they're not allowed to do. The program could tell the player that it doesn't recognize a particular word they used in their command, because "I don't know what that means," while traditional, isn't very helpful.


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to place a bunch of rooms in a world and specify their relation to each other. It should be easy to set the player's starting location. It should be easy to create items that the player can pick up. It should be easy to specify what a player can do with an item (either as a property of the item or as a property of something else that interacts with the item). I think it should be impossible to define new data types, which would mean that items and the like would need
to be instances of already-defined data types. I'll add a caveat that it should only be impossible if this is implemented as an internal DSL; if it's external, it should just be difficult to do so to encourage users to work within the language but allow for functionality that the language doesn't have but maybe should.


### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There's one very extensive DSL that I found called [Inform](inform7.com). The newest version, Inform 7, is very heavily English-based, but at the same time having looked at examples it looks at least a little easier to write in than AppleScript. I suspect this is for a few reasons, for one because Inform's domain is interactive fiction. I think another significant part is that the English largely takes the form of complete declarative sentences. Just the same, I think it could be
useful to create a similiar if less extensive language that is less based on English. If nothing else that give potential users more options.


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I'm not really sure how much time would be spent on each. Certainly trying to strike the right balance between English-heavy and English-deficient would be a significant portion of the project. I guess what I mean is the language design portions would be the most important part, but might or might not take the most time.

### Scope
_How big an idea is this? How ambitious is this project?_

If I were trying to completely replicate Inform, this would be way too huge. I imagine though that just basic functionality and language elements is within the scope of the class, and it would still be possible to write a text adventure with just those.


### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This could be a really good opportunity to engage with some of the ideas we've talked about with regard to language design (the role of natural language for example). On the other hand as I've said already I'm not really sure exactly how much _time_ would be spent on each portion of the project.
