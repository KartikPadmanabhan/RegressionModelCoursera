# Useful links:

**Github Page** For Project: https://github.com/KartikPadmanabhan/RegressionModelCoursera

**gh-page branch** for Project Report:   http://kartikpadmanabhan.github.io/RegressionModelCoursera/mtcars.html 


# HTML Rendering

We make use of bootstrap to add beauty to html report. To install bootstrap please install it the following way:

```
library(devtools)
install_github('rstudio/rmarkdown')
install.packages('knitr', repos = c('http://rforge.net', 'http://cran.rstudio.org'),
                 type = 'source')
install_github('jimhester/knitrBootstrap')
```

To knit an Rmd file to use with bootstrap in order to generate the html report as shown in the project report please do something like this from rstudio:

```
knit_bootstrap('mtcars.Rmd')
options(rstudio.markdownToHTML =
            function(inputFile, outputFile) {
                require(knitrBootstrap)
                knit_bootstrap_md(input=inputFile, output=outputFile)
            }
)
```

Reference: http://cran.r-project.org/web/packages/knitrBootstrap/knitrBootstrap.pdf

## Project Goal 

Take the mtcars data set and write up an analysis to answer their question using regression models and exploratory data analyses.

Your report must be:

    * Written as a PDF printout of a compiled (using knitr) R markdown document.
    * Do not use any packages that are not in R-base or the library datasets.
    * Brief. Roughly the equivalent of 2 pages or less for the main text. Supporting figures in an appendix can be included up to 5 total pages including the 2 for the main report. The appendix can only include figures.
    * Include a first paragraph executive summary.

Upload your PDF by clicking the Upload button below the text box.

Peer Grading

    * The criteria that your classmates will use to evaluate and grade your work are shown below. 
    * Each criteria is binary: (1 point = criteria met acceptably; 0 points = criteria not met acceptably)
    * Your Course Project score will be the sum of the points and will count as 40% of your final grade in the course. 
    
