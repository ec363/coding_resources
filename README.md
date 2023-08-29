# Coding Resources for Molecular Biologists

This is a list of resources that I, as a wet lab molecular biologist working in synthetic biology, have found helpful for learning to code. The vast majority of the resources are by no means exclusive to molecular/cellular biologists, but I will probably have a particular perspective for what is important and useful as a result of my background. It is centred around the R language, but also includes other important tools such as GitHub for version control and Markdown for text editing in coding-friendly formats. This document will be continually updated as/where appropriate.

---

### R

The two most widely-used languages in my field are R and Python. In an ideal world one would probably learn both, however people often have preferences depending on their immediate needs/the language they are most comfortable with. I think for the basics of learning to code and data visualisation, it doesn't matter which you use. It is often smartest to learn the language most used by those around you, and/or the language that is being most actively developed specifically for the application you require it for, if your use case is somewhat specialised.

You will often hear that R is a statistical language, developed for statisticians and data scientists. This is true, but this is not all R is. R has been under active development for biological data analysis for about 20 years. R was conceived in 1992, became popular in 2000, and the Bioconductor project began in 2001. [Bioconductor](http://www.bioconductor.org/) is a project that hosts bioinformatics-specific packages for the analysis of **high-throughput sequencing data**, but also includes packages specific for the analysis of other kinds of data, such as from **flow cytometry**. It has an estimated 1000 active developers and 300,000 active users (source: [Credibly Curious](https://soundcloud.com/crediblycurious/episode-1-cran-and-bioconductor)). So R is well-placed to be the language of choice for these specialised bioinformatics use-cases. But it can just as justifiably be used for the analysis of smaller and less specialised data sets (indeed I use it for that all the time), particularly since its **data visualisation capabilities are incredibly powerful** (in other words, it's easy to use R to make really stunning figures). Beyond this, both developers and users of R, as a community, are proactively open source and uphold a friendly attitude to newcomers, and there are now countless projects whose objective is to make the language easier to use and applicable to a broader and broader set of applications.

In short, I'd recommend it.

* __Where to start__
  * [What is R?](https://www.r-project.org/)
  * How to use R on your computer:
  	* either:
  	* (a) download R & an application that lets you write and test R code easily
  		* Download R (and extra packages) from the [Comprehensive R Archive Network, aka **CRAN**](https://cran.r-project.org/).
  		* Download [**RStudio**](https://rstudio.com/products/rstudio/): a desktop app (also known as an "interactive development environment" or IDE) which makes working with R a lot nicer than not having an IDE (it will help you organise your code, data and plots).
  		* If you have an Anaconda distribution downloaded and you use Jupyter Notebooks for Python coding, it might have RStudio bundled with it or [easily installable](https://anaconda.org/r/rstudio) [from within the bundle](https://docs.anaconda.com/anaconda/navigator/tutorials/create-r-environment/). Jupyter Notebooks [can also be configured to run code written in R](https://docs.anaconda.com/anaconda/navigator/tutorials/r-lang/). I haven't tried either of these yet, however.
  	* or:
  	* (b) use R in the cloud
  		* [**RStudio Cloud**](https://rstudio.cloud/learn/guide) lets you write, test and save scripts in a browser environment.
  	* Of all these options, **I would recommend RStudio**.

* __General R tutorials__
  * I learnt the basics of R using a free online course that no longer exists. But plenty of others do. Searching for one that others specifically recommend is a good move to find the highest quality starting points. 
  * See ['Data Science Guide'](https://github.com/Chris-Engelhardt/data_sci_guide) for a great list.
  * See ['How to Learn R'](https://www.r-bloggers.com/how-to-learn-r-2/) for a nice intro.
  * [Swirl](https://swirlstats.com/students.html) is an R package for interactive R learning from within RStudio: a very nicely implemented idea. Besides a few introductory courses that can be accessed as soon as you get started, more can be found [here](https://github.com/swirldev/swirl_courses#swirl-courses) and [here](http://swirlstats.com/scn/title.html).

* __Specific R tutorials__ (for applications relevant to biologists)
  * [__R for Data Science__](https://r4ds.had.co.nz/introduction.html) is a great book that deals with how to use R for handling data and visualising it.
    * Don't worry about the name, Data Science is just the name given to any task that deals with (a) importing (b) analysing (c) plotting/visualising data (ie. everything you might use Excel for). this is an everyday thing for biologists, you don't need to be dealing with terabytes of data to need these tools.
  * __ggplot2__ is probably the major package in the life of experimentalists with a requirement for data visualisation. Start [here](https://ggplot2.tidyverse.org/) for a good introduction.
  * __R for Biochemists__ is a layperson's course run specifically to familiarise biochemists with R. It deals with the basics of R, data import, plotting (eg. RNAseq log2 plots and enzyme kinetics data) and curve fitting. The link to the course is on the [Biochemistry Society webpage](https://biochemical-society.myshopify.com/collections/frontpage/products/r-for-biochemists-101-starting-30-march-2010) and the accompanying blog is [here](http://rforbiochemists.blogspot.com/).

* __Reference sheets__
  * ggplot2 Cheatsheet: [pdf download link](https://github.com/rstudio/cheatsheets/raw/master/data-visualization-2.1.pdf)
  * [ggplot2 functions](https://ggplot2.tidyverse.org/reference/)
  * [ggplot2 cookbook](http://www.cookbook-r.com/Graphs/)
  * [other cheat sheets](https://rstudio.com/resources/cheatsheets/)
  * [Collection of Errors, Warnings and Messages in R](https://github.com/rmflight/rerrors)
  * [The R manual](https://cran.r-project.org/doc/manuals/r-release/R-intro.html): literally a dry reference manual.

* __Books__ I'd recommend.
  * [R Cookbook, by J. Long and Paul Teetor](https://rc2e.com/)
  * [R for Data Science, by Garrett Grolemund and Hadley Wickham](https://r4ds.had.co.nz/)

---

### Other programming languages

Curated lists of courses (online and in person) can be found here:

* [Data Science Guide](https://github.com/Chris-Engelhardt/data_sci_guide)
* [Coder Newbie Advice](https://github.com/charlottebrf/coder-newbie-advice)

---

### Markdown

Markdown is essentially a way of writing formatted files in plain text: like HTML but easier. You've probably come across very similar 'lightweight' text editing methods before, such as in messaging apps that let you **bold** text written between asterisks (\*) or put text in _italics_ when wrapped with underscores (\_). Markdown was designed to be unobtrusive (readable) and convertible into other file types. More flexible than Word, simpler to learn than HTML or LaTeX. It is useful for annotating code, as code can be inserted within markdown documents (eg. "R markdown"/Rmd type of markdown documents). It has been adopted by many platforms including GitHub (note GitHub renders .md files but not .Rmd files). This file is written in Markdown and converted to HTML (rendered) when a user clicks on a folder ('repository'/'directory') within which which a markdown file called README.md exists: on the GitHub page, click on 'README.md', then 'Raw' to see this file in plain text, as it was written.

* [Markdown reference](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [GitHub flavor markdown](https://help.github.com/en/articles/basic-writing-and-formatting-syntax)
* [R markdown reference 1](https://rmarkdown.rstudio.com/authoring_basics.html) & [2](https://rstudio.com/wp-content/uploads/2015/03/rmarkdown-reference.pdf)
* R markdown [examples](https://rmarkdown.rstudio.com/gallery.html) - used for reports, data analysis workflows, lab notebooks.. 

---

### GitHub

GitHub is useful for many things: as a backup system that makes it easy to see what was changed in each version ('version control'), for sharing code and for contributing to group projects. The latter two are the most talked about aims of GitHub, but you needn't use it to publish code or collaborate for it to be useful; I find versioning the most useful aspect. Git is the language that allows the tracking of changes to files within a folder ('repository'), and GitHub is the most popular site that uses Git for syncing such changes.

The language of Git is very weird at first and takes time to get used to. I'd recommend working through the Git commands via command line like in Blischak's paper to start. For most applications however, I use GitHub Desktop, a much nicer and more intuitive interface than command line.

* Start here:
  * [**Blischak 2016**: A Quick Introduction to Version Control with Git and GitHub](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004668)
  * [**GitHub Desktop**](https://desktop.github.com/) 
* Tutorials:
  * [GitHub Getting Started Guide](https://help.github.com/en/categories/getting-started-with-github)
  * [GitHub Guides](https://guides.github.com/)
  * [Git and GitHub learning resources](https://help.github.com/en/articles/git-and-github-learning-resources)
  * [Perez-Riverol, 2016: Ten Simple Rules for Taking Advantage of Git and GitHub](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004947). __See Table 2 for a list of tutorials.__ 
  * [Wickham, 2015: Git and GitHub](http://r-pkgs.had.co.nz/git.html) 

---

### Troubleshooting 

There is a sort of truism in coding that there is always an answer to a question on Google. This is true, though finding the right way to phrase a question and/or getting an answer that is written in an accessible way can be a challenge. Still, a mixture of asking people, Googling and reading reference texts is often the way to get to the answer. 

* Most of the helpful answers to my Google queries turn out to be entries on the following sites:
  * StackOverflow https://stackoverflow.com 
  * STHDA http://www.sthda.com/english/
  * Data Novia blog https://www.datanovia.com/en/blog/

---

### Organisations focused on education & community-building in coding/data science

A number of interesting organisations provide free and informal guidance on coding and related topics. Their forums are also great places to ask technical questions and meet like-minded people.

* [**R-Ladies**](https://rladies.org/) - an international community of women who use R 
* [**R4DS**](https://twitter.com/r4dscommunity) - a community of those learning/using R for Data Science
* [**Researc/Hers Code**](https://www.researcherscode.com/) - a London-based group working to promote women who use coding in their research 
* **#tidytuesday** - an initiative to get R users to practise their data wrangling and visualisation skills by making visualisations of a new sample dataset each week and sharing their code/plots on [Twitter](https://twitter.com/hashtag/tidytuesday) and [GitHub](https://github.com/rfordatascience/tidytuesday)

---

**Articles and Resources on Related Topics**

### How to learn to code

* ['The ten commandments for learning how to code' by Atma Ivancevic](https://www.nature.com/articles/d41586-019-00653-5)

### How to manage computational biology projects

* [Noble, 2009: A Quick Guide to Organizing Computational Biology Projects](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000424)
* [Boettiger, 2012: Research Workflow](https://www.carlboettiger.info/2012/05/06/research-workflow.html)
* [NiceR code, 2013: Designing Projects](https://nicercode.github.io/blog/2013-04-05-projects/)
* [Wilson, 2014: Best Practices for Scientific Computing](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001745)
* The Turing Way: an [online book](https://the-turing-way.netlify.app/) and [github repository](https://github.com/alan-turing-institute/the-turing-way) on Reproducibility in Data Science

### Data visualisation

* [Claus O. Wilke, Fundamentals of Data Visualization](https://serialmentor.com/dataviz/)

