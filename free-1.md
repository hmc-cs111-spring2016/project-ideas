# Free project 1

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

It seems as though there are many people struggling with the same problem: how do we place things into groups based on an assortment of criteria. Much of this sort of problem solving is done by hand, but as the domain becomes larger, it becomes nearly impossible to do by hand. I would like to create a language to help these people, perhaps specifically focusing on creating a language which clinic organizers can use to place students on clinic teams based on what position they like, what projects they are interested in, who they want to work with or do not want to work with, and perhaps even who thy can easily meet with on a weekly basis. This is a small domain in which a general purpose programming language could be unweilding and over complicating but still large enough that a full language would make planning significantly easier so I think DSL could easily fill that niche.

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

We need better ways to describe a set of constraints and relationships to organize teams for things like clinic. Many students become very frusterated with clinic because they don't work well with the students on their team or don't like their project. If we could create a language that would make optimizing the team divisions easier, everyone might have a more positive clinic experience. 

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL would allow the users to easily learn how to use my language and then use it to input all the data on which clinic team assignments are decided and then just trust the computer outputted optimized team divisions. This removes much of the human bias from the selection process and greatly simplifies the process for the faculty in charge of the team divisions. It optimizes to meet as many of the weighted hopes of the students to grant them better clinic experiences and it is easily scalable for organizing teams even if the number of students doing clinic doubles or triples.

### Why you?
_What excites you about this idea? How did you come up with it?_

I am enthralled by this idea because it addresses a very relevant problem at Mudd. It seems like it would work well with a language like Prolog which I am interested in exploring more in depth, and is easily scalable so that if I have enough time I can add many additional features, but I should be able to get the base of the language created well within the alloted time frame. 

I came up with this because I was interested in creating a Prolog like language that does some sort of pattern matching, rules, and data storage, I liked the ideas in the tree-tracer lanugage created by ellenfkh which stored relationships from complicated book series and allowed you to look up characters again later and I discussed my idea with Prof Ben and he gave me the idea of applying it to the specific domain of clinic team formation.

### Domain
_Describe the project's domain in five words._
Optimizing clinic team formation choices.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user would interact with the language by creating new students in the system with a set of things the student want, weighted by how important each is to him or her. The user can then type a command to get the best clinic team divisions. A program would look like instantiating a set of students and then typing a command to get the top few possible team divisions. This is the right way to interact with the domain because it is very similar to what is done now excpet that rather than having a person do it, the computer will be considering all the combinations of possible teams based on the criteria and choosing the best.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

If I create this as an internal DSL in Prolog, when a program runs it will run as a Prolog program, checking to see what combinations of variables match all the rules its been given and will then ouput the desired number of most optimal team divisions. If there are multiple "best" team divisions the program should let the user know about the tied team divisions. If there is no best division the program should print an error asking for more criteria.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to optimize team formation. It should be difficult to create programs in which you specify criteria that absolutely must be true, becuase the language should try to find the best combination which satisfies the most important criteria, but should not satisfy one students desire at the cost of everything several other students want. It should be impossible to use the language to program more general things that don't have to do with optimizing based on a set of criteria.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

I have been assuming the clinic teams are determined by the clinic coordinator, but I emailed her to check if that is actually the case or if she uses some sort of software to help. GPLs like Prolog function in this sort of braod domain and are used for many things like this, but most programmers are more comfortable with languages like Java, Python, C or C++ where the programmer tells the computer exactly what he or she wants it to do rather than languages like Prolog where the programmer defines a set of rules and the pogram figures out what combination of things satisfies those rules.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

This language would most likely be an internal DSL in Prolog, so most of the time, (maybe 80 or 90 percent) would be spent making language design decisions such as what criteria the user will be able to specify for optimized team divisions.

### Scope
_How big an idea is this? How ambitious is this project?_

This feels like an easily extensible project. The base of the language should only take a few weeks to create and then the rest of the time would be spent adding additional features to make it work better and to allow the user to specify more criteria.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This woulc be a good idea for a project because it is easily scalable, it would address a real need for people at Mudd, and it works in a domain like Prolog where quite a bit less has been done by mainstream programmers because most programmers are more comfortable with languages like Python, Java, C or C++ which are signifcantly more difficult to use to solve these types of problems



