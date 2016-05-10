# Free project 3

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

Many students in CS70 are frusterated by the makeFiles the use to compile and run their code with all the correct dependencies. They may spend hours debugging trying to find what is wrong with their program, when really its just an issue with the makeFile. I would like to make a tool like sbt that works for C++ instead. This would recognize when a dependent file was updated and saved and then recompile and run. This language would be clearer and simpler to use, allowing students to focus their time and energy on their actual C++ code and make the debugging process faster and easier by allow them to make minor changes to their code, save, and then have everything automatically recompile and run.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate for the same reasons that the DSL sbt is appropriate for making Scala programs easier to debug and rerun. This is an small, frequently used domain in which intuitive commands are needed to compile and run the C++ programs with all the right dependencies but there is not yet an easy to use tool.

### Why you?
_What excites you about this idea? How did you come up with it?_

When Prof. Ben showed us sbt in class when he introduced Scala, my first thought was "Oh, why didn't we have this in CS70, this is so much easier than how we did it" as soon as someone asked if this was one of the DSLs hidden in the presentation, I realized that it was and that I could perhaps make a useful tool like that which would ease the frusteration of the CS70 students following in my footsteps. I love the practicality of this idea.

### Domain
_Describe the project's domain in five words._

Simple build system for C++.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

I would like to allow the user to simply type a short command into the commandLine and then have the program check for dependencies, newly saved file changes or errors, compile, and run the program. My users should be able to use only one or two broad commands to create a "large" program in which the compiler is executing quite a bit of code. Most build automation software is used in a similar way, so it would be easy for my users to adapt to using my language.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, the parser will read in the short, specific command the user typed and the execute a series of commands to check for updates, then check for dependencies, then compile the code and then run it. An error could happen at any point and it would need to be able to clearly communicate the error to the user.Error handling and messages would be a large part of this language. It will need to let the user know if it cannot compile, is missing a dependency, or something else is wrong with the code it is trying to run.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy for the user to simply state a broad, abstract command like "run" without having to specify all the details of what to run, and what to update or what dependencies to use. It should be easy for the user to read error messages and pinpoint the location of the problem in their code. It should be difficult for the user to interfere with the low level details of how everything is being compiled and run, because my language would attempt to abstract that for them. It should be impossible to use this language alone, it can only be used to run other programs.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There seem to be quite a few languages which have been built to help with compiling and running programs in various languages. There is a wikipedia page [here](https://en.wikipedia.org/wiki/List_of_build_automation_software) with a long list of them. However, when I searched for something like sbt, I found many threads of discontent people, who had tried using something like CMake and been frusterated by it. Many of them asking if there was anything more like sbt that could be used for C++. I  found [this](https://groups.google.com/forum/#!topic/simple-build-tool/xcwTZUvVJdo) email chain of people who are already looking into expanding sbt itself to work with C++ and [this](https://github.com/d40cht/sbt-cpp) which is "a cross-platform native build system" that someone else made to address this problem, but which does not yet appear to have a very large user base.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

If someone were to work on this project, each command they created would require quite a bit of programming in the host language to ensure that it worked correctly. Since there are already quite a few tools out there, it would also make the most sense for them to spend time looking at existing tools and then determining how to best subvert them to use for C++, so more of their time would probably be spent on things that are not directly part of the language aspects of this project.

### Scope
_How big an idea is this? How ambitious is this project?_

I could probably create a very basic version of this tool within the given time frame, but there are quite a few extensive projects that people have been working on for years in this domain, so it would be to ambitious to get very far with mine.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This would be a good idea for a project because it is a DSL with a very clear domain in which people are still unsatisfied with the tools they have and looking for new languages to expres themselves. However, it is very ambitious and would be difficult to get very far into the actual language creation within the allotted time.



