This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

This problem set is based on the content of the paper "The Consequences of Industrialization: Evidence from Water Pollution and Digestive Cancers in China" written by Avraham Ebenstein (2012). Its aim is to investigate if contaminated water in China's rivers and lakes influences the digestive cancer death rate. The interactive structure of the problemset together with descriptions of economic theory and explanations of R commands grant a diversified and informative journey through the topic.

The paper can be found online at https://scholars.huji.ac.il/sites/default/files/avrahamebenstein/files/ebenstein_waterpollution_2012.pdf.

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.
```s
if (!require(devtools))
  install.packages("devtools")
source_gist("gist.github.com/skranz/fad6062e5462c9d0efe4")
install.rtutor(update.github=TRUE)

devtools::install_github("brigittepeter/RTutorWaterPollutionChina", upgrade_dependencies=FALSE)
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.
```s
library(RTutorWaterPollutionChina)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorWaterPollutionChina")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorWaterPollutionChina",
       load.sav=TRUE, sample.solution=FALSE)
```
If everything works fine, a browser window should open, in which you can start exploring the problem set.
