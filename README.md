# wkNNMI

wkNNMI is an R tool for the imputation of static and dynamic mixed-type data. A typical example of this kind of data are clinical registers containing subsequent screening visits for several patients.

This package implements an adaptive weighted k-nearest neighbours (wk-NN) imputation algorithm for clinical register data developed to explicitly handle missing values of continuous/ordinal/categorical and static/dynamic features conjointly. For each subject with missing data to be imputed, the method creates a feature vector constituted by the information collected over his/her first *window_size* time units of visits. This vector is used as sample in a k-nearest neighbours procedure, in order to select, among the other patients, the ones with the most similar temporal evolution of the disease over time. An *ad hoc* similarity metric was implemented for the sample comparison, capable of handling the different nature of the data, the presence of multiple missing values and include the cross-information among features.

## Installation

The package needs the R packages *infotheo* and *foreach*.

From CRAN:

```r
install.packages("wkNNMI")
```

From GitHub:

```r
# install.packages("remotes")
remotes::install_github("sdaberdaku/wkNNMI")
```

## Getting started

The package contains two functions *impute.subject* and *impute.wknn*. Load the package and check the documentation of the two functions.

```r
library(wkNNMI)
?impute.subject
?impute.wknn
```

## Citation

If you use wkNNMI, please cite:

> Tavazzi E, Daberdaku S, Vasta R, Calvo A, Chiò A, Di Camillo B. Exploiting mutual information for the imputation of static and dynamic mixed-type clinical data with an adaptive k-nearest neighbours approach. *BMC Medical Informatics and Decision Making* 20(Suppl 5), 174 (2020). https://doi.org/10.1186/s12911-020-01166-2

`citation("wkNNMI")` prints the same reference.

## License

GPL-3
