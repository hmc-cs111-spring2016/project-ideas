# Free project 1

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

The project would serve mathematicians who want to be able to clearly and efficiently articulate and visualize combinatorial problems. A language makes sense for a number of reasons: there are many structured problems in combinatorics that could be specified in a language nicely. For instance, being able to specify that you want to place 3 green balls and 2 red balls into 6 indistinguishable bins. There are nouns like balls and bins and other combinatorial objects, and verbs that could specify different aspects of those objects (they're really adjectives but they could be used as verbs). The language would be able to understand certain aspects of the problem and help users understand them.

I imagine two different kinds of experiences that could be aided by this language:
* The experience of a mathematician already familiar with combinatorial principles who wants another tool to help them articulate a new combinatorial problem. Right now, it may take time to visualize the problem or compute basic aspects of it, but this tool could simplify those processes.
* The experience of someone learning combinatorics. This tool could make it easier to learn the principles of combinatorics in a few ways: it could help them visualize problems, it could let them see why the answers to certain problems are as they are, and it could let them describe new problems and essentially play around with it to get a better understanding. 

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

Many concepts in combinatorics are very unintuitive at first (such as generating series). This language could make understanding those concepts a lot more intuitive. Additionally, Professor Omar (my combinatorics professor) has mentioned that in his work he often makes use of programming. A DSL to streamline that workflow could be useful.

### Why you?
_What excites you about this idea? How did you come up with it?_

I love math, I'm in combinatorics this semester and it seems appropriate. I think the topic has a lot of potential for a project like this.

### Domain
_Describe the project's domain in five words._

Describing and visualizing combinatorics problems. 

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user starts by specifying a problem. Programming consists of asking the DSL to compute different aspects of that problem, changing aspects of the problem on the fly, adding new objects to the problem and examining how they interact with each other. Ideally there would also be a visual component where you can see parts of the problem visualized. 

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs it creates a model of the problem that was specified so that the user can query that model for information. An error could consist of the user specifying something impossible or something that makes no sense, for instance asking how many ways there are to put 3 balls in -1 bins. 

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to specify an instance of a problem, it should be easy to modify different parameters of that problem (like the number of objects or the number that have certain properties) or add additional objects and specify how they relate to the original objects (for instance, you might have a grid with a number of stones on it, and you might specify that another grid exists and say that the stones can't be in the same place as on the first grid).

It should be difficult to specify problems that aren't really combinatorial in nature. I could imagine using the syntax of this language in some kind of subversive way to solve other unrelated problems.

It should be impossible to specify certain other kinds of problems. For instance, combinatorial problems are generally specified with integers, so there would likely be no floating-point type, so you'd be unable to specify anything decimal. You wouldn't be able to do anything in other mathematical domains for this reason (at least not easily). 

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are "combinatorial calculators" online (like <http://www.numberempire.com/combinatorialcalculator.php>). These are great for the very narrow domain that they service but I want to give the user more freedom to define different parameters of a problem. They shouldn't just be able to specify that they're picking 6 eggs out of a basket of 20; they should be able to specify that 10 of the eggs are red and 10 are blue and that all they care about is how many blue eggs they pick, or that they actually care about how many ways there are to place those eggs in a circle so that no two red eggs are adjacent, and so on. All of these things would hopefully be specifiable using some more general syntax. Something that dictates what is acceptable in a solution to the problem. This is much more general than these kinds of calculators.

There are also many libraries in existing general-purpose languages that can serve this function to a very minor degree (like itertools in python which can get combinations and permutations of a list). But these are really targeted more towards general-purpose programmers who need these basic functions. I'd be targeting those with more of a mathematical interest and not a general programming interest.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I'm really not sure. I think both would require a lot of work. The systems in the project would probably be fairly complicated, but if I didn't care about big scope then I could just write some back-end that just computes all of the possibilities enumeratively (which would be slow but simple). Language design would be a big component: figuring out how to allow the user to specify how objects interact with each other, and what kinds of interactions I would allow the user to specify, ans what kinds of things they would be able to query and how they would be able to query those things and what form the information would be displayed in. All of these are language design decisions that might be tricky.

### Scope
_How big an idea is this? How ambitious is this project?_

I think it's a very expansible project; it has a lot of basic functionality that would be relatively simple to implement (specifying basic problems) and many other features that could be added on. I could start with something at the level of the combinatorial calculator and add features onto it one at a time, eventually getting into things like visualization.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

It'd be a good idea because I'd be very interested in it and I think I have a good idea of what it would be like. I have some domain knowledge that I would be able to take advantage of. On the flip side that knowledge might constrict my view of the problem, so I would need to be careful to gear it towards what a general person interested in combinatorics needs and not just what I would need.
