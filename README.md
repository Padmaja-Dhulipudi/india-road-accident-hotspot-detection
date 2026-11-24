# 🚦 Indian Road Accident Hotspot Detection using DBSCAN

##  Project Overview

This project aims to identify geographical road accident hotspots in India using **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**.

Using Python and data mining techniques, the project analyses geographical accident locations to discover high-density regions and isolated incidents.

##  Objectives

- Identify geographical accident hotspots.
- Apply DBSCAN for density-based spatial clustering.
- Detect isolated incidents and noise points.
- Visualize geographical accident patterns.
- Generate meaningful insights from the dataset.

##  Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Folium

## Algorithm

**DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**

DBSCAN groups nearby geographical points based on density without requiring a predefined number of clusters.

The Haversine distance metric will be used to calculate distances between geographical coordinates.

## 📂 Project Structure

```text
india-road-accident-hotspot-detection/
│
├── data/
├── outputs/
├── notebooks/
├── main.py
├── requirements.txt
├── README.md
└── .gitignore
```

##  Project Workflow

1. Dataset collection
2. Data cleaning and preprocessing
3. Exploratory Data Analysis
4. DBSCAN clustering
5. Hotspot identification
6. Interactive map visualization
7. Results and insights

## Results and Observations

DBSCAN clustering was performed independently for eight Indian cities using the Haversine distance metric.

**Model parameters:**
- Algorithm: DBSCAN
- Epsilon: 1.0 km
- Minimum Samples: 5
- Distance Metric: Haversine

### City-wise Results

| City | Number of Clusters | Noise Percentage |
|---|---:|---:|
| Bangalore | 129 | 18.91% |
| Chandigarh | 1 | 0.00% |
| Chennai | 1 | 0.54% |
| Delhi | 168 | 41.88% |
| Hyderabad | 123 | 19.47% |
| Kolkata | 4 | 0.78% |
| Mumbai | 93 | 12.60% |
| Pune | 7 | 1.11% |

### Key Findings

- Delhi produced the highest number of clusters (168).
- Bangalore and Hyderabad also showed a relatively high number of clusters.
- Chandigarh produced one cluster with no noise records.
- The number of clusters varied considerably across cities.
- DBSCAN classified records that did not meet the density requirements as noise.

### Limitations

- The dataset's real-world provenance and accuracy have not been independently verified.
- Results should be interpreted as exploratory clustering of the supplied records, not confirmed real-world accident hotspots.
- DBSCAN results depend heavily on the selected epsilon and minimum-samples parameters.
- A single parameter combination may not be equally suitable for every city.
- Noise points are not necessarily errors or unimportant records.

### Conclusion

This project demonstrates how DBSCAN can be applied to geographical accident-record data using the Haversine distance metric. The city-wise analysis shows how density-based clustering identifies spatial groups and noise points. It also demonstrates practical applications of data mining, geographic data processing, and visualization using Python.

##  Future Enhancements

- City-wise hotspot analysis
- Accident severity analysis
- Time-based accident pattern analysis
- Interactive Streamlit dashboard

## Project Status

Currently under development.

