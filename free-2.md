# Free project 2


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

A lot of hardware design is done via hardware description languages (HDLs). While this is preferable to designing the logic yourself, HDLs are notoriously bad to work with and are about as intuitive as using C. It would be nice if we could make a DSL for generating hardware designs (or at least for generating HDL code). This could help hardware designers avoid some of the issues with working with HDLs and make their lives easier.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

HDLs are already on the verge of a DSL themselves. While they need to be Turing complete as they need to build all kinds of hardware, they fairly deterministically convert certain expressions into certain logical elements. This feature is pretty DSL-y as well as the fact that the intended output is actually hardware instead of some kind of data value or file like in GPPLs. However, as stated earlier, HDLs don't do a very good job. Thus, it could be nice to create a new DSL that allows programmers to focus on what's being done or on the logical elements being created instead of doing this dance of writing code in a form that gets the compiler to do what you want with the hardware you want.

### Why you?
_What excites you about this idea? How did you come up with it?_

There's actually a huge amount of room for improvement in HDLs, so this could actually make a big impact on how easy it is to work with them. Plus, I know a lot of people who would like something like this.

The idea for this DSL just popped into my head while trying to think of DSL ideas.

### Domain
_Describe the project's domain in five words._

Better / easier hardware description.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user would interact with the language by writing code to manipulate bits and arrays of bits using logic. So, they should be able to XOR two arrays of bits together, take the AND of a bit array, or invert the value of a single bit. Depending on how the interface goes, users may have to work by specifying low-level components (kind of like the ones above) or they may be able to do fairly high-level operations on data (like reversing an array of bits). By making it more transparant which components are being created, it makes it easier to understand what the language is creating. Also, having lots of handy operations built-in to the language is nice and cuts down on having to rewrite code (there are "functions" in HDLs, but calling them can be more pain than it's worth).

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, either a hardware design will be generated or code for a hardware design in a HDL will be generated. There isn't much interaction between the program and user except for telling the user they made a basic error (like they misspelled something).

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should hopefully be easy to get a better idea of the underlying hardware that will be generated. It should also be easy to work at a higher level by having functions like bit reversals and objects like state machines built-in. Ideally, it should be possible to do everything you could in a HDL, though doing some things may take longer in some cases. Anything other than generating hardware designs / descriptions should be impossible.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are HDLs like SystemVerilog HDL, but they are what this DSL is trying to help replace. I did find some more interesting HDLs, though. For example, a few people created [a way to make hardware designs in Haskell](http://www.cse.chalmers.se/edu/year/2012/course/TDA956/Papers/Lava98.pdf) of all languages. While this is interesting, I'm not sure how many people want to work with Haskell's syntax while also trying to design hardware. Although, you can use Haskell with an interpreter, which is nice. I think it would probably be better to use syntax that is more appropriate for the task at hand and Haskell wasn't exactly meant to be pushed to be used in this strange way.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

Perhaps surprisingly, language will be a big part of this project. For the system aspect, the language can be "translated" into HDL code, which should be fairly straightforward if you know what your doing. This will definitely be the case when high-level components are simply just cookie-cutter code in the HDL.

### Scope
_How big an idea is this? How ambitious is this project?_

To fully support all the possibilities built in to a HDL would probably be pretty overwhelming. It might be easier to stick to the basics and make sure you can do that really well. That way it could at least be a language for beginners.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

There is definitely a need for a better HDL and this would be a good way to start. If successful, a project like this could save so many people's time. However, there are going to be a lot of hard decisions to make about the language and it will be tricky to support a lot of advanced HDL features. Automating stuff like state machines could turn into it's own DSL as they are so complicated.