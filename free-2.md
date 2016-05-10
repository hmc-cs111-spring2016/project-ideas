# Legislative Law

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

The language is designed for policy makers and legislators. The legislative process for passing laws seems to be concerned less with the content of the law and more with the language of the law. Several laws are written with intentional vagueness and ambiguity for the sake of less opposition. This turns out to be very problematic later on as ambiguity inevitably leads to different interpretations with respect to legality. This language would seek to provide some standard for future laws and if permitted some form of logic checking.

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This idea helps eliminate ambiguity in laws. This language would help legislators in both developing laws and referencing laws. With a computer based language, it would be significantly easier to look up laws. For instance, there may be several laws that come up when specific key words are searched(e.g. "shoplifting with weapon law") that differ drastically based on context (state-state level, scale of the shope, state-national level). Additionally, legislators could avoid drafting a similar law that was previously repealled or still enact. As of now, it seems like drafting a law requires a significant amount of man power just to reference check thoroughly. 

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate because it is deliberate and strict. Unlike English, this DSL will allow little room for ambiguity as it will have fields such as who/what this law is intended for, when this law will be enacted, who/what this law will effect. This DSL addresses a longstanding need for clarity and conciseness in law making.

### Why you?
_What excites you about this idea? How did you come up with it?_

I am currently taking a public policy course off campus and one thing made extremely obvious is how convoluted the legislation process has grown to be. You don't have to be taking the course to understand just how slow the process can be. Although it can be argued ambiguity is a virtue (which is something we discussed in class e.g. the Constition is relevant today only because of its ambiguity), I think there is significant room for optimization.

### Domain
_Describe the project's domain in five words._

Law making without B. S.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

A legislator may interact with the lanuage by entering statements line by line, with each statement being some rule that adheres to the syntax of the language such that it can be made some logical predicate. Programming would ideally look closer to natural language with a few syntactical oddities (maybe logic symbols) to ensure clarity and enforce rules/logic. I would argue this is the right way to interact with laws because legislators can focus more on the content and less about the semantics.  

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

Ideally, when a program runs, each statement will be processed into a logic statement which could then be compared to the existing set of laws and show similar or related laws. There can also be a field to specify some type of categorization of the law e.g. federal law, state law, local law, etc. Errors that may occur include improperly formatted statements, or conflcits with existing laws, which would be outputted and made apparent to the user.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be pretty easy to write clear laws. I feel like one determinant of how effective this DSL will be based on the language design. The language should be flexible enough to express any reasonable law, but unflexible to a degree that makes it difficult to make ambiguous rules. It should be easy to define new terms, but difficult to retroactively enforce this new term that may have been accidentally used. It should be impossible to incorporate any kind of control flow as the domain doesn't exactly lend itself to this. 

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

I think there are some slightly relevant DSLs in this domain. They are mostly concerning [business logic](http://www.drools.org/) and private industry rules. Drools seems like a pretty popular and effective business rule management system, and its interface seems extremely easy to use. I think because the domains are related but not exactly the same, it's difficutl to compare qualities. 

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I imagine msot of the time would be directly engaging the language aspects of the project. Once all the basic legislative jargon has been implemented, the remainder will be spent on how to effectively design language to meet the pretty specific criteria specified earlier (specific enough to not cause ambiguity, unspecific enough to express most reasonable laws).

### Scope
_How big an idea is this? How ambitious is this project?_

This idea seems pretty big and ambitious, as it requires some type of logic checking (JAPE) in addition to the several legislative jargon that needs to be defined and implemented. 

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

I think this might be a good idea if someone was legitimately interested in legislation and logic; however, I personally do not have the necessary background in law making for this to be feasable (and CS81 wasn't exactly my favorite class). I do think there are several possibilties to explore in regards to the design of the language. 
