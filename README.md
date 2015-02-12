# Version Control with Git

A collection of content related to a seminar on the nature and use of version
control as defined with Git. This content was presented during the spring
semester of 2015 at the University of Montana. 

The purpose of the seminar is to provide a introductory exposure to fundamental
git to enable students to use version control more effectively within their
coursework and professional work. This begins by exploring the abstract
structures within git while functionally exploring the git command set. This
provides a foundational understanding of git that can extended upon in practice
as well as a working knowledge of tools utilizing git.

## Build

Content is written using markdown and compiled into revealjs slides to be served 
from the web.

I use [pandoc][pandoc_home] to convert the markdown notes to html
[revealjs][revlealjs_home] slideshows. This is not pertinient to git but illustrates 
my process.

> `pandoc -t revealjs -s notes/*.md -o notes/*.html`

Subsequently, I use python to start a simple webserver to server the slideshows.

> `python -m http.server`

[pandoc_home]: http://johnmacfarlane.net/pandoc/
[revealjs_home]: https://github.com/hakimel/reveal.js/
