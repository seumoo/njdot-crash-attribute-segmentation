# Attribute Segmentation of New Jersey State Vehicle Crash Data
[Machine Learning Nanodegree Capstone Project]

This repository contains the files for my Machine Learning (ML) capstone project. The goal of this project was to identify crash patterns across New Jersey municipalities by using K-Means clustering algorithms and Principal Component Analysis (PCA) to summarize crash attributes. Crash attributes are characteristics of a crash such as:
- alcohol use
- weather conditions
- street lighting type
- person's injury severity

Additionally, this project also compares PCA and clustering results between Amazon Sagemaker and Scikit-learn to identify any differences between the two ML libraries.

### Problem Statement
The New Jersey Department of Transportation (NJDOT) publishes crash data based on police reports. From 2014 through 2018, there are over 5 million crash data points with each point having over 20 columns representing an attribute such as "alcohol used" or "weather conditions". The sheer volume of textual data makes it difficult to identify correllations between multiple crash attributes. Data analysis questions I wanted to explore include:
- What attributes have the highest importance across all crash points?
- Are there crashes across NJ which have similar groups of attributes?
- Where are these groups located?
- How can this analysis help engineers prevent future crashes?

### Technologies & Libraries Used
This project utilizes Jupyter Notebooks with Python 3.8 to perform all data analysis and ML tasks. The two ML libraries used are:
1. **Amazon Sagemaker**: an open source ML library for Python integration. Training models uses Amazon's cloud servers and incurs a fee for training time and uptime.
2. **SciKit-learn**: a free ML library that is easily imported in any Python enviornment. Training models is free and dependent on your hardware.

### Data Source and Processing
Crash data is publicilly avaliable on the New Jersey Department of Transportation website. The data contains over 5 million crash data points, each point having over 20 columns representing an attribute such as "alcohol used" or "weather conditions". 

### Results



## Repository Structure
The following section explains this repository's structure and contents.

### Reports
The following are technical documentation for the project:
1. **Capstone Report**: details the project goals, methodology, and results. 

### Juypter Notebooks


### Additional Materials
Supporting material is found in the Additional Materials folder which includes all images of component makeup charts, attribute value heatmaps, cluster makeup Excel, raw data before pre-processing, and normalized dataset used to train the PCA and K-means model.
