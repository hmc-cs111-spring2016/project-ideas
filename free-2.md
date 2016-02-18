# Free project 2


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

It can be difficult for script-writers (of TV, film, theater) to get a sense of how their dialogues sound before an initial read-through, especially when the dialogues are chaotic and involve many characters speaking lines at precise timings.  By having a simulation-type DSL that could perform read-throughs of dialogues, script-writers would have an easier time planning out chaotic dialogues before hiring voice actors.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

Script-writers already write out their scripts via some sort of text editor.  With this DSL, they'd be able to assign specific timings for lines of dialogue.  Script-writers would then be able to export their script to an audio file and listen to a rough read-throughs of their dialogues without having to hire a crew of script-readers.

### Why you?
_What excites you about this idea? How did you come up with it?_

To be honest I don't remember how I came up with this idea.  I just found a note on my iPhone from a week ago vaguely describing it.  What excites me is that it seems like something that could actually be of use to people.

### Domain
_Describe the project's domain in five words._

Simulating dialogues that depend onTiming.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user would interact with the language creating "scenes" of chaotic dialogue that are ideally not too long.  For each scene, the user would start by defining a list of actors.  The user would then type out the dialogue along with markings to indicate the timings of each line.

Character Kevin = K  
Character Maria = Ma  
Character Marcus = Ms

* K: Hey, wanna hear a jo- {-1}
* Ms: Shut up! {10}
* K: Uhh, you okay?
* Ma: He's having a bad day.  Just leave him alone.  {-5} 
* Ms: I said stop talking!  {20}
* Ma: Oh.  {10}
* K {-1} + Ma: Sorry.  

Explanation: the number in braces at the end of each line represents the amount of silence before the next line (unit in this case is 1/10 of a second).  A negative value would indicate that the line is interrupted by the next line.  No value (see line 3) means that the next line will start after some default amount of time.  The last line will be spoken by both Kevin and Maria in near unison (Kevin will start one tenth of a second earlier than Maria) one full second (10 tenths of a second) after the previous line.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When the program runs it should parse the user's script and generate an audio file by layering audio clips (one for each line) on top of each other based on the timings given by the user.
Any types of errors on the user's end, such as typing "Charcter" instead of "Character", should be displayed to the user as an error message highlighting the problem area.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to generate read-throughs of dialogues with precise timings for each line.  It should be difficult, or impossible, to do pretty much anything else.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

Yes.  [Readthrough](https://readthrough.com/) and [Screaming bee](http://screamingbee.com/Product/ScriptVOXStudio.aspx) are examples.  Both do essentially what my DSL would do except for the following:
- They provide a large amount of control over the details of the pitch and timbe of the voices used.
- They provide little to no control over the timings of the lines.

While my DSL would also ideally provide control over pitch/timbre, this may be out of the scope of the project.  It is because these DSLs already exist that my DSL would focus specifically on busy dialogues rather than on entire scripts.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

If a suitable TTS API/Library can be found, the majority of time (maybe 70%+) would be spent directly engaging in the language aspects of the project.  A "systems"-type aspect that would still need to be addressed is the I/O for the audio.  Clips generated from the TTS API/Library would have to be properly stitched together and then output as a single audio file.

### Scope
_How big an idea is this? How ambitious is this project?_

The project seems decently-sized.  The scope is very specific, meaning that there aren't a huge number of features to be implemented.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

The fact that this DSL would rely heavily on some sort of TTS API/library is potentially a benefit or a drawback.  The benefit is that, if a decent TTS API/library can be incorporated then the creator of this language could focus mostly on language design elements.  If, however, a decent TTS program that would work with this DSL can't be found, then the DSL might not be feasible.