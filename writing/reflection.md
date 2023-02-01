# CMPSC 480: Portfolio project reflection

Follow guidelines in the README to complete

I've decided to use 11ty for my personal website project and the theme for my portfolio site is roxo by StaticMania. 

The first challenge I've come across is understanding the overall structure of the theme and how 11ty layouts its projects.

Solution: I just played around with the project repository by changing variables and trying to understand the connection between files to understand the overall structure of the website. Basically, the whole structure of the project is that everything is compiled into one big HTML called "index.html" in the "_site" folder. The "base.njk" is the foundation file as the name suggests. Every nunjuck files in the layouts folder are compiled into "base.njk" which compiles into "index.html", and those nunjuck files themselves get their data from the "_data" folder. Everything is styled according to "style.css" file in the CSS folder in assets.

The second challenge I encountered is that I wanted to display my projects as one column on the home page, but the theme was set up in a way that it was showing projects by 2x2 grid, and when I changed the images of the projects it messed up the alignment.

Solution: I experimented with the "homepage.njk" file and figured out that the theme was using bootstrap to display rows and columns. Then, I did research on how to change columns and rows in bootstrap and found out that I can move the projects section out of the "row" div and move it into its div to make it one column. Also, there was a problem with my project images not displaying correctly. I fixed the issue by adding padding-bottom to the parent div and adding "height: 100%;" to the image CSS.

The third challenge I came across for this project was that I needed to completely redo the design for the about page. Firstly, I deleted all the styles related to about page and cleaned up the about.njk file to start fresh.