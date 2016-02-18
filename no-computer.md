# No computer project
Baseball! It's TOTALLY a DSL.

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

This language would be good for people who want to run baseball simulations to ask "what if" questions. If a pitcher throws the ball a certain way to a certain location to a certain hitter who swings a certain way, what will happen?

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This idea would help baseball executives and casual fans alike entertain possibilities of things that would happen in a game. For an employee of a baseball team, it would help them prepare for games and opposing pitchers/hitters by "seeing what would happen" ahead of time. It could also help settle petty arguments between fans or help them see what would happen if their favorite player did something specific.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate because so much language and terminology is specific to baseball. We can define these things specifically in a DSL, which makes it seem like the right approach. We can define the field, the players, the strike zone, and so much more as well.

### Why you?
_What excites you about this idea? How did you come up with it?_

I LOVE baseball and this is totally something I would use! I think baseball, which is one of the stats-heaviest sports I can think of, lends itself well to computation and simulation well.

### Domain
_Describe the project's domain in five words._

Helping people simulate baseball events

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

I think the user would input either existing players (whose hitting zones, pitch preferences etc would come directly from the internet) or create players within the program, as well as a pitcher with certain pitches, pitch speed, and so on, and then ask at what likelihood different events would occur (single, strikeout etc) if a pitcher through a certain pitch aimed for a certain area. This is the right way to interact with the domain because the user is given the ability to specify exactly the desired event.

The DSL is massively extensible, which is both a blessing and a curse. The field itself can be broken up into (arbitrarily small) zones and then, if a physics engine is applied, we could actually simulate where a ball would go, with what exit velocity, and so on.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

I think at first, the program could look up how hitters have dealt with certain pitches in certain zones in the past, and also see how well pitchers have successfully located pitches in the desired location in the past (baseball has lots and lots of data -- this would be easy to look up/reference), in order to provide some sort of probability of various outcomes. Eventually a physics simulation could be added, which would actually look at contact with the bat and provide a prediction for where a ball would land.

Errors would possibly include insufficient data (at which point perhaps the program could harbor a bad guess or something like that), or if the user inputs unreasonable inputs, which the program wouldn't be able to do anything with, such as the pitcher throwing 200MPH or something like that. I suppose the program would simply pop up an alert/error

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to make predictions as to how batters will do against certain pitchers (as this is the intended functionality). It should be difficult to ask for unrealistic projections, such as impossibly fast pitchers. It should be impossible to create non-standard baseball outcomes, like a ball hitting a bird or having fan interference disrupt play.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_
There is [baseball-sim](https://www.sabersim.com/mlb), which is very similar to what I described! (I didn't know about it before I started writing). While the writer does pretty much everything I described above, he still feels the simulator is not very useful -- he writes about his thoughts [here.](http://www.hardballtimes.com/10-lessons-i-learned-from-creating-a-baseball-simulator/)

## The Project
This section examines whether the idea makes for a good CS 111 project.

Probably not a good CS111 project... I think it's probably a bit too complicated.

### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I think this would require a LOT of systems/semantics work, especially in defining all the terms and outcomes of a baseball game. As such, I can't imagine it would be particularly fun to code.

### Scope
_How big an idea is this? How ambitious is this project?_

Extremely ambitious. Huge idea.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This would be a good project because nothing in the project would be difficult to do on its own. That is, all the components are doable and straightforward. That said, there are just an unreasonable number of components, which is why this really would not be a good idea for a project on such a short timeframe. If I had more time though, this is definitely something I would like to pursue!!


