# Attribute Segmentation of New Jersey State Vehicle Crash Data
[Machine Learning Nanodegree Capstone Project]

This repository contains my Machine Learning (ML) capstone project files. This project aimed to identify crash patterns across New Jersey municipalities by using Principal Component Analysis and K-Means clustering algorithms to identify crash attribute trends. Crash attributes are characteristics of a crash, such as:
- alcohol use
- weather conditions
- street lighting type
- person's injury severity

This analysis identified New Jersey municipalities that had crashes with similar groups of attributes. Engineers can then identify problematic locations with these attribute groups, potentially implementing safety measures to prevent future crashes.

### Technologies & Libraries Used
This project utilizes Jupyter Notebooks with Python 3.8 to perform all data analysis and ML tasks. The two ML libraries used are:
1. **Amazon Sagemaker**: an open-source ML library for Python integration. Training models use Amazon's cloud servers and incur a fee for training time and uptime.
2. **SciKit-learn**: a free ML library easily imported into any Python environment. Training models are free and dependent on your hardware.

### Problem Statement
The New Jersey Department of Transportation (NJDOT) publishes crash data based on police reports. From 2014 through 2018, there were over 5 million crash data points, with each point having over 20 columns representing an attribute such as "alcohol used" or "weather conditions". The sheer volume of textual data makes it challenging to identify correlations between multiple crash attributes. 

The following are data analysis questions I wanted to explore:
- What attributes have the highest importance across all crash points?
- Are there crashes across NJ which have similar groups of attributes?
- Where are these groups located?
- How can this analysis help engineers prevent future crashes?

### Methodology
Because many stakeholders involved in safety programs use crash data containing serious injuries or fatalities, I analyzed crash data containing a serious injury or fatality. This reduced the dataset to 6,800 data points. 

To identify crash patterns, the following ML tools were used:
1. **Principal Component Analysis**: reduces the number of column attributes by removing redundant attributes and maintaining attributes with the highest weight
2. **K-means Clustering**: 

### Results



## Repository Structure
The following section explains this repository's structure and contents.

    .
    ├── Additional Materials                 # Compiled files (alternatively `dist`)
    ├── Juypter Notebooks                    # Documentation files (alternatively `doc`)
    ├── Additional Materials                 # Source files (alternatively `lib` or `app`)
    └── README.md

### Reports
The following are technical documentation for the project:
1. **Capstone Report**: details the project goals, methodology, and results. 

### Juypter Notebooks


### Additional Materials
Supporting material is found in the Additional Materials folder which includes all images of component makeup charts, attribute value heatmaps, cluster makeup Excel, raw data before pre-processing, and normalized dataset used to train the PCA and K-means model.
