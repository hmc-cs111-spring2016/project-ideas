# No computer project


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.



### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

Grading a problem set for a math or science class can be tricky and subjective. How do you determine how many points an incorrect solution gets? Graders have to use inuition to determine how close they are to a solution. Rubrics are essentially a DSL for grading, as they remove some of the subjectivity of this process. With rubrics, someone simply references the part of the problem set on the rubric, and reads off the points to give. 

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

The rubric itself is a simple language, only specifyin the amount of points to give someone for various different types of answers. Its a language because it has its own grammar rules of how to specify parts of a problem, breaking it down, and giving each a point value. It addresses the users needs by removing the subjective element of decision making. 

### Why you?
_What excites you about this idea? How did you come up with it?_

I grade classes. In Algs grading, we always create a detailed rubric for each problem, so we don't have to carefully read each part of the problem, but can just look for the parts we care about and input the corresponding grades. 

### Domain
_Describe the project's domain in five words._

Problem set grading breakdown system

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user interacts essentially with a table of problem part to point values. The programming language is the rubric, and a program is the problem set. To program is to map the parts of the problem set to the rubric. This is the simplest way to interact with the domain, because it breaks each problem into logical parts, so if someone answers part of the problem, but not all, you can pick out which parts they did and give the corresponding points.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, the user acts as the computer, breaking down the problem into its syntactic parts, and consulting the language (the rubric) for rules for how to interpret each part. It outputs a number. Errors occur when something isn't in the rubric. The grader uses judgement here, leaving a note (usually "good start" or "see sample solution", the standard error messages in this domain).

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

This language makes it very easy to grade problems that break down into the logical parts. Its very difficult, but still possible, to use it to grade problems that don't follow the logical parts using judgment and interpretations of the problem set. Its impossible to use it to do things other than grading. 

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

Other methods of grading exist, but this one is the most common. 

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I'm not sure how to answer this, seeing as rubrics for grading are already a thing, and aren't valid CS 111 projects.

### Scope
_How big an idea is this? How ambitious is this project?_

Same as previous question

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

Same as previous question.