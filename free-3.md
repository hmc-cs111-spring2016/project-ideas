# Free project 3

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

Unusual music listeners, like myself, generally listen to a large selection
of music that cannot be found in one place. For instance, certain songs I like
are only found on YouTube, while others can be streamed on Spotify, listened
to from a file, or streamed via internet radio. Although there are ways to
download songs from nearly any source, sometimes I just want to add a song to
a playlist without having to go through all the trouble. Unfortunately, there
doesn't seem to good ways to create playlists that span multiple sources.
Either you have a playlist on YouTube, Spotify, or locally, but never all
three. This DSL will be a wrapper around a database that allows you to
catalog a wide range of music from various sources and either play them locally
or stream them as a personal internet radio station to a private device.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

By wrapping a DSL around annoying music codecs, music sources, and APIs,
a single DSL will allow users to achieve many of the distinct properties
of a playlist in a program like iTunes, without needing to have all the
sources match. Additionally, by wrapping the DSL around streaming services,
your collection can be easily listened to on the go via typical internet
radio streaming services.

### Why you?
_What excites you about this idea? How did you come up with it?_

This is a practical idea that my roommate has previously attempted to address
(at least in the YouTube domain), with a tool he calls
[Snackbar](https://www.cs.hmc.edu/~wwong/playlist). While this tool is
exciting, I now want to make an "improved" version that also enables typical
playlist features, streaming, and inclusion of local files. I would use this
tool so much it isn't even funny.

### Domain
_Describe the project's domain in five words._

Listening from multiple audio sources.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

In some ways, I am torn about the best way to address this question. On one
hand, like ImageOrganizer, I am interested in designing this DSL so it is
easily incorperated into custom GUIs. That being said, a command line music
tool doesn't feel ideal. That being said, it is possible I could design it
as a command line tool and integrate it into a GUI as a plugin to something
like [Foobar2000](https://www.foobar2000.org/), arguably the most customizable
media player around.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

A program will be a wrapper around various APIs, database
requests, and streaming services. Thus, ideally, the end result will be a
pretty typical music player that has an atypical set of sources (i.e. not
just files). Especially if we go for a more GUI approach, it would be important
for errors to be communicated to the user, but not in a experience breaking
way. For instance, if there is an intruption to the internet, the removal of
a YouTube video, etc. the problem songs should be noted but then skipped.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to add new songs, shuffle, repeat, etc. Additionally it
should be able to stream music via typical internet radio methods without
much effort. Furthermore, adding a weighted shuffle with a series of
parameters would be awesome (i.e. song more recently added are more likely
to play, song with more upvotes are more likely to play, etc.) That being said,
it should be challenging to do things beyond this simple command/result
interface. The most complicated scripts will be simplified wrappers around
database commands for queries like "finding all songs listened to within the
last 10 days."

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

Although tools like iTunes exists for general music listening and 
[VLC](http://www.videolan.org/vlc/index.html) can
provide streaming (both as host and client), no tool that I've been able
to find enables these features in addition to allowing music from multiple
sources. The closest I've been able to find is
[Spotify](https://www.spotify.com/us/) which can allow users to listen to
music streamed from Spotify or stored locally on the computer. For what
I presume are legal reasons, however, you don't seem to be able to stream
the files on your computer or incorperate YouTube sources. That being said,
since I intend to only allow streaming to your own devices using either your
own files, accounts, or publicably available content, this program does not
suffer the same short comings as my Spotify client.

Additionally, as mentioned before, [Foobar2000](https://www.foobar2000.org/)
is an amazingly extendable media player that will likely be incorperated
in my solution in some capacity (perhaps dealing with codecs?)


## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

This project seems to have the most uncertainties of the proposed projects.
This is mostly because a lot of this project involves streamlining a number of
APIs, codecs, and tools under a single roof. Because of this, unless extensive
use of existing code from something like Foobar2000 can be utilized, a lot of
this project, although not all of it, will be on aspects besides the
language design. Although the language is ultimately the glue that binds
everything together, and thus its design will be closely tied to how the
various APIs work, the more I'm thinking about it, the more this might
devolve into trying to make a bunch of APIs play nicely together. That being
said, I would need to investigate code libraries a bit more before I can
be certain of this.

### Scope
_How big an idea is this? How ambitious is this project?_

Like  ImageOrganizer, although all the GUIs might make this, overall, a very
ambitious project, by scaling to specific functionality, assuming the existing
APIs play nice, feels like this could be a very reasonable project. This is
especially so since the ambitious parts of the project (i.e. the APIs) can be
trimmed down if they are not cooperating without limiting the design of the
language.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This might be a good project because it is very practical, seems well scoped,
and seems to provide tools that I have not been able to find elsewhere.

This might not be a good project because there is a lot of things that need
to come together. This means it might devolve into more of an API project and
less of a language design project.