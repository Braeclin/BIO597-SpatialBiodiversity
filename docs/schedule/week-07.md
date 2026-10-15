# Week 07: Building a complete SDM w/ a machine learning model

## Icebreaker

If you could bring back any fashion trend, what would it be?

## Paper discussion

- Allie will be leading the discussion this week of Aoyama et al 2020
["Incorporating diversity measures into Ecological Site Descriptions to manage
biodiversity on heterogeneous landscapes"](https://doi.org/10.1016/j.rala.2020.05.002)

# Lab Exercise: Building a more complete SDM w/ Machine Learning


* Next, the usual intro update exercise: Go to your
[JupyterHub](https://maine.cloudbank.2i2c.cloud/) and pull the latest version
of the class github repository.

## Core Questions

- How does a random forest learn a species–environment relationship from presence and background cells?
- Why can a random train/test split overstate performance at unsampled locations?
- What happens when we train in southern Maine and test in northern Maine, then reverse the regions?
- How can we identify environmental conditions outside the training sample, and why are predictions there harder to trust?
- What can disagreement between two regional models tell us about model uncertainty?
- Which climate variables does the forest use most, and does importance imply an ecological cause?
- Why is a presence/background suitability score different from a probability of occurrence?

## Concepts

- Train/test splitting
- Spatial cross-validation
- Environmental extrapolation and novelty
- Model uncertainty
- Variable importance

## Python Tools

- scikit-learn
- GeoPandas
- NumPy
- pandas
- xarray
- Matplotlib

## Applied Lab

Students build a presence/background SDM for a Maine amphibian using
`scikit-learn`'s `RandomForestRegressor` and the supplied occurrence–climate
table and Maine bioclimatic raster stack. In short, guided steps, they
train a forest, test it on withheld cells, map suitability, and plot
variable importance. A north/south comparison introduces spatial
cross-validation, unfamiliar temperatures, and disagreement between models.

- [Lab 07: Machine Learning SDMs](../labs/lab07-MachineLearningSDM.ipynb)

## Assignment

Repeat the workflow for a chosen amphibian species, justify predictor
choices, and compare random testing with testing in a different region.
Submit a completed notebook with maps, short interpretations, and one
saved suitability raster. Use the lab's model settings throughout.

- [Assignment 07: Machine Learning SDMs](../assignments/Assignment-07-MachineLearningSDM.ipynb)

**Paper discussion leader next week:** Next week we will need to do 2 papers
so everyone has a chance to lead over the semester. So, **Meg & Hao!** Please each
select a (hopefully shorter) paper for the group to discuss before Sunday 10/18
6pm and send it around to the class email list: bio597-fall2026-group@maine.edu
