# Version Control with Git

A collection of content related to a seminar on the nature and use of version
control as defined with Git. This content was presented during the spring
semester of 2015 at the University of Montana.

## Build

Content is written using markdown and compiled into revealjs slides to be served 
from the web.

`pandoc -t revealjs -s notes/*.md -o notes/*.html`
`python -m http.server
