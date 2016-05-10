# Free project 1

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

Part of being a great drummer is having a wide variety of interesting drum fills in your arsenal.  However, since drummers' ears/hands are so used to hearing/playing the same cliche drum fills, it can be difficult to come up with original, rhythmically-interesting fills.  With some sort of external creative stimulation, this could become much easier.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A language would provide drummers with an interface through which they could create fills and then apply modifications to them (with some element of randomness).  This could potentially help drummers come up with interesting ideas for fills that they otherwise might not be able to.

### Why you?
_What excites you about this idea? How did you come up with it?_

I came up with this idea after thinking back to my experience of trying to pick up the drums.  I felt like everything I was playing, especially my fills, were very uninspired and had difficulty coming up with rhythmically-interesting fills that didn't sound like a bunch of other fills I'd heard.  It excites me because it relates to music (music = exciting) and it's something that I'd want to use myself.

### Domain
_Describe the project's domain in five words._

Creating and discovering drum fills.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

A user might be able to define a fill in the following ways:
- By creating an ASCII representation of musical notes. 
- By creating fills programatically from their constituent parts.  A Fill might be made up of Measures (by defining measures separately, each could have a different meter.  This is important for complex fill patterns), which might be made up of Beats.  Notes could be defined on top of whatever rhythmic structure was created with the previous 3 elements.  Notes are played by Instruments (each piece of the drum kit is a different instrument), which are each assigned their own audio file (or MIDI instrument?  Not sure about this).
- By calling some command that creates a random fill based off some specified parameters, such as min/max note value, number of measures, etc.

Once a fill is made, a user should be able to modify it with various commands, such as "randomizeRhythm(Instrument kitPiece, Measure measure, Int maxNoteValue, Int minNoteValue)".  This type of interaction is helpful because it allows users a large degree of control over the types of modifications they could make to their fills.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

Running a program would be similar to running the program from the soundbyte lab.  After defining a fill, users would be able to modify it incrementally (and, importantly, be able to hear what it sounds like after each step).  Syntax errors could occur if users call commands improperly, and these errors could be communicated to the user by pointing out the problematic portion of their code.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to create simple drum fills and randomly modify specific aspects of them.  It should be possible, but difficult (tedious) to create a drum track for an entire song.  It should be impossible to change the pitch of an instrument (meaning no melodies can be played with a single instrument).  Generally, it should be impossible to do anything other than create and modify drum fills.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are many GUI-based drum sequencers, and there is even an app to help people notate and randomly generate drum fills called [DrumFill App](http://www.drummerworld.com/forums/showthread.php?t=96465).   However, this app provides very little flexibility in its random generation of drum fills.  From what I understand, it has something along the lines of a "generate random fill" button, and doesn't allow users to randomly modify existing fills (let alone randomly modify them based off specific parameters).  This is something that could definitely be improved.  An admirable quality is its user-friendliness.  Since it is GUI-based, things like notating drum fills are very easy.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

It's difficult to tell at this point, but my guess would be around 50% language design.  In terms of language design, the creator would have to design a way to accept an ASCII representation of a drum fill.  The creator would also have to create user-friendly syntax for commands that would alter the drum fill.   In terms of "systems", algorithms would be needed to develop to properly randomize elements of a drum fill based on given parameters.  The creator would also have to come up with a robust representation of a drum fill internally (a potential system for this was explained in the "Interface" section), and a playback system would need to be created, likely with MIDI.

###  Scope
_How big an idea is this? How ambitious is this project?_

This DSL idea is relatively ambitious, as it would require a few separate processes to be implemented, none of which are trivial.  These processes include drum fill "parsing" (reading in fills that users create), algorithms to alter these drum fills, and properly handling MIDI.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This might be a good idea because it's very extensible.  The creator could start off with support for just one "instrument" (e.g. a single track for just a hi-hat) and a basic "randomize" algorithm.  This would allow the creator to flesh out the "language" aspects of the DSL while having a fully-functioning vertical slice of what the final DSL might look like.  From there, for the purposes of the project it shouldn't matter too much how far along the creator is able to get in adding multiple instruments or more complex "randomize" algorithms.
It might not be a good idea because the project depends on some potentially complex, non "language-y" things like audio/MIDI manipulation that could prove very time-consuming.
