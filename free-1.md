# Free project 1 -- Sound and frequency manipulation

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

I think the need being met here is and easy and user-friendly way to manipulate sounds and frequencies that the user records. As of now, I believe the only way that users can do what I'd like to have happen is by recording a sound, then using FL or other studio-type software to pitch bend to an appropriate frequency.  I don't believe there is an easy way to record and manipulate sounds in the way that I envision it.

I imagine the experience as follows: A user records themselves singing or playing an instrument. They then use the DSL in order to add thirds, fourths, and other intervals as they choose. They can also do other simpler things such as slowing down and speeding up 

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

I think a DSL is appropriate because it would allow for lots of different types of behaviours from the user, and would also allow them lots of precision. For example, if a user wants an octave above a recorded sound at 50 percent volume with .1second reverb, that would be easy to do and straightforward to write. I think it addresses the need by making it really intuitive to do.

### Why you?
_What excites you about this idea? How did you come up with it?_

The idea came straight out of the sound lab we did in class. As someone who loves singing and is especially obsessed with harmonies and chord progressions, this seemed like something I would love to use. 

### Domain
_Describe the project's domain in five words._

Modifying and complementing recorded sounds 

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user would start by recording and uploading sound files (in some format) and loading them in/putting them in the correct directory. The user would then use the commands written in to the language in order to modify, add to, and harmonize with the the sound file, by allowing the language to detect the frequency of the sounds in the file and apply transformations on it.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

As I wrote in the previous section, the frequency would be detected and tracked by the language after it is loaded in to the language. Then, once transformations are applied to the sound (by adding or reducing sounds at relative frequencies to the sound, by manipulating volume and reverb, and so on), the sound is then stored or played back (depending what the user wants). If multiple transformations on the sound are required, they are done in sequence.

Errors would occur if, for example, a sound that doesn't exist is attempted, or if a user does not provide the correct inputs for modifying a sound (like, for example, not specifying a volume increase value when calling a increasVolume function). A standard error message should do here.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to record voice or instrumental music and transform it in the ways described above. It should be possible but difficult to do so with multiple instruments at once, provided you know exactly what you want to have happen with the sound. It should be impossible or very difficult to produce new music entirely out of transformations on an original sound -- that sound should really carry the piece, as I could imagine it would be really difficult to create new compositions using just transformations.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

I think this is a good possibility for a project because there just does not seem to be something like this out there. FLStudio and similar applications allow you to pitch bend and autotune, which is nice, but there isn't anything out there exactly like what I am describing. This makes me both hopeful and nervous about this idea.


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

This seems like something in which language design would actually be the core of the work. I imagine extracting and manipulating the frequencies from a sound file is something that would probably be borrowed from another language or package. This would leave the programmer (me) with more time to actually think about and implement language design that makes sense.

### Scope
_How big an idea is this? How ambitious is this project?_

I think this is actually totally doable, **provided** the idea of borrowing pitch bending/manipulation software or packages from elsewhere isn't ridiculous. I spend a short amount of time perusing the internet for just such a thing and couldn't find anything, so perhaps I am underestimating the difficulty of such a project. But at the very lest this is something I _do_ know how to do with FLStudio so I do feel something can be finagled. Also, this is similar to how autotune works, so I know this technology does exist in some form.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This seems like a good idea for a project because it would allow the programmer (me) to focus on the language and design aspects of the project, and allow a lot of the more technical stuff (matching and bending frequencies, etc) to be taken from other projects. 

