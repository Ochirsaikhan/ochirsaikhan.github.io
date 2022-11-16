# CMPSC 480: Portfolio project reflection

Follow guidelines in the README to complete

I've decided to use 11ty for my personal website project and the theme for my portfolio site is roxo by StaticMania. 

The first challenge I've come across is understanding the overall structure of the theme and how 11ty layouts its projects.

Solution: I just played around with the project repository by changing variables and trying to understand the connection between files to understand the overall structure of the website. Basically, the whole structure of the project is that everything is compiled into one big HTML called "index.html" in the "_site" folder. The "base.njk" is the foundation file as the name suggests. Every nunjuck files in the layouts folder is compiled into "base.njk" which compiles into "index.html", and those nunjuck files themselves get their data from the "_data" folder. Everything is styled according to "style.css" file in CSS folder in assets. 