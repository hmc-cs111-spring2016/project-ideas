# Free project 2


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

The idea of this project is similar to ContextFree: the goal is to make a tool for creation of a very specific kind of art. I'm not sure if there are specific users who specifically want to create that kind of art, but like ContextFree, knowing that the language exists would give you some degree of artistic inspiration (or so I'd hope). 

The idea is to be able to make small-scale animations and put those animations on a canvas in some way (maybe by just specifying x-y position, or maybe in some relative way like in ContextFree). Imagine something like a 5-frame animation of a square rotating 90 degrees, or a circle slightly growing then shrinking back to its original size. The idea is you would be able to make a bunch of copies of those small animations and choose where to place them on a canvas, and modify aspects of different instances of those animations like in ContextFree. For instance you could make one instance redder, or larger, or even have a faster or slower framerate. This would create interesting visual effects. Like ContextFree it would be targeted at abstract art. It could also benefit a LOT from randomness in the same way that ContextFree does.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

It's essentially the exact same idea as ContextFree: a language gives a lot of expressive power for how different ideas relate to each other. In this case you could express how an individual animation works easily, and specify where they should go and how to modify them.

### Why you?
_What excites you about this idea? How did you come up with it?_

A really, really, really long time ago (like somewhere in 5-10 years ago I'd guess) I liked to code things in Flash. I made a little tool that was like Photoshop except instead of drawing with a brush, you'd draw with animations. So as you clicked and dragged across the canvas it could make circles that grew and shrunk, and each animation would start as you drew over it so you would get a cool pulsating effect. I had around a dozen different animations that you could choose from. It's inspired by that, except the goal would be to give the user a lot more freedom to define custom animations.

### Domain
_Describe the project's domain in five words._

Abstract art through small animations.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

Again I think I could model this on ContextFree: the user modifies a program and can re-render their art as they change things to see what would change in the art. This is the right way to interact because it lets them quickly see if what they've changed is really what they want to change. They could quickly see a lot of different randomized variants of what they've created so that they can find things that they like and stress those things. They could essentially 'prototype' their animations in real time by adding frames and seeing what happens. 

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_


### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

Language design would be a huge part of this. Big questions would be how to specify an animation or a frame of an animation. For instance, would we want something where you can specify each frame like Animation{Frame{Square()}, Frame{Square()}, Frame{Circle()}} or something more focused on how an animation changes from frame to frame like Animation{Frame{Square(X)}, Frame{}, Frame{Circle(Y), Delete(X)}}, or any syntactic variations of any of these or any huge number of other ideas. The systems wouldn't be too complicated in comparison, I think.

### Scope
_How big an idea is this? How ambitious is this project?_

Like my first idea I think this is pretty extensible. It might be a tad ambitious because I'm not _entirely_ sure how easy the rendering would be to create. But I think it would be a reasonable level of ambitious.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

