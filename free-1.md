# Free project 1

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

This language would be for describing dance choreography. The project would serve both
choreographers and those trying to learn choreography. A language could be useful as
the current notation system is extremely complicated to both read and use.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

Currently, choreographers primarily use Laban notation for written records of their
work. However, Laban scores are notoriously complicated. Developing a computer
languge to either simplify Laban or quasi-replace could help make reading
choreography more accessible. At this point, choreography is often reproduced
by either knowing the choreographer or by trying to figure it out from a video.
The first method is very limiting, and the second method is not always very 
accurate. By having an easy(er) to use language, this could widen the 
accessibility and record-keeping of choreography.


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

Given that Laban notation, a DSL of sorts, already exists, it's seems reasonable
that a computer-based DSL could help with record keeping. This addresses
the need by making that record keeping easier.

### Why you?
_What excites you about this idea? How did you come up with it?_

Personally, I'd be excited to easily record my own choreographic ideas. Right 
now, I always have to jot down notes and hope I'll understand what they mean
or take a video (not always very practical). Having a languge to play with
to create could be useful. This was the inspiration for the language--my own
potential use of it.

### Domain
_Describe the project's domain in five words._
Choreography creation and record keeping.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

To interact with the language, the user can write out commands for different
areas of space the dancer should interact with or the quality of movements.
Programming will look like writing out at least a spacial direction, and then 
layers can be added on (which limbs, quality, timing, etc). This is a useful
way to interact with the problem domain because it starts from the key part of 
dance--where are you--and adds on layers to create the dance itself.


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, the user could maybe see some sort of basic visualization
of the dance they have created. This can this be used as a guide for actually
dancing out the ideas that the user has. Errors could be things like programming
anatomically impossible movements. Having knowledge of what those are could allow
the programm to give error messages like "Human arms don't work that way" and such.


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

Giving the instructions for the space for the dancer to move in should be 
easy to do. Specifications (as more and more arise) should be increasingly 
difficult. Choreography that is humanly impossible should not be programmable.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are some programs that exist to aid in choreography, such as http://www.choreopro.com/Dance_Designer_s/47.htm
or http://dance.lovetoknow.com/Ballet_Choreography_Software. However, most of these
options seem outdated, and I've never seen anyone use one in person. Given that
they seem to have fallen out of use, I don't think that these are very reasonable 
solutions to the problem.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_
I think the hardest part of this project is the language aspects, by far. There
is a lot of work to be done in deciding how to represent different movements, 
which movements to allow, which movements to not allow, etc. Because movement is
not finite, the language should be as open ended as possible. However, this will
require a lot of organization.

### Scope
_How big an idea is this? How ambitious is this project?_
Pretty ambitious. There's a lot of range in dance and movement, which is part of
the difficulty. To be succesful in creating this, there would need to be a way 
to break down and work on just a smaller aspect of the domain (such as a 
specific style of dance or a certain type of movement). 

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_
This could be a good project because it ties my two majors together, which is 
pretty exciting. However, it could be very broad and open, and might be hard to 
pull all the pieces together. The scope has to be narrowed.

