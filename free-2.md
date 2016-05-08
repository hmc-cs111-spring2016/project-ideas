# Free project 2

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This idea, like Binary Star, is another project I have previously started
called "ImageOrganizer" (although I will probably change this name). It is
designed as a simple DSL for organizing large quantities of images based on
user defined categories. This DSL will help computer users, like myself,
who generally save a lot of pictures to eventually need to attempt to sort
them. Although in the past I've designed a simple GUI with buttons
corresponding to predefined folders, I have always thought it would
be interesting to build a simple command line language that can be interacted
with by a customized GUI (similar to how Git GUIs interact with Git). Thus
the command line tools will allow for simple workflow, classification,
taging, macros, etc. Although many well defined tools already exist 
for organizing pictures (even Facebook provides features like this), by
building a simple scripting language like this, I can design different GUIs
to be used locally on my computer or remotely on my Android cell phone.
This means ideally you can organize your local files with a slick
consistent underlying system with a GUI customized to the current
enviorment.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

This DSL is essentially an API that will allow for easy local or remote
organization of locally stored pictures. This addresses the need by
allowing users to organize local files regardless of their location
(i.e. generally the best time to organize pictures, since it is a realitively
mindless task, is when you're on a bus, on a line, etc. and not sitting at
your computer where you could be doing something "more productive").

### Why you?
_What excites you about this idea? How did you come up with it?_

It is a project that would be very useful to me and one that I have made
several solutions for in the past. Originally, I made the first GUI-only
solution so my grandma, who is very uncomfortable with computers, could
organize some digital pictures without too many excessive features or buttons
that could be potentially confusing. After that I made a better GUI program
with more features that I have used. Now I essentially want to make this
DSL so I could run it as a server application with a remote GUIs.

### Domain
_Describe the project's domain in five words._

Extendable language for image organization.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

Like Git, I imagine this program will be made up of a number of useful
commands that are all launched from command line arguments. I imagine
macros, the interesting DSL aspect of this project, will be defined
in an init file similar to a .bashrc or .vimrc file. The syntax will
allow for easy access to file system level actions like moving and copying
files but also to accessing properties of pictures (i.e. date modified,
average color, dimensions, etc.)


### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs, ideally a photo is moved to a new directory. This action
can be either very explicit (i.e. the command specifically tells the file
where to go) or very macro based (i.e. the image is sent to the "red" folder
since red is the most prominent color). Since this language is entirely
action based, a given action will either succeed or fail. Since this language
aims to be extendable to GUIs, when an action fails, there will need to be
some standarized way (probably string) to communicate what went wrong to
the user.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

Moving files within the working directory should be easy. That being said,
although easy access to file system level actions is a must, security must
also be considered so no file accidently gets moved over important OS
files, etc. Thus, these file system level actions should probably be
restricted to a well defined "working directory."

Additionally, accessing image properties (i.e. dimensions, date modified) for
major image types (i.e. .jpg, .png, .bmp, .gif) as well as calculated properties
(i.e. average color, brightest pixel, etc.) should also be easy.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

Although many Adobe products contain extendable scripting languages (i.e. 
Photoshop, Lightroom, etc.), I have not been able to find any tool that fills
this exact set of requirements. While something like
[Adobe Lightroom](https://en.wikipedia.org/wiki/Adobe_Photoshop_Lightroom)
will probably provide users with a better set of tools for editing images
that I can ever make, it is more about managing a database than being a set
of commands with easy extendability to GUIs and network applications.

Additionally, although other "image organizing programs" can be found at either
this [link](https://en.wikipedia.org/wiki/Image_organizer) or this
[link](http://www.techsupportalert.com/best-free-digital-photo-organizer.htm),
none of them seem to provide this set of features.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

Although designing the various GUIs for this project, especially the App,
can be very time consuming and not directly related to the language aspects of
this project, the GUIs can be mostly overlooked for this project. At the end
of the day, the goal is to design a series of command line programs and
simple macro scripts are easily extendable and callable from a GUI, not make
the actual GUI. Although it would probably be nice to make a very simple
computer GUI to demonstrate how the language could be extended and called
from elsewhere, this could be kept very restricted to allow most of the
development to be directly related to the language design. 

### Scope
_How big an idea is this? How ambitious is this project?_

Although all the GUIs and App make this, overall, a very ambitious project,
by scaling it down as decribed above, this feels like a very reasonable
implementation of a command line program that makes use of an external DSL
script.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This might be a good project because it is very practical, seems well scoped,
and seems to provide tools that I have not been able to find elsewhere.

This might not be a good project because some of functionality will take
place entirely on the command line.