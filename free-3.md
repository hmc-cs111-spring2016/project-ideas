# Free project 3

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This DSL would help anyone manage their time better. As of right now, the current means of time planning is a static calendar. However, this has a lot of disadvantages as it can be hard to tell which plans are flexible (like homework) and which are not. By using a DSL to add and remove events from a calandar, the computer can explore options, detect user patterns, and help make suggestions for when to schedule / reschedule events.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

Time scheduling is a very specific domain that has its own nouns and verbs. A DSL would allow users to focus on the time planning aspect and allow for a lot of interaction optimizations that would not be possible at all in a general purpose language.

### Why you?
_What excites you about this idea? How did you come up with it?_

There are a lot of features that could really make this useful to people and a lot of room for predictive suggestions. I may have come up with this idea while looking at my own calendar.

### Domain
_Describe the project's domain in five words._

Flexible event planning and scheduling.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user would interact via an interpreted interface. They can view currently scheduled events, attempt to schedule an event, or remove an event. Attempting to add an event that overlaps with another wouldn't necessarily fail as the DSL could potentially reschedule more flexible events to make room. The DSL could also support deadlines and work with the user to find the best time to get the work done, so long as it happens before the deadline. This could allow an unprecendented level of interactivity in the scheduling process.


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When the program runs, it waits for the user to request information from it or to change the schedule. The program could also run in the background to alert the user to events and monitor how long it takes them to start working on work with deadlines. Errors could include trying to schedule an event during an immovable event or during a time when there are too many nearby deadlines.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to use the DSL for basic scheduling and for managing deadlines. It should also be possible to move / delay certain types of events and restructure the user's schedule. It should be difficult / impossible to do non-scheduling tasks (besides setting reminders and stuff related to scheduling events).

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are definitely a lot of calendar apps out there, some of which support more advanced scheduling features. However, many do not have this kind of flexibility and are not interactive. I think there is / was a CS research project related to an app that helped users plan their time kind of like this, but I don't know how far it got. Prediction will be key to really making something better than before, though. If this DSL could find how long it takes you to start and do homework, it could change its suggestions about when to start working on it appropriately.

Also, I found out that apparently my idea isn't completely original: [a related idea](https://github.com/aputman/project/blob/master/documents/final.md) was implemented for a DSLs final project pretty recently.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

To just do a really basic time scheduling DSL, most of the time spent will probably be on the interface. However, more advanced features may take a lot of time to implement, especially finding how to move events to make room for new ones and predicting good start times for meeting deadlines.

### Scope
_How big an idea is this? How ambitious is this project?_

This is a pretty big idea, but doing it on a basic level should be reasonable. It might be good for people who have a background in AI and want to apply some ML techniques.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

I think this is a really cool idea and it could really impact people's lives, especially if it had a good interface. However, this also has the potential to get out of control. Making predictions is hard and the user experience may depend on doing it well.