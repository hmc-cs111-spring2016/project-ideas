# No computer project


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.



### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

The basis for this language is West Coast Swing (ex: https://youtu.be/QiB-xYd9PSo?t=30), 
a type of social dancing with specific rules and technique. This can be explained as a 
DSL by translating those rules into a specific wording that results in particular steps 
done in a certain way. This helps anyone who wants to dance West Coast Swing to break down 
the movements. This is more aimed at beginner level dancers than advanced
dancers who have master most of the movement. By having this broken down as a
language, it can help beginning dancers organize the different movements they
have available to them and when it is appropriate to use them.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate because of the strict nature of West Coast Swing technique.
Unlike other social dances, the vocabulary of movement has more definition
and expectations as to how it's executed, especially at a competition level. 
Understanding and remembering all of the different pieces (and what is acceptable
when) can be a lot to manage at the beginner level. By understanding this information
as a language, it can be easier understood and manipulated.

### Why you?
_What excites you about this idea? How did you come up with it?_

I've been dancing west coast swing for a while, and I still feel a bit of thrill
when dancing it or watching it. I came up with this by trying to think of everday
activities that have specific rules to them, and this came to mind.

### Domain
_Describe the project's domain in five words._

West Coast Swing, partner dancing.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user interacts with this language through dancing, either by practicing
on their own or by dancing with a partner. Programming looks like the set of
moves they plan to execute or a choreographed routine. It can also look like
a combination they are practicing. This is a good way to start picking up the
basics of a dance--by learning premade sets--so this would be a useful way to 
begin learning west coast swing.


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, a dance happens. The program interacts with the user in 
that the user has to physically carry it out. Errors include not remembering
the steps, not following the basic rythym, not being on time, stepping on 
your partner's feet, etc. Usually, an outside observer can make note of these.
Users can also videotape themselves dancing to see the mistakes that they make.


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

Executing a sequence of west coast moves should be possible in this language.
Given the direction of momentum required to execute some of these movements
must be provided by the previous movement, some movements may not flow very
naturally together. Dancing tango should be impossible.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

I did once see a friend make a turing machine to describe the different moves
he could switch between. Otherwise, I don't know of any other West Coast Swing
DSLS, as there is no subset to WCS. However, one could argue that social 
dancing in general is a DSL, and that WCS is a subset of that. Examples of
other social dances include Lindy (https://www.youtube.com/watch?v=v9xxeWRxSbA), 
blues (https://www.youtube.com/watch?v=-m0V2Zq-Qf4), and Salsa
(https://www.youtube.com/watch?v=3nd8WQy58Pw).

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

The implementation is definitely the harder part--learning WCS is not easy.
All of the basic design already exists. There's room to add advanced styling
and movements, but this would not happen at a beginner level. As such, all
the work lies in actually executing a program.


### Scope
_How big an idea is this? How ambitious is this project?_

This project is only as ambitious as the number of moves included. The basic
steps and the few normal variations would not be complicated to write and to 
determine which can follow which. However, once more complex variations and 
movements are introduce, the rules of the language become more complicated.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

West Coast Swing has lots of room for rules and precision which makes it suitable
as a DSL. It also has a basic rythym that is necessary for the dance to be considered
WCS, which translates to the idea of a basic grammar. However, there's not a lot of 
room to be creative and create new ideas in this language, which makes it more
limited as a project.

