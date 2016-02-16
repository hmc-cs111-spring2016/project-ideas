# Free project 2


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This language would serve latex users, helping them figure out how to do what they want mathematically in latex's language. 

Latex is hard to learn. There are a ton of commands that you have to google search to be able to write, and you usually have to do this one at a time. Despite this, its still the most widely used math typesetting language that I know of. My idea is for a DSL that lets someone input the mathematical words for the symbols they want to use, and have the language output the latex commands for whatever they said. A language is good for this, as it would essentially be simplified google searching, which is normally what people do (e.g. "floor symbol in latex" would be someone searching for "\lfoor" and "\rfloor"). Thus, a language seems like the natural extension of what this is. 

Additionally, this process only works on one symbol at a time. In my project, you could do something like:

floor(n over 2)

and get $\lfloor \frac{n}{2} \rfloor$ as a result.


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

The need is very simple and domain specific. You need to figure out how to write a symbol in latex, so you ask a language with a simple query syntax and get an answer. Seems self-evident here. 

### Why you?
_What excites you about this idea? How did you come up with it?_

First, I came up with this by looking at the reccomended domains section of the project ideas page. Then, I thought about things that I would like out of latex, and the first thing that came to mind was an easier way of finding out how to write what I want. I'm excited by this, because since I write latex a lot, its something that I would actually use. 

### Domain
_Describe the project's domain in five words._

Latex symbol syntax lookup helper 

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

This is the most important part of this project. If the language isn't intuitive to use, then its no better than latex, as the user would have to look up in the projects documentation how to write what they want to get what they want in latex. Not very useful. The basic idea would be two things. First, a user could specify a mathematical statement in the syntax of the language, and save it as a variable. The language would output the syntax for this, and then save the variable. One could then modify the original variable, so it would look like:
var x = [statement in math language]
> [latex syntax for statement]
var y = x + 2
> $[latex syntax for statement x] + 2$
and as such reduce some of the copy-paste work that goes into latexing math. Obviously this example is trivial since adding two to a statement is easy, but if it were something that involved more complex syntax, this could save a lot of time. 

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When the program runs, the user's input would be parsed by an engine that then looks for the symbol that best matches what they asked for. This should be relatively simple. The real issue is if the user looks for something that doesn't exist (or mispells something). Instead of just erroring and breaking, the system should try to "fuzzy match", or find something that the user probably meant. It should then ask for the users input here, probably displaying a list of possible alternatives (a la Google's "did you mean X?"). This output would be hard to do via image, but could be done through text pretty easily. A GUI for this could let you do it via image.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

Ideally, any latex query should be easy to do (as long as its in the program's database). Things that are possible but difficult *might* include some level of symbolic manipulation, i.e. simplifying expressions that you give it. This depends on how feasible it is to implement, and how much users want it.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are, with the best example being [Detexify](http://detexify.kirelabs.org/classify.html). This site lets you draw a symbol, and it outputs suggestions for what you meant in latex. I use this quite a bit. The issue however, is that it only lets you do one symbol at a time. If you want to compose complex symbols, this is less useful, as you have to deal with the composition syntax yourself. 

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

By *far* the most time consuming aspect of this project would be the language issues. Like I said earlier, if this language isn't as intuitive to use as possible, its just another layer of indirection above latex, which helps nobody. I can imagine *tons* of user study data being necessary to make this work. 

### Scope
_How big an idea is this? How ambitious is this project?_

The idea itself is pretty small. There are more ambitions extensions of it, like symbolic manipulation, but the overall concept is very doable. The challenge is entirely in getting it to be something that people want to use. Making it work on a systems level should be quite easy relative to my last idea.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This is something that, if done right, could be very very useful. Additionally, its entirely a question of the language design itself, so its perfect for the class goals. However, there is a very very good chance that it will just fail, and end up being useless to people, or that its simply not possible to make something like this work. 
