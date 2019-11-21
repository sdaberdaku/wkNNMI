# wkNNMI

wkNNMI is an R tool for the imputation of static and dynamic mixed-type data. A typical example of this kind of data are clinical registers containing subsequent screening visits for several patients.

## Reference
**An adaptive Mutual Information-weighted k-NN algorithm for the imputation of static and dynamic mixed-type data**

Tavazzi E., Daberdaku S., Vasta R., Calvo A., Chiò A., Di Camillo B.

## Installation

#### Installation from GitLab

wkNNMI is available on GitLab at https://gitlab.com/sysbiobig/wkNNMI

To install wkNNMI from GitLab, please use the following commands:
```r
library(devtools)
install_gitlab("sysbiobig/wkNNMI")
```


#### Installation from source package

The wkNNMI R package can be downloaded at http://sysbiobig.dei.unipd.it/?q=wkNNMI

It requires the *infotheo* and *foreach* packages to work.

To install it from source, please use the following command:
```r
install.packages("wkNNMI_X.X.X.tar.gz", repos = NULL, type = "source")
```
where "X.X.X" indicates the package version.

## Getting started

The package contains two functions *impute.subject* and *impute.wknn*. Load the package and check the documentation of the two methods.

```r
library(wkNNMI)
?impute.subject
?impute.wknn
```

