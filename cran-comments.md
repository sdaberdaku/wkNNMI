## Resubmission

This is a resubmission of 1.0.1. In this version I have fixed NEWS.md, which
was not in a format R can parse ("No news entries found" in the incoming
pre-tests).

## Resubmission of an archived package

wkNNMI was archived on 2023-08-19 because email to the maintainer address
(sebastian.daberdaku@unipd.it) became undeliverable: I left the University of
Padua and the account was closed. I am the same maintainer, now at
sebastiandaberdaku@gmail.com. The old address cannot receive a confirmation.

Changes in 1.0.1:

* New maintainer email address.
* Added the reference to the published paper in the Description, a CITATION
  file, and the URL and BugReports fields.

## Test environments

* Docker rocker/r-ver, R 4.6.1, Ubuntu 24.04
* Docker rocker/r-devel, R-devel (2026-10-19 r90708)

## R CMD check results

0 errors | 0 warnings | 1 note

* checking CRAN incoming feasibility ... NOTE
  New submission. Package was archived on CRAN (archived on 2023-08-19 as
  email to the maintainer is undeliverable; see above).

  Possibly misspelled words in DESCRIPTION (NN, Tavazzi, et, al): "k-NN" is
  the usual abbreviation of k-nearest neighbours, and "Tavazzi et al." is the
  reference to the paper describing the method.
