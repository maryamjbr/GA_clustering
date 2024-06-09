# Iris Dataset Analysis and Clustering using Genetic Algorithm

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset Fetching and Exploration](#dataset-fetching-and-exploration)
3. [Data Visualization](#data-visualization)
4. [Dimensionality Reduction](#dimensionality-reduction)
5. [Genetic Algorithm for Clustering](#genetic-algorithm-for-clustering)
6. [Results](#results)
7. [Dependencies](#dependencies)
8. [How to Run](#how-to-run)

## Introduction

This project focuses on analyzing the Iris dataset, a well-known dataset in the field of machine learning. The primary objective is to explore and visualize the data, reduce its dimensionality for better understanding, and apply a genetic algorithm to perform clustering.

## Dataset Fetching and Exploration

The Iris dataset is fetched from the UCI Machine Learning Repository. It contains 150 samples from three species of iris flowers (Setosa, Versicolor, and Virginica), with four features measured for each sample: sepal length, sepal width, petal length, and petal width. The dataset is then explored to understand its structure and the variables it contains.

## Data Visualization

Several visualization techniques are applied to the dataset to gain insights into the relationships between different features. This includes creating pair plots and scatter plots, which help in understanding how the features of the different iris species compare and contrast with each other.

## Dimensionality Reduction

Principal Component Analysis (PCA) is used to reduce the dimensionality of the dataset from four to two components. This makes it easier to visualize and analyze the data. PCA helps in identifying the directions (principal components) in which the data varies the most.

## Genetic Algorithm for Clustering

A genetic algorithm is implemented to perform clustering on the Iris dataset. The genetic algorithm includes:
- Initialization of a population of possible solutions (chromosomes).
- Crossover and mutation operations to create new offspring from the current population.
- Evaluation of the fitness of each solution using the Adjusted Rand Index (ARI).
- Iteration until an optimal solution is found or a stopping criterion is met.

The goal of the genetic algorithm is to find the best clustering of the iris data points into their respective species.

## Results

The genetic algorithm successfully clusters the Iris dataset into three groups, corresponding to the three species of iris flowers. The final clustering solution is visualized using a scatter plot, demonstrating how the genetic algorithm has grouped the data points based on their features.

## Dependencies

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `ucimlrepo`

Install the dependencies using:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn ucimlrepo
```

## How to Run

1. Clone this repository.
2. Install the dependencies.
3. Run the script to fetch the dataset, visualize the data, perform PCA, and apply the genetic algorithm for clustering.

```bash
python script_name.py
```

Replace `script_name.py` with the name of your script file.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
