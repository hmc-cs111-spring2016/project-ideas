# Free project 4 - Encoding Decoder

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This project would serve weird people (me) who want the ability to transform text into different encodings. If a person were writing a message in Morse Code and realized that they wanted to see what it looked like in Braille, this language would be able to meet their needs.

The idea meets the needs of people who enjoy encodings but don't want to take the time translating between them. It would be especially useful for events like [puzzlehunts](https://en.wikipedia.org/wiki/Puzzlehunt) in which participants solve puzzles. Some of these puzzles involve multiple ciphers which the average person can't translate on the fly. With this language, the user would only have to input the encoded text as well as the language of encoding/decoding and the user would understand what the encoded text was saying.


### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL would be appropriate for users because it would give them a lot of options when encoding or decoding text. The user would not necessarily need to translate to/from English and could select from a wide variety of encodings. It could also include the functionality of listing how a string would appear in multiple different encodings, something which would address a user's need for more information and could help with time constraints in encoding puzzles.


### Why you?
_What excites you about this idea? How did you come up with it?_

I have participated in a lot of puzzle hunts and I really enjoy learning new encodings. In the past, teammates who don't have encodings memorized take a while to decode them. If they use online solvers, they need to use a different solver for each type of encoding. I came up with this idea in the interst of consolidating many different decoding tools into a single resource.


### Domain
_Describe the project's domain in five words._

Translating between all the encodings.


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The interface could be either a CLI or a GUI. I could see this as a web app resembling [Google Translate](https://translate.google.com/) where the user would specify two encodings. There could also be options in the GUI to list the text in all available encodings. I think that it might be easier to add functionality to the tool if it were a command line application. This would limit the user base to people who are comfortable with using the command line. I think that this could provide a more reasonable and extensible method of interaction for users. I could see a sample command being something like: 'encoding1 encoding2 textToBeTranslated'


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, the language would output the result of the translation. The user would be able to view this result and select it for use elsewhere. Perhaps the language could give the users the ability to do something directly with this result, much like piping commands. There could easily be errors if text or characters cannot be encoded in different ways, so the developer would need to take care to handle many of these cases and the language could communicate any remaining errors by saying that the text could not be encoded in the desired language.


### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to translate between two languages with valid character mappings (for example, Braille and Morse Code both map to the characters in the English alphabet). It should be possible for the user to add their own encoding system. Perhaps this encoding system would include several unknown characters, so it should be difficult but not impossible to translate between this and other encodings. For example, maybe the user created an encoding with a known character mapping for A-Z with the exception of two characters. The translation for this language would simply include blanks if there is no valid conversion. It should be impossible to decode languages with no common character mappings.


### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

As previously mentioned, there are many specific tools available that focus on a single encoding. [Morse Code Decoder](http://morsecode.scphillips.com/translator.html) is one such example. It allows the user to translate between Morse Code and English. A different [encoder/decoder tool](http://www.splitbrain.org/services/encode) lets the user input text and lists how it appears in a lot of different encodings. The first decoder is limited in that it only converts between English and Morse Code, though it has a helpful GUI. The second decoder does not allow the user to input a message in anything besides English (Latin) or UTF-8. However, it shows the user many different ways of encoding the text.


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I think the majority of the project would be spend on the language aspects of the problem. Especially if the DSL were to use the CLI, little time would need to be spend on a UI. The challenge lies in deciding which encodings to include and how to handle the errors associated with translating between the various encodings. Tied to this problem are the challenges of storing each encoding and their various character mapping as well as deciding whether the user should be able to translate between characters beyond A-Z.


### Scope
_How big an idea is this? How ambitious is this project?_

This is a fairly ambitious project. It seems fairly simple to explain on the surface but contains a lot of hidden problems that could easily cause a lot of trouble. It would be easy to start small and gradually expand the scope of the project.


### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

I think it would be a good project to get experience focusing on a specific domain. It would be possible to make the language extensible and the project would involve a lot of challenging questions. It would not be a good project idea if the questions were difficult to solve or if it tried to do too many things with little organization. The risk with this idea is starting small and expanding the idea in inefficient directions.

