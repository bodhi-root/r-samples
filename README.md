# R Samples

GitHub Pages: https://bodhi-root.github.io/r-samples/

## Overview

This is a place to put sample R notebooks with re-usable code.  The site
is built using R Markdown and the helpful guide here:

* http://nickstrayer.me/RMarkdown_Sites_tutorial/
* https://rmarkdown.rstudio.com/rmarkdown_websites.htm

As an FYI (since I get paranoid about space usage): the bare-bones "hello world"
sample had 65 files and total 3.56 MB of data (mostly the JavaScript and
stylesheet libraries).  This isn't too bad.

## Editing

To add new pages to this website simply:

* Create a ".Rmd" file similar to those that already exist
* Run the "build_site.R" script to build the site
* Commit the code to github

NOTE: I originally had the website going to the "docs" folder (since github
can pick it up from here).  However, that ended up duplicating a lot of
content.  It copied all of the notebooks in the "notebooks" folder over into
"docs/notebooks".  The new method is what the blog recommended: outputting the
website to ".". This will create ".html" files for all of the ".Rmd" files in
the base directory, but it won't touch the R notebooks in "notebooks".  This
works out well, and you can link to the ".nb.html" files for the notebooks.
