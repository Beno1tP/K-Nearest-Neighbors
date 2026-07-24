# Air Quality and Pollution Assessment using K-Nearest Neighbors (kNN)

## Overview
This is an academic project for an "Introduction to AI" course (since 2024), focusing on the research and application of the basic **K-Nearest Neighbors (kNN)** algorithm. The primary goal is to classify air quality and pollution levels based on various environmental attributes, such as $SO_2$, $NO_2$, $CO$, and Proximity to Industrial Areas. 

The project involves data preprocessing, exploratory data analysis, dimensionality reduction (LDA), kNN model evaluation, and visualizing the decision boundaries.

## Project Structure
The project is divided into 6 main steps, each contained in its own directory:

- **`step1_preprocess_dataset/`**: Data cleaning, handling missing values, and splitting the main dataset (`final_pollution_dataset.csv`) into training, validation, and test sets.
- **`step2_correlation_matrix/`**: Computing and visualizing the correlation matrix to understand the relationships between different environmental attributes.
- **`step3_lda_analysis/`**: Performing Linear Discriminant Analysis (LDA) to reduce dimensionality and better visualize class separability.
- **`step4_plot_data/`**: Basic data visualization techniques (scatter plots, etc.) to examine the distribution of the attributes.
- **`step5_plot_k/`**: Finding the optimal number of neighbors ($k$) and the optimal distance metric parameter ($p$) for the kNN algorithm by plotting accuracy/error against various values.
- **`step6_classification_map/`**: Generating 2D (and pseudo-3D) decision boundaries for the kNN algorithm to visualize how the model partitions the feature space across chosen attributes.

## Dataset
The primary dataset used is `final_pollution_dataset.csv` (and related cleaned/updated versions). It contains features related to air quality parameters that are used as inputs for the kNN model to predict the pollution class or level.

## Future Work
Due to time constraints, this project is limited to exploring the fundamental, standard implementation of the kNN algorithm. Advanced methods of kNN (e.g., optimized search structures like KD-Trees, distance weighting, and other nonparametric discrimination optimizations) could not be implemented at this stage.

Exploring these advanced methods is considered for future work, building upon foundational theories of nonparametric discrimination. 
For reference on these theoretical foundations and advanced justifications, please refer to:
> **[1]** E. Fix and J. L. Hodges, Jr., "Discriminatory Analysis. Nonparametric Discrimination: Consistency Properties," *Technical Report*, USAF School of Aviation Medicine, Randolph Field, Texas, 1951.

## How to Run
Navigate into the respective step directories and run the Python scripts or Jupyter Notebooks.
For instance, to run the classification map generation:
```bash
cd step6_classification_map
python classification_map.py
```
