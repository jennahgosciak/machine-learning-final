# Machine Learning for Cities Final Project

The purpose of this repository is to keep all materials used in developing the final class project for Spring 2022 Machine Learning for Cities course.

The report that corresponds to this analysis is available [here](https://docs.google.com/document/d/1T1InD_ZbMtyMqE9pm8Ek6AF-Qwg7OlPeFKRd-EmGCIQ/edit?usp=sharing).

The Project Team:
* Ariadne Rivera
* Danielle Bayer
* Jennah Gosciak
* Kai Elwood-Dieu

The objective:
* Identify neighborhood and built environment characteristics linked to structural fires in residential buildings
* Accurately predict where fires might occur in NYC

# Repository structure

## a) Data preparation

1. [Calculate catchment area for the proportion of census tract each alarm box serves](code/00a_calculate_catchment.ipynb)
2. [Process building data PLUTO](code/00b_data_processing.ipynb)
3. [Clean census data at the census tract level](code/00c_census2009_2019_data_processing.ipynb)
4. [Clean building HPD/DOB violations](code/00d_HPD_DOB_violations_data_processing.ipynb)

## b) Create analytic files

1. [Building level dataset](code/01_merge_bbl.ipynb)
2. Alarm box level dataset has two steps
    * [Merge boxes fire and census tract data](code/merge_boxes_boroughs.ipynb.ipynb)
This code merges census tract data at the fire alarm box level, based on the weights for the proportion of census tract each.

    * [Fire alarm box level dataset](code/02_merge_box.ipynb.ipynb.ipynb)
This code merges fire alarm box with census tract data with other databases.

## c) Analysis Alarm Box Level
1. [Decision tree and random forest](code/04a_rf_bayesnet_box.ipynb)
2. [Bayes Net](code/04a_rf_bayesnet_box.ipynb)
3. [Cluster analysis](code/06a_K_Means_EM_Box_Level.ipynb)
4. [SVM](code/05_SVMs.ipynb)
5. [Naive bayes](code/04b_naivebayes_gp_bbl.ipynb)

## d) Analysis Building Level
1. [Decision tree and random forest](code/03a_rf_bayesnet_bbl.ipynb)
2. [Bayes Net](code/03a_rf_bayesnet_bbl.ipynb)
3. [Cluster analysis](code/06b%20K-Means%20EM%20-%20BBL.ipynb)
4. [SVM](code/05_SVMs.ipynb)
5. [Naive bayes](code/03b_naivebayes_gp_bbl.ipynb)

* This [program](code/05a_pr_prob_box.ipynb) generated maps at the alarm box level.
* This [program](code/05a_pr_prob_bbl.ipynb) generated maps at the building level.
