# Free project 3

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

Many programmers, especially novus programmers struggle to debug their code. They read the error message, but the only part the understand is that it means there code wont work. Especially for novus programmers, this can be an intensely frusterating process, they may only be missing a semicolon, of have used a ')' instead of '}' but they have dumb and inept, like computer science is something only "those smart people" can do. I would like to make a programming language that could be used along with existing programming language but would make the debugging process easier for programmers, by providing more easily understandable error messages with suggestions for what might be the problem.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

Error messages often seem like an entirely new language to new programmers, they seem impossibly to understand and are therefore useless to them, if I created a DSL to address this specific need, it would act as an interpreter for the person, translating the language of error messages into human readable English. The domain is limited to debugging and error messages so it does not require a GPL but the complexity of the input error messages and interpretation needed require an entire language to solve the problem, so a DSL is the appropriate tool.

### Why you?
_What excites you about this idea? How did you come up with it?_

In CS105, we are currently learning how to debug by looking at the assembly code and at the information we can glean from gdb, but it is an often frusterateing process as much of the error messages seem unnecessarily vague and complicated. I have been coding for the past 4-5 years and if I am still struggling with it, surely there must be something that would make this better and more accessible to new programmers.

### Domain
_Describe the project's domain in five words._

Compiler error message translation to English.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

If the user gets an error message they don't understand they should be able to run a command like "interpret" which will attempt to translate the error into clearer English. Or "suggestions" which would output probably causes for the error. This would allow users to use this tool alongside the languages they are learning as a helper for when they get stuck and can't figure out what is wrong with their code. This will decrease overhead, because my language will only be used when it is actually needed and the commands will be straight forward and easy to remember.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When the program in my language runs, it will read in the error message from the users program, pick out the relevant information for the user and print it out in full sentences for the user alonge with suggestions for what might be causing the error. An error could occur of my language does not recognize the error message output by the program, but in general my language would do all its work in the error domain.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to get more information about the error, where it occured, likely reasons for its occurance, and clear, full sentences in English explaining the problem like a human tutor might. It should be impossibly to write programs in it that don't involve error checking.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There do not seem to be any DSLs which quite do this. There are many debuggers like valgrind and gdb listed [here](https://en.wikipedia.org/wiki/Debugger) but they seemed to be geared towards very "technical" people, who are creating huge code bases that are very difficult to debug and therefore need the detail these dubuggers provide. None of these seem to focus on easing new coders into debugging, perhaps because most new coders learn in a setting like college where there are tutors who can help them or they just google the error. These tools were therefore mostly created by programmers working for big technical companies to be used on the sorts of projects they use and less to be used on "simply" things.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

This language would have very few things the user would need to write and most of the language writers time would be spent working on the back end to ensure that error messages were being correctly reinterpretted for the user.

### Scope
_How big an idea is this? How ambitious is this project?_

This seems like a very big idea, but also a very intersting one. Tools like valgrind and gdb seem useful, but like the learning curve is extremely high. I would like to lower that learning curve but I would guess that it would take much longer than we have to do it well.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This would be a good idea because it seems very useful but it may just be too ambitious for the amount of tiem we have to create our DSL and might require to much background work and to little actual language developement for the user.


