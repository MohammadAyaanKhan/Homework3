# DSCI 552 — Homework 3

Name : Mohammad Ayaan Khan

USC ID: 4147952900

Email ID : mkhan736@usc.edu

Time series classification on the AReM dataset (feature creation and extraction), plus ISLR exercise 3.7.4.

## Contents

`Homework3.ipynb` — The solution involves the entire process of feature creation. It involves downloading the AReM dataset, applying the prescribed training/testing split, extracting seven respective time-domain features (minimum, maximum, mean, median, standard deviation, first quartile, third quartile) from each of the six sensor series, determining the standard deviation for each of the features with a 90% bootstrapping confidence interval, and choosing three features, together with the answer to question ISLR 3.7.4.

## How to run

1. Install the dependencies: `pip install numpy pandas matplotlib seaborn scikit-learn`
2. Open the notebook and run cells: `jupyter notebook Homework3.ipynb`

The notebook downloads the AReM dataset from the UCI repository automatically. Therefore there is no need to download any data files, but it is necessary to have an Internet connection 

## Notes

- The prescribed data split implies that datasets 1-2 are stored in `bending1`/`bending2` and datasets 1-3 are retained in other folders as test data, and thus, we get 19 as test data and 69 as training instances out of 88.

- The notebook stops in case it does not load precisely 88 data instances or if any data file does not have 480 valid sensor rows.
