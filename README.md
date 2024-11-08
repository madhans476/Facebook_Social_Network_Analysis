# Social Network Analysis of Food Pages

This project explores the structure, connectivity, and influence of food-related pages on social networks, using social network analysis (SNA) metrics. The analysis aims to uncover important nodes (influencers), community structures, and potential future connections among these pages.

## Table of Contents
- [Project Overview](#project-overview)
- [Files and Directory Structure](#files-and-directory-structure)
- [Setup and Installation](#setup-and-installation)
- [Data Analysis](#data-analysis)
- [Acknowledgments](#acknowledgments)

## Project Overview
This study leverages SNA techniques to analyze and interpret relationships within a network of food pages. The analysis includes metrics like PageRank, betweenness centrality, degree distribution, clustering coefficients, and link prediction to identify potential collaborations or partnerships among food brands and influencers.

## Files and Directory Structure
The main files in this repository include:
- `fb-pages-food.nodes`: Contains the nodes (pages) data with attributes.
- `fb-pages-food.edges`: Contains the edges (relationships) data between nodes.
- `fb_network.ipynb`: A Jupyter Notebook file with the complete analysis using NetworkX, including visualizations and metric computations.

## Setup and Installation

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Required Python libraries (listed below)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. Install the required Python packages:

  To begin, install the necessary Python packages using `pip`:
  
  ```bash
  pip install networkx matplotlib pandas jupyter
  ```

3. Open the analysis notebook:
  Once the packages are installed, open the analysis notebook in Jupyter:
  ```bash
  jupyter notebook fb_network.ipynb
  ```
## Data Analysis

The analysis notebook (`fb_network.ipynb`) includes the following steps:

1. **Loading and Exploring the Data**  
   - Load the network data and inspect its structure.
   - Check basic statistics and explore the dataset to understand its properties.

2. **Calculating Network Metrics**  
   The following key network metrics are calculated:
   - **Degree Distribution**: Analyzing the distribution of the degree (the number of connections) across all nodes in the network.
   - **Degree Centrality**: Measures the number of direct connections a node has.
   - **Betweenness Centrality**: Measures the number of times a node acts as a bridge along the shortest path between two other nodes.
   - **Closeness Centrality**: Measures how close a node is to all other nodes in the network, based on the shortest paths.
   - **Connected Components**: Identifying and analyzing the distinct connected components in the network.
   - **Bridges**: Identifying edges whose removal would increase the number of connected components in the network.
   - **PageRank**: A ranking algorithm that assigns a score to each node based on its connectedness.
   - **All Pair Shortest Path**: Calculating the shortest path between every pair of nodes in the network.
   - **Clustering Coefficients**: Measures the degree to which nodes in a graph tend to cluster together.

3. **Link Prediction Metrics**  
   Several metrics for predicting potential links between nodes are calculated, including:
   - **Common Neighbors**: The number of neighbors that two nodes share.
   - **Resource Allocation Index**: A measure based on shared neighbors that assigns a score for link prediction.
   - **Jaccard Similarity**: Measures the similarity between two nodes based on the ratio of common neighbors to total neighbors.

4. **Visualizing the Network and Key Metrics**  
   - Visualize the network using `matplotlib` and `networkx`.
   - Create plots showing the distribution of key metrics such as degree centrality, betweenness centrality, and others.


## Acknowledgments

- Rossi, R. A., & Ahmed, N. K. (2015). The Network Data Repository with Interactive Graph Analytics and Visualization. AAAI. Available at [https://networkrepository.com](https://networkrepository.com).

