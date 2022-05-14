# Attribute Segmentation of New Jersey State Vehicle Crash Data
[Udacity Machine Learning Nanodegree: Capstone Project]

## Table of Contents
- [Attribute Segmentation of New Jersey State Vehicle Crash Data](#attribute-segmentation-of-new-jersey-state-vehicle-crash-data)
  - [Table of Contents](#table-of-contents)
  - [Project Overview](#project-overview)
  - [Technologies & Libraries Used](#technologies--libraries-used)
  - [Problem Statement](#problem-statement)
  - [Methodology](#methodology)
    - [Principal Component Analysis (PCA)](#principal-component-analysis-pca)
    - [K-means Clustering](#k-means-clustering)
  - [Results](#results)
- [Repository Structure](#repository-structure)
  - [Reports](#reports)
  - [Juypter Notebooks](#juypter-notebooks)
  - [Additional Materials](#additional-materials)
  
## Project Overview
This repository contains my Machine Learning (ML) capstone project files. This project aimed to identify crash patterns across New Jersey municipalities by using Principal Component Analysis and K-Means clustering algorithms to identify crash attribute trends. Crash attributes are characteristics of a crash, such as:
- alcohol use
- weather conditions
- street lighting type
- person's injury severity

This analysis identified New Jersey municipalities that had crashes with similar groups of attributes. Engineers can then identify problematic locations with these attribute groups, potentially implementing safety measures to prevent future crashes.

## Technologies & Libraries Used
This project utilizes Jupyter Notebooks with Python 3.8 to perform all data analysis and ML tasks. The two ML libraries used are:
1. **Amazon Sagemaker**: an open-source ML library for Python integration. Training models use Amazon's cloud servers and incur a fee for training time and uptime.
2. **SciKit-learn**: a free ML library easily imported into any Python environment. Training models are free and dependent on your hardware.

## Problem Statement
The New Jersey Department of Transportation publishes crash data based on police reports. From 2014 through 2018, there were over 5 million crash data points, with each point having over 20 columns representing an attribute such as "alcohol used" or "weather conditions". The sheer volume of textual data makes it challenging to identify correlations between multiple crash attributes. 

The following are data analysis questions I wanted to explore:
- What attributes have the highest importance across all crash points?
- Are there crashes across NJ which have similar groups of attributes?
- Where are these groups located?
- How can this analysis help engineers prevent future crashes?

## Methodology
Because many stakeholders involved in safety programs use crash data containing serious injuries or fatalities, crash data containing a serious injury or fatality were kept. The resulting dataset was reduced to 6,800 crashes. 

Next, data was pre-processed to prepare for K-means clustering. Because K-means clustering requires numerical data, all categorical data was encoded and normalized (Tables 1 & 2). This step resulted from 20 attributes to 174 attributes. 

<figcaption><b>Table 1: Data with categorical attributes</b></figcaption>

| Location | Alcohol Involved | Weather Condition |
|----------|------------------|-------------------|
| 1        | Yes              | Rain              |
| 2        | No               | Dry               |

<figcaption><b>Table 2: Data with encoded attributes</b></figcaption>

| Crash ID | Alcohol Involved Yes | Alcohol Involved No | Weather Condition Rain | Weather Condition Dry |
|----------|----------------------|---------------------|------------------------|-----------------------|
| 1        | 1                    | 0                   | 1                      | 0                     |
| 2        | 0                    | 1                   | 0                      | 1                     |


Due to the larger number of attributes, it will be difficult for a K-means model to determine the most important attributes. Therefore, principal component analysis was used to reduce the number of attributes.

### Principal Component Analysis (PCA)
PCA reduces the number of column attributes by removing redundant attributes and maintaining attributes with the highest weight. A 70% variance was chosen resulting in the top 25 attributes to be chosen. After reducing the dataset, the data was used to train a K-means model for attribute segmentation.

### K-means Clustering
To identify crash attribute patterns, a K-means model was trained using the resulting dataset from PCA. K-means algorithms are ideal for identifying similarities or differences within groups; in this case, the algorithm will group 

## Results
The following tables 


# Repository Structure
The following section explains this repository's structure and contents.

    .
    ├── Additional Materials                 # Supporting material including all component makeup charts and heatmaps
    ├── Juypter Notebooks                    # Documentation files (alternatively `doc`)
    ├── Reports                              # PDF files of the Capstone Report and Proposal
    └── README.md                              

## Reports
The following are technical documentation for the project:
1. **Capstone Report**: details the project goals, methodology, and results. 

## Juypter Notebooks


## Additional Materials
Supporting material is found in the Additional Materials folder which includes all images of component makeup charts, attribute value heatmaps, cluster makeup Excel, raw data before pre-processing, and normalized dataset used to train the PCA and K-means model.
