# Free project 3

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This language would be to generate pictures of boba drinks. The project would serve 
boba connoisseurs and people who like looking at boba. The language would be a 
good way to meet this need because it means that people can generate their own
boba pictures without having to have artisitic skill. Currently, people can 
only create pictures of boba by drawing them by hand or actually taking a 
photo of a boba cup. Being able to create your own picture of a boba drink would 
be much more satisfying.


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL eliminates the need for artistic skill. Rather, the user just has to understand 
the basics of what a boba drink should or could look like. This is good, because I 
assume the user is a boba fan but not necessarily one with any artistic skill.


### Why you?
_What excites you about this idea? How did you come up with it?_

I really like boba. I was desperate for a final idea and then I had a lavendar milk
tea boba. The path forward then became clear.

### Domain
_Describe the project's domain in five words._
Boba drinks in beautiful pictures.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user could interact with this language by dragging and dropping visual
blocks, kind of like in Scratch. These blocks will be things like cups,
boba bubbles, and straws. Programming looks like placing these objects on 
some sort of background, making sure there is always a cup first. This is 
a good way to interact with this domain because this is a visual art, and 
the programming process is visual.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, the user is given a "compiled" (aka jpg or png) version of
the image. The program interacts with the user by letting them know where this 
image is saved or how to save it. If the user tries to create an image that does
not follow the rules (like having liquid to drink but no cup), then the program
will let them know that their boba drink is invalid. Another error might be trying
to save it to a non-existent location.


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

Making a picture of a boba drink should be easy to do. Making it look bad should
be possible but not easy. Having an impossible drink (liquid outside the cup, boba
instead of liquid) should not be possible. 


### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are plenty of other art DSL's out there. For example, we all played with
Context Free earlier in the semester. As for boba specific DSL's, I don't believe so.


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

This would probably be more of an implentation challenge. Having the graphical 
interface be smooth and easy to use could be difficult. The language choices
themselves should be easy since there's only a few things you can do to a boba
drink.


### Scope
_How big an idea is this? How ambitious is this project?_

This is a fairly unambitious project in terms of the language idea itself. The 
interface part, however, could be quite a lot of work. I don't know how well 
Scala is suited to creating such interfaces.


### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This could be a good project because there is a definited problem area and it 
can't be pushed out of scope easily. However, given that the language definition
itself won't be that complex, it may not be the best way to understand how
to create a language.

