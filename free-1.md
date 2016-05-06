# Free project 1

## The user and a language
This section describes who the project would serve and why a language might be a
good way to meet their needs.


### What's the need?
Currently, it is difficult for a non-technical user to create a personal
website with enough flexibility. Also, it is difficult for such a user to 
understand the concepts behind how websites work such as the front-end and
back-end. The DSL would be typed in Microsoft Word or Powerpoint and be able to 
hook in and Excel spreadsheet essentially creating a dynamic website.


### Why a language?
I think a DSL would be a good fit for this because Word documents are
similar to web framework templates which use a DSL. A DSL would allow
users to work in a familiar environment (MS Office) with just a few changes
in syntax. 



### Why you?
I am excited about this idea because it could bring website creation to 
another user base of non-technical users. Originally it was a joke that 
some of my coworkers over the summer had. The joke was that people with 
no development experience would create a website with Microsoft Office. 
Word and Powerpoint would be the front-end and Excel would be the back-end.
As the saying goes, "There is a grain of truth in every joke."


### Domain
Website creation with Microsoft Office


### Interface (syntax)
I imagine the interface being something like web templates for popular 
frameworks such as Django. In Django, you can reference a variable from
the backend with the syntaxt {{ var_name }}. I could imagine changing
this to reference the row/col in an excel file e.g. {{ A4 }}.


### Operation (semantics)
The program would take in Word documents and Excel spreadsheets as input
and create a html website as output. There could be many possible errors
that would need to be communicated to the user such as syntax errors or
file_not_found errors. Perhaps I could create an error checker for this.


### Expressiveness
It should be easy to create a simple dynamic web page with the language. 
It would be difficult to put anything on the website that you cannot put
in a Word document. Anything besides making a website would most likely
be impossible. 


### Related work
I do not think there are any other DSLs in this specific language however, 
there are tools that address the need that I am trying to address. Programs
such as Wordpress allow non-technical users to create personal websites. There
are also an almost unlimited number of websites on which you can create a personal
site. A few are listed below.

+ https://wordpress.com
+ http://www.wix.com
+ http://www.squarespace.com
+ http://www.weebly.com

## The Project
This section examines whether the idea makes for a good CS 111 project.


### Suitability
I would think that the project would be more of working on the system of the 
language rather than language design, although I do not see a shortage of work
for language design. 

### Scope
This project is somewhat ambitious. I don't know how to parse word documents. I 
do know that there are libraries in python for writing to Excel files so that 
part would not be difficult. Also Word already has an option for turning a
document into an HTML file so that part would not be difficult. 


### Benefits and drawbacks
This would be a good idea for a project because it seems like the right amount
of work and also seems like a fun language to implement. I would be implementing
for users on the opposite end of the technical spectrum than myself so it would
realy make me think from a different perspective. I also see this as a good way
to get Microsoft Office users introduced to the ideas of programming. A SQL 
database in essence is the same as an Excel spreadsheet and Word document is the
same as an HTML file. Perhaps if users saw it from that perspective, they could 
better grasp the concepts. A drawback of this project is that it may never get used. 
Anyone who is non-technical enough to use this DSL would probably never be able to 
find it on the internet. Especially if it were only on GitHub. 

