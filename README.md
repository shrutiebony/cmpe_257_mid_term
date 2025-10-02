
The colab file link is: https://colab.research.google.com/drive/10-e_5gziwPk9ZB0SCFeeID_zJAuL0_cZ#scrollTo=tMMP9j5wRRRg

## Housing Insights & Clustering Project
### Overview
The majority of property sites allow users to filter properties based on price, size, and location. However, soft criteria such as safety, proximity to schools/hospitals, and pollution levels also play a huge role in a property’s value.
This project explores housing datasets to uncover deeper patterns that balance affordability, safety, and investment potential. Using clustering and visualization, we aim to help buyers and investors make smarter, fact-based choices.

#### Data Narrative
Combined three datasets to build a rich, diverse housing dataset:
1) Kaggle Dataset 1 (Zillow housing data)
2) Kaggle Dataset 2 (Zillow housing data)
These datasets cover 100M+ homes in the U.S., including features like:
1) Location (state, city, neighborhood)
2) Property specifications
3) Market value estimates
4) Nearby amenities

#### Installation & Requirements
Run the following in Colab to install required dependencies:
'''
!pip install uv
!uv pip install sweetviz --system
!uv pip install umap-learn --system
!pip install ydata-profiling
'''
#### Python Libraries Used
1) Pandas / NumPy → Data cleaning & manipulation
2) Matplotlib / Seaborn / Plotly → Data visualization
3) Sweetviz / ydata-profiling → Exploratory Data Analysis (EDA)
4) UMAP → Dimensionality reduction
5) Scikit-learn → Clustering & machine learning
### Features & Workflow
##### 1. Data Preparation
1) Imported, cleaned, and merged datasets
2) Handled missing values & duplicates
3) Standardized feature columns
##### 2. Exploratory Data Analysis (EDA)
1) Distribution of property prices, sizes, and locations
2) Correlation heatmaps
3) Automated reports via Sweetviz & ydata-profiling
##### 3. Feature Engineering
1) Created derived features (affordability index, safety score, etc.)
2) Normalized numerical values for clustering
##### 4. Clustering & Dimensionality Reduction
1) Applied UMAP for visualization in 2D space
2) Used KMeans / DBSCAN to cluster properties
3) Identified groups of homes balancing affordability, safety, and investment potential
##### 5. Insights
1) Which neighborhoods balance low cost + high safety
2) Which regions are strong investment prospects
3) Patterns across states and cities
##### 6. Results
1) Clear separation of property clusters in UMAP visualizations
2) Actionable insights for buyers & investors (affordable yet safe zones, hotspots for growth)
3) A reusable pipeline for housing market analysis


### How to Run
1) Open the notebook in Google Colab.
2) Run all cells sequentially.
3) Explore EDA reports, cluster visualizations, and insights.


### Repository Structure
Housing.ipynb        # Main Jupyter/Colab notebook
README.md            # Project documentation
data/                # Raw and cleaned datasets (if uploaded)
outputs/             # Visualizations and profiling reports
