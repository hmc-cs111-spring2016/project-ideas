# Free project 2


## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help 
them?_

Many college students struggle to organize multiple homework assignments, classtimes, meetings, big projects with smaller parts, reoccuring due dates, a calendar for events, and a list of all the little things they need to do "at some point" during the week. They use checklists, calendars, todo lists, sticky notes and other resources, but there doesn't seem to be one resources that can take care of all of those needs in one place. I would like to build a DSL that would allow them to merge all of these things they need to do into one calendar, this would decrease stress and help them to more efficiently complete everything that they needed to do.

### Why a language?
_Why is a DSL appropriate for your user(s)? How does it address the need?_

A DSL would require the students to invest time in setting up their calendars but it would give them the flexibility, ease, and detailed control needed to put in all their due dates at the beginnning of the semester and then add additional pieces as they go. They could more easily express their busy lives in a calendar using this DSL than in the current, widely used software. A DSL is the appropriate tool, because this is a very limited, specific domain, but we want users to be able to easily express anything within it.

### Why you?
_What excites you about this idea? How did you come up with it?_

This seems so relevant to the lives of all college students. I have often felt frustrated with the difficulty of specifying exactly what I want on a calendar or of needing to use multiple tools to keep track of everything I am doing throughout the day. I was thinking about it some before I looked at any examples of past projects and was encouraged in my idea when I read about what NCarter3 did for his DSL in 2014 and what aputman did for his project in 2015.

### Domain
_Describe the project's domain in five words._

Organizing tasks and activities together.

### Interface (syntax)
_How might the user interact with the language? What does programming look 
like? Why is this the right way to interact with the problem domain?_ 

I would like to allow the user to type a command perhaps in terminal adding a new event or task and for them to immediantly see the updated result in their calendar. This would allow them to easily add new things to their calendar and if I create a simple documentation of what commands are available they can look up what kind of thing they want to add, type it in and then instantly see their result.

### Operation (semantics)
_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When a program runs a new event or activity should be added to the calendar and become visible to the user. Their might be errors if the user tries to use an invalid date or the parser does not understand an input and the program should return an error message with the word it cannot interpret or the invalid date.

### Expressiveness
_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

It should be easy to make a daily todo list, to carry events over from a previous day, to schedule appointments, including ones with complicated repitition patterns and set reminders. There shouldn't be very many things that are possible but difficult and it should be impossible to create a program that does anything beyond editing a calendar.

### Related work
_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well 
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

In 2014, NCarter3 created a similar DSL for CS111 [here](https://github.com/NCarter3/project/blob/master/documents/description.md). He attempted to "create a new DSL that wraps Todo.txt with powerful calendar calculations. Effectively, I want it to tell me what to do next and when to do it". His project focused on making a calendar more like a todo list which could tell him what activity he should do next. 

In 2015, aputman created a project along these lines [here](https://github.com/aputman/project/blob/master/documents/final.md) for CS111 as well. His idea was to focus on making it easier for users to scope "different events with different dates" for things like classes which meet several times during every week except during breaks and holidays or finals week when the schedule is different. I got my idea before I began researching but when I found these I liked them both and have borrowed ideas from both in this write up.

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I would need to spend time determining what language I wanted to implement my DSL in and how I might make use of existing code basis and programs since many things have been made which are similar to this, and I would just be combining them in a new way.

### Scope
_How big an idea is this? How ambitious is this project?_

Depending on what existing work I leverage this could be either a very big project or a very reasonable project but I might spend a lot of time determining how to leverage and intermingle existing programs.

### Benefits and drawbacks
_Why might this be a good idea for a project? Why might this not be a good idea 
project?_

This seems like a very interesting domain to work in and one that would be very useful, but there is already a lot of work that has been done in this area so its not very original. I would need to think more about what unique aspects my program would bring to its users.


