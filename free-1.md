# Music Mixing

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

This project is mostly targetted at people who have a general interest in audio mixing, but have neither the background nor the expensive software typically used (e.g. Ableton). Additionally, for the less serious music enthusiast, this DSL would be a significantly lighter weight and cheaper alternative to currently existing music software. This DSL would help users learn more about mixing music by providing them basic and easy to understand tools to manipualte sounds as well as allowing them to develop their own tools if necessary. For instance, some built-in features of the language might be basic volume adjustments at specified intervals or  allowing for a certain segment of a sound to be looped.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This DSL allows users to get their food in the door when it comes to mixing music. Given how popular electronic music has become, I imagine that several fans probably have a few of their own novel ideas, but no outlet for them. I know personally that most existing audio mixing software is not only very pricey, but also extremely complicated. Simply learning how to use the basics requires several hour long tutorials on Youtube. This DSL plans to help amateurs who simply want some exposure to audio mixing without the time or capital investments.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

I think a DSL would be appropriate because, if designed effectively, audio mixing can be made more user-friendly. Most audio mixing software emulates a DJ console (the thing people use with a lot of knobs and dials and what not). Although it may seem counterintuitive, I felt audo mixing can be more effectively done through a language rather than a visual gui of a DJ console. To me, all the knobs and dials are pretty intimidating, and make it difficult to express ideas.

### Why you?
_What excites you about this idea? How did you come up with it?_

I once thought audio mixing would be an extremely easy thing to do. I had several ideas, but was met with more barriers to entry than I expected, including both the cost and complexity of existing software. Although these tools have been proven to be the best for the trade, these barriers alone were enough to make me abandon the idea. I felt like at the time there existed two extremely polarized types of audio mixing software: extremely powerful but extremely complicated, and extremely simple but extremely easy. I'm hoping this DSL will find somewhat of a middle ground. 

### Domain
_Describe the project's domain in five words._

Music mixing for the amateur

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The program would take in any number of audio files and allow the user to apply some basic audio manipulation tools to it such as volume, bass, speed adjustments, cutting and looping tools, simultaneously playing multiple tracks, among others (mostly limited by the scope of the project). The user could combine some of these tools to create their own. Programming might look something like LateX in that it would look very structured with sequential blocks that correspond to parts of the music file (e.g. \begin{volume-boost}@3:44 ... \end{volume-boost}@3:55) or something along those lines. I think this is a correct way to approach the problem as it makes the structure of the music files more apparent without any visual ui. 


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

The program would run through the code above when a specific key word is found (e.g. play at the bottom of the file) and apply any effects to the song. A program interacts with the user by outputting any changes they make to the song. Some errors that might occur include applying an undefined effect, applying an effect outside the bounds of the current song, undefined behavior when combining effects, among others. 

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to do very basic individual edits like increasing volume at a certain portion of the song or increasing the bass near the end. It should be possible to actually make a song from scratch using several samples created from another audio recording program, but this would be extremely difficult to do. This language seems more for editting an existing song. It would be very difficult, if not impossible, for users to make production quality music with this, I imagine, given its rather basic tools. 

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

It seems like there are already exists a good amount of [audio entertainment related DSLs](http://kyma.symbolicsound.com/); however, each of these appear to target a different niche area of mixing music. For instance, a good amount of existing DSLs seem to be focused more on classical music and composing classical music. Given their continued existance, I imagine most of them address the needs of their particular users. DSLs more related to mixing music seem to go for a "big language" approach in that it almost emulates their audio mixing software counterparts in complexity. As argued before, although it allows for more professional usage, it makes it difficult for amateurs to learn.

## The Project
This section examines whether the idea makes for a good CS 111 project.

### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

It seems like it would be a 60-40 split, with 60 percent of the time spent directly engaging in the language aspects of the project and 40 percent spent on the systems aspect. As discussed in the scope question, I feel the most important part of this language is the user-friendly aspect. The project could easily be 99% systems in that the language will have several audio manipulating tools, but determining an effective language design feels more relevant considering my intentions.

### Scope
_How big an idea is this? How ambitious is this project?_

Although the idea seems big and extremely ambitious, it can be rescoped to only include a few audio tools, with most of the project focusing on directly engaging with the langauge aspects of the project. The language design decisions are probably the most important aspect of this project as the language is built with the intention of making the process easier to understand nad less overwhelming.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This would be a good idea for a project because it genuinely interests me and meets a need I actually have. Additionally, consider I will be focusing on the language design, it seems extremely relevent to our course. This might not be the best idea because it can easily get out of hand given its potential scope.

