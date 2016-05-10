# Scheduling

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.

This project would serve users looking for a faster way to create and expand schedules. The DSL would "codify" scheduling by converting some text-based representation of the schedule into valid Google Calander or iCal format. This language might be a good way to meet the needs of people who enjoy the convenience of online schedules but find the process of filling it out and making changes or adding events very laborious. It might seem a bit silly at first to create an entire DSL for the sole purpose of saving a few minutes, but consider git. Github has both a terminal interface and a desktop alternative. Although some may consider the desktop interface to be limited in its functionality and less efficient than the terminal interface, others may find this more user-friendly and harder to mess up. Similarly, some may find terminal too hard to use or too easy to potentially mess up the repository. 

### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

This idea helps make scheduling easier by allowing for a text-based alternative. For instance, people who simply want to type up a few lines to generate a schedule for their semester classes rather than having to manually click and add each of their classes individually in the iCal interface. Rather than having to navigate through the calander to the specified month and date, potential users could simply write a one line command to schedule an event. Perhaps the biggest experience change with this DSL is that users would not have to actually open their calender app to input their schedule. As of now, users have to open their calender app and manually click through and create all their events.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL is appropriate because it streamlines the process for certain users. This DSL definitely appeals to a niche category of users that much prefer function over form. As someone always on the computer, it would be nice if I could simply schedule an event within a few seconds rather than having to open a browser, go to the calender app, and add it. 

### Why you?
_What excites you about this idea? How did you come up with it?_

I know that I am a forgetful person and would benefit exceptionally from a planner or calender of some sort; however, I find myself too lazy to actually go out of the way to create an event or reminder in Google Calenders or iCal, especially if the event is within a few days or even a few hours. It's ironic because it is these events that tend to be the most important. What excites me is the idea of simply oepning my computer, typing a command in terminal or some other environment and have the reminder automatically created.

### Domain
_Describe the project's domain in five words._

Scheduling made for lazy people


### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

The user would simply type a series of commands that would compile into a .csv format. I imagine the program would be very simplistic and similar to terminal commands, something along the lines of "schedule: 3/20, 9pm - 10pm, hwk" or "schedule: 1/6, 1pm - 4pm, e59 class, repeat until 5/1." I think this is the right way to interact with scheduling because something made with the intention of improving time management shouldn't waste time.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When the program runs, the commands are compiled into a valid .csv format that can be easily imported into a calender app. The program interacts with the user by taking their commands, which are in relatively readable code, and making them nicely formatted. Some errors that might occur include not filling out required fields or messing up the sequence of arguments, since (based off of the above example) it's pretty arbitrary right now.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

The expressiveness is super limited for this language, as the domaind of "scheduling" isn't particularly extensive. It should be easy to schedule! It should be impossible or very very difficult to do anything else, really. 

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

The [ASPC Scheduler](https://aspc.pomona.edu/courses/schedule/) kind of does this with class schedules in that it takes a schedule and formats it into a .csv or .ics to allow for easy importing. However, it is still a lot of clicking and querying for classes. If the user already knows what classes he or she is taking, and when they are, they should not have to go through the process of individually searching for the class and adding the class. 

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I imagine most of the work would be on the "systems" aspects, as the language is pretty simplistic in terms of the syntax. I'm sure there are ways in which we could emphasize language design decisions more, such as taking in arguments in an arbitrary order and recognizing what they are. Because there is some degree of natural language embedded in it, building some form of parsing might be also a good amount of work (I consider this parsing to be part of the language aspect, but I'm not sure if others do).

### Scope
_How big an idea is this? How ambitious is this project?_
This idea is very manageable compared to the other ones I've written about, and not very ambitious. Perhaps this project could be extended to handle class registration as well, which would increase the scope significantly since the implementer would have to handle some back end interactions with Portal.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_
This would be a good idea for a project because it is, by itself, extremely manageable and almost guaranteed to be completed by the end of the semester. Additionally, it is relatively easy to build upon it if the implementer were to finish this early. This might not be a good idea because it can easily just ignore the language aspect, which pretty much defeats the purpose of this course.
