# Coding Resources

A list of resources that I have found helpful for learning to code, centred around the R language, but including other important tools such as GitHub for version control and Markdown for text editing in coding-friendly formats.  

---

### R

* __Where to start__
  * What is R https://www.r-project.org/ 
  * Download R (and extra packages) https://cran.r-project.org/
  * Download RStudio - a desktop app (also known as an "interactive development environment" or IDE) which makes working with R a lot nicer than not having an IDE (it will help you organise your code, data and plots) https://rstudio.com/products/rstudio/

* __General R tutorials__
  * I learnt R using a free online course that no longer exists. But plenty of others do.
  * See Data Science Guide for a great list https://github.com/Chris-Engelhardt/data_sci_guide 
  * See How to Learn R for a nice intro https://www.r-bloggers.com/how-to-learn-r-2/
  * Swirl (is an R package for interactive R learning) https://swirlstats.com/students.html 
  * R For The Rest Of Us (looks good) https://rfortherestofus.com/ 
  * R manual (a little dry for the beginner) https://cran.r-project.org/doc/manuals/r-release/R-intro.html 

* __Specific R tutorials__ (for applications relevant to biologists)
  * __R for Data Science__ https://r4ds.had.co.nz/introduction.html
    * don't worry about the name, Data Science is just the name given to any task that deals with (a) importing (b) analysing (c) plotting/visualising data (ie. everything you might use Excel for). this is an everyday thing for biologists, you don't need to be dealing with terabytes of data to need these tools.
  * __ggplot2__ probably the major package in the life of experimentalists with a requirement for data visualisation. start here: https://ggplot2.tidyverse.org/
  * __R for Biochemists__
    * blog: http://rforbiochemists.blogspot.com/ 
    * course: https://biochemistry.org/events/r-for-biochemists-101-sept-2019/ a layperson's course run specifically to familiarise biochemists with R and deals with the basics of R, data import, plotting (eg. RNAseq log2 plots and enzyme kinetics data) and curve fitting.

* __Reference sheets__
  * ggplot2 cheat sheet https://github.com/rstudio/cheatsheets/raw/master/data-visualization-2.1.pdf & functions https://ggplot2.tidyverse.org/reference/ & cookbook http://www.cookbook-r.com/Graphs/
  * other cheat sheets https://rstudio.com/resources/cheatsheets/ 

* __Books__
  * R Cookbook, by J. Long and Paul Teetor https://rc2e.com/
  * R for Data Science, by Garrett Grolemund and Hadley Wickham https://r4ds.had.co.nz/

---

### Other programming languages

Curated lists of courses (online and in person) can be found here:

* Data Science Guide https://github.com/Chris-Engelhardt/data_sci_guide 
* Coder Newbie Advice https://github.com/charlottebrf/coder-newbie-advice

---

### Markdown

Markdown is a way of writing formatted files in plain text, essentially. Like HTML but easier. You've probably come across very similar 'lightweight' text editing methods before, like in other apps that let you **bold** text written between *s or put text in _italics_ when wrapped with _s. Markdown was designed to be unobtrusive (readable) and convertible into other file types. More flexible than Word, simpler to learn than HTML or LaTeX. It is useful for annotating code, as code can be inserted within markdown documents (eg "R markdown"/Rmd type of markdown documents). It has been adopted by many platforms including GitHub (note GitHub renders .md files but not .Rmd files). This file is written in Markdown: on the GitHub page, click on 'README.md', then 'Raw' to see it in plain text, as it was written.

* Markdown reference https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
* GitHub flavor markdown https://help.github.com/en/articles/basic-writing-and-formatting-syntax 
* R markdown reference https://rmarkdown.rstudio.com/authoring_basics.html & https://rstudio.com/wp-content/uploads/2015/03/rmarkdown-reference.pdf
* R markdown examples - used for reports, data analysis workflows, lab notebooks.. https://rmarkdown.rstudio.com/gallery.html

---

### GitHub

GitHub is useful for many things, for version control, for understanding what you've changed in your code, and for annotating why you made certain changes to certain code. You needn't use it to collaborate for it to be useful. Git is the language that allows tracking of changes to files within a repository (folder), and GitHub is the most popular site using Git for syncing changes, sharing code and collaborating with others. 

The language of Git is very weird at first and takes time to get used to. I'd recommend working through the Git commands via command line like in Blischak's paper to start. For most applications however, I'd use GitHub Desktop, a much nicer interface than command line.

* Start here:
  * Blischak 2016: A Quick Introduction to Version Control with Git and GitHub https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004668
  * GitHub Desktop https://desktop.github.com/ & https://help.github.com/en/desktop/getting-started-with-github-desktop
* Tutorials:
  * GitHub Getting Started Guide https://help.github.com/en/categories/getting-started-with-github
  * GitHub Guides https://guides.github.com/
  * Git and GitHub learning resources https://help.github.com/en/articles/git-and-github-learning-resources
  * Perez-Riverol, 2016: Ten Simple Rules for Taking Advantage of Git and GitHub (__see Table 2 for list of tutorials__) https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004947
  * Wickham, 2015: Git and GitHub. http://r-pkgs.had.co.nz/git.html

---

### Troubleshooting 

* Google first!
* Most Google queries link me to:
  * StackOverflow https://stackoverflow.com 
  * STHDA http://www.sthda.com/english/
  * Data Novia blog https://www.datanovia.com/en/blog/

---

### Organisations focused on education & community-building in coding/data science

* R-Ladies https://rladies.org/
* R4DS https://twitter.com/r4dscommunity
* Researc/Hers Code https://www.researcherscode.com/
* #tidytuesday https://github.com/rfordatascience/tidytuesday https://twitter.com/hashtag/tidytuesday

---

**Articles and Resources on Related Topics**

### How to learn to code

* 'The ten commandments for learning how to code' by Atma Ivancevic
https://www.nature.com/articles/d41586-019-00653-5

### How to manage computational biology projects

* Noble, 2009: A Quick Guide to Organizing Computational Biology Projects https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000424
* Boettiger, 2012: Research Workflow https://www.carlboettiger.info/2012/05/06/research-workflow.html
* NiceR code, 2013: Designing Projects https://nicercode.github.io/blog/2013-04-05-projects/
* Wilson, 2014: Best Practices for Scientific Computing https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001745

### Data visualisation

* Claus O. Wilke, Fundamentals of Data Visualization https://serialmentor.com/dataviz/

