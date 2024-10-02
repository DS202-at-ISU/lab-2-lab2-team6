
<!-- README.md is generated from README.Rmd. Please edit the README.Rmd file -->

# Lab report \#1

Follow the instructions posted at
<https://ds202-at-isu.github.io/labs.html> for the lab assignment. The
work is meant to be finished during the lab time, but you have time
until Monday evening to polish things.

Include your answers in this document (Rmd file). Make sure that it
knits properly (into the md file). Upload both the Rmd and the md file
to your repository.

All submissions to the github repo will be automatically uploaded for
grading once the due date is passed. Submit a link to your repository on
Canvas (only one submission per team) to signal to the instructors that
you are done with your submission.

```
remotes::install_github("heike/classdata")
library(classdata)
install.packages("ggplot2")
library(ggplot2)
data()
str(ames)

ggplot(ames, aes(x=`Sale Price`)) + geom_histogram(binwidth = 500) + ggtitle("binwidth - 500")

max(ames$`Sale Price`, na.rm=TRUE)
The range of the variable Sale Price is 0-20,500,000. The highest value is a very far outlier, which most Sale Price values lying between 100,000 and 500,000. Additionally, there were quite a few listed as 0.

data.frame(ames$`Sale Price`)
```
