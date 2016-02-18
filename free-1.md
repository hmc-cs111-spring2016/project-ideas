# Free project 1

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

My idea would help physics students (or just people in general) do simulations involving some basic forces (like gravity and magnetic forces). As of right now, many physics students don't have very good access to simple simulators that they can play around with. There are some online, but they're written in Java and are very difficult to get working. This DSL would hopefully make it easy to set up simple demos and create animations of the results of the simulaiton.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

Some things are best learned through demonstration or experimentation, but not every concept in physics is easy to safely demonstrate or play with. This DSL would help make very small or very large simulations accessible to physics students, which could help them with understanding concepts they encounter in class.


### Why you?
_What excites you about this idea? How did you come up with it?_

Many years ago I actually worked on a simulation program as part of my research at the time. I also have some friends who are physics majors too. This could be another opportunity to work on such a simulation program and actually work with people who might actually use it for help / feedback.

### Domain
_Describe the project's domain in five words._

Simple physics simulations.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user would likely describe objects and their initial conditions (like velocity) in a file. This could be done in a variety of different ways, including some that we discussed in class. "Programming" would involved setting up a simulation with everything in the right place. Depending on the implementation, numerical limits may have to be considered when writing a program as it's really easy to for simulations to become unstable unless the simulation software is written well.

This language could theoretically be interpreted too. So, objects could be added or removed when the simulation is paused and the user could control how long the simulation would run before pausing again.


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, the objects in the file would be loaded and simulated according to some laws of physics. In theory, the program could have a live graphical interface in while the user could add forces or objects, but this would be a stretch. The end result (which would consist of the positions of the objects at certain timesteps) could be rendered as a video or series of pictures.


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to set up some objects with some basic properties and simulate them. Besides simulation parameters, there shouldn't be anything else you can do.


### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There's probably tons of DSLs in this domain. Physical simulations are very important in industry and acadamia, so I wouldn't be surprised if there were hundreds of various programs out on the internet. [This page](https://phet.colorado.edu/en/simulations/category/physics) alone has a massive number of standalone, free, interactive simulations (that aren't programmable). However, like I said earlier, a lot of the simple applets used in Physics classes are written in Java, which can make them hard to run. Professional simulation packages may be expensive or suffer from feature bloat (that is, it is hard to use them). [This software](http://www.comsol.com/products) looks like a good example as it supports many different kinds of simulation, but you have to contact sales just to get an idea what the price is. The proposed setup would hopefully be pretty straightforward and simple to work with.


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

This depends on their understanding of physics and how to do simulations. Most people will probably spend a lot of time implementing systems and may even not get around to adding many language aspects due to the long time to implement each.

### Scope
_How big an idea is this? How ambitious is this project?_

Pretty ambitious. It would be recommended to target a small domain within physics and do that well rather than trying to support everything.


### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This would be a cool way to learn about or refresh your knowledge of physics and work on simulating stuff, which is cool. Unfortunately, there's a lot that would need to be accomplished that requires a wide variety of knowledge, so there's a lot to learn and a lot of potential complications that could come up.