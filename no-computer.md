# No computer project


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

There are a lot of songs that don't have official published sheet music or tablature. This means that if you don't want to learn a song entirely by ear, you might need to go to the internet for help. Unfortunately, a lot of the people who write guitar tab on the internet have no idea what they're doing. It's hard enough to check if sheet music is right without using, say, a piano if you don't have perfect pitch. It's even harder to do so with guitar tab, so basically the only
option is to learn to play whatever is written, hope whoever wrote it knew what they were doing, and find out if they did when you can play the song at full speed. This (speaking from experience) is a gigantic pain. Now, there are some websites that include a MIDI player for all their tablature, and it's pretty easy to tell whether that tablature is correct just by listening. The problem is that most websites _don't_ have those players. There are also some free software tablature
editors that come with MIDI players; in theory you could use these but they're generally GUI-based and involve a lot of clicking. With this DSL I think it would be less time-consuming to check whether tablature is correct.


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

Guitar tab already is a DSL (at least as much as sheet music and chess are, anyway). It can potentially have similar functionality to GUI-based tab editors, while being faster and easier to use for checking tab from the internet.

### Why you?
_What excites you about this idea? How did you come up with it?_

I play guitar (well, technically speaking I do...), so I've experienced the need I think this idea could fulfil. It's probably pretty clear from the first question that I would use this quite a bit if I got it working. Basically, I came up with the idea by wishing that all tab websites had MIDI players, discovering that tablature editors exist, and then deciding that they take too long to use.


### Domain
_Describe the project's domain in five words._

Checking correctness of guitar tablature.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

Very broadly speaking programming looks like writing a text file. The syntax might be similar to LilyPond (see below) but I couldn't say for sure. As long as everything in the language is clearly associated with a particular component of tablature it should be almost as easy to use as a graphical editor; typing tends to be faster than using a mouse, so it should also take less time to write a complete tab in text than in an editor. 


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

I have two ideas of what might happen when a program runs, and I think a fully fleshed-out version of this DSL should implement both because both would be useful. A program in this language might either output a MIDI file or a typeset standard musical notation version of the input. The user interacts with a program by benefitting from the output. Most errors will probably be syntactic, since I don't really imagine there being much of a type system, for example. It might be
reasonable to make it an error if the user says a chord has two different notes on the same string, or says anything else impossible. Errors would be communicated as the program is being processed (I don't know yet whether it would be compiled or run as a script).


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to express anything that's very common in tabs. The easiest thing to do in this language should be to specify the string and fret of a note, and its duration as a member of the set {whole, half, quarter, eighth, sixteenth}. It should probably also be easy to make dotted notes (e.g. dotted half note which is three beats). It shouldn't be difficult to express thirty-second and sixty-fourth notes either in a complete version of the language; however since it's always possible to
just double the number of beats per minute and write all notes with durations twice as long, I don't think such short notes are important to start with. I guess that means they should be possible but difficult. It should also eventually be relatively easy to specify how the guitar should be tuned.


### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

The DSL most similar to what I'm thinking of doing is called [LilyPond](lilypond.org). LilyPond doesn't actually let you check tablature, since it's designed to typeset music (this can be standard notation and/or tablature). As such, it takes note names (rather than string/fret combinations) as input. However, the language itself is very concise as far as I've seen and should I use this project idea I might emulate the syntax.

There are some tablature editors such as [TuxGuitar](www.tuxguitar.com.ar) which _could_ fulfil the intended purpose but are probably a little slower to use since they're really designed for people to write their own songs. All of these editors are GUI-based and, as far as I can tell, pretty click-heavy. This is fine for writing a new song, but if you have a preexisting tab to look at, it's probably faster to type it in than to click it in. Since the point is to save time checking
tabs that someone else wrote, using these editors works but is less than ideal.


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I think at least 70% of the work would be language design. There are libraries to output MIDI files, and things like LilyPond can already typeset standard musical notation. I think the largest piece of systems design would be the intermediate representation of the tab between the user's input and the final output.


### Scope
_How big an idea is this? How ambitious is this project?_

Every last feature I can think to include would make this a very ambitious project indeed, but the most absolutely basic functionality might not even take the whole second half of the semester. Specifying notes and their durations and getting a MIDI output would be well within the scope of this class, and if that turned out to be too small, there are things like chords and time signatures that could be added.


### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

The main drawback I see is that it has sort of been done before. It's also possible that other guitarists would not find a DSL to be the best solution like I think they might. I'd certainly need to ask some people before I could commit to this project. Aside from that, I think this is a good project idea.
