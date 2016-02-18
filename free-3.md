# Free project 3 - Poem writing helper

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

I imagine this being helpful for novice potery writers who may need help writing poems in certain formats, such as sonnets and limericks, and want various types of help in doing so. Now, the experience may be difficult for writers who have a hard time with meter or with rhyming. I imagine this DSL to suggest words to users to help them with rhyme scheme, point out overused words, and look up pronounciations of words to make sure meter and rhythm is correct.


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate because poems, and especially structured poems, are a very particular and strictly defined subset of natural language, that can be checked as long as the rules are properly described. I think it addresses the need by acting as a domain-specific spellchecker, to which inputs (which type of poem, the poem itself) can be input, and suggestions can be output.

### Why you?
_What excites you about this idea? How did you come up with it?_

I like the idea because it seems like something that could be done in a fairly straightforward way. I came up with it just thinking of DSL ideas -- it seemed like something I could do and something that would be fun to play around with.

### Domain
_Describe the project's domain in five words._

Poems with well defined structure


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

I think the user would input to the language a specific poem type, as well as a text file or string which is the poem itself. I think a text file would be logical because then the program could look for line breaks more easily. The program would then output either a list of suggestions referencing line numbers and specific words, or maybe a text file of suggestions based on the poem type, or some similar format.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

Once the program receives the desired inputs from the user, it would cross-check the poem type against existing poem types that it has. Then, it would look up each word individually against a dictionary (either something stored to a database or using Webster or something through an API). It would check :
	- that the word exists or is a proper noun
	- that the word is in the appropriate rhyme scheme
	- that meter (i.e. iambic pentameter) is observed on a word and line level

Errors would occur when poem types that don't exist are attempted, or perhaps when weird symbols are entered in a poem (though this should really be something that can be caught by the program).

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to see that poems are correctly formatted, provided the poem type and a poem. It should be possible but difficult to write non-poems or prose and run it through the checker. It should be impossible to do things like ask the language if a poem is good or something like that.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

I found [this website](http://www.howmanysyllables.com/), but it doesn't check if words are even real and only tells you how many syllables you have. For things like a sonnet, where lines have 10 syllables at most, this doesn't seem all that useful, though it does tell you syllables per line. I think there is still space for some sort of "sonnet checker" or general poem checker as this website doesn't do quite enough for me.

I found a few other syllable counters, but they all kind of do the same thing as the above website (and probably a bit worse).

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

This seems like a project that could actually have a lot of cool language design. That said, a lot of initial work would have to be done to teach or input rules of various poems to the system, and then work would have to be done on the checker, both of which seem to be substantial tasks. After that, though, all sorts of additional functionality and design options open up; would you want to maybe have the language be able to suggest rhymes, alliterations, and other thing? Maybe we would want to allow users to define a new poem type (rhyme scheme, meter, length etc) that could then be checked by the checker? It seems like possibilities abound here.

### Scope
_How big an idea is this? How ambitious is this project?_

This seems like an idea that can be implemented to be large or small, and as such seems to be appropriately ambitious. It seems largely extensible and with an MVP that is not outrageous.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

As I described in the previous section, this seems like a good idea for a project because it could be extended to include all sorts of features, but could work well with just a subset of functionality. I can't think of too too many downsides to this one -- perhaps I'm not considering potential drawbacks here... is this even a DSL, though? That may be the biggest question here.
