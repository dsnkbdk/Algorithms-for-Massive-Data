# Project 2: Track Frequency Analysis

## Overview

This project focuses on analyzing the frequency of tracks from a given dataset of playlists. The key objective is to extract tracks, compute their frequencies, and visualize the distribution of these frequencies to gain insights into the popularity and occurrence of tracks within the dataset.

## Key Technologies

### JSON
Utilized for loading and parsing the dataset from a JSON file, enabling easy access and manipulation of the data.

### Collections (Counter)
The `Counter` class from the `collections` module is used to count the frequency of tracks efficiently. It provides a straightforward way to tally occurrences and sort them in descending order.

### Pandas
A powerful data manipulation library that allows for the creation and handling of DataFrames. In this project, Pandas is used to convert frequency data into a structured format for easier analysis and visualization.

### NumPy
Used for numerical operations and setting random seeds to ensure reproducibility of the results. NumPy's functions facilitate efficient computation and manipulation of numerical data.

## Data Analysis Techniques

1. **Data Loading**: The dataset is loaded from a JSON file, which contains a collection of playlists, each with multiple tracks.
2. **Track Extraction**: Tracks are extracted from the playlists and stored in a list, with each track represented by its name and a portion of its URI.
3. **Frequency Calculation**: The total number of tracks, the number of unique tracks, and the average frequency of tracks are computed to provide basic statistical insights.
4. **Frequency Counting**: The `Counter` class is used to count the frequency of each track, and the results are sorted in descending order.
5. **Data Conversion**: The frequency data is converted into a Pandas DataFrame for easier manipulation and analysis.
6. **Visualization**: A scatter plot is generated using Matplotlib to visualize the frequency distribution of tracks, providing a clear view of their popularity and occurrence.

## Visualization
The scatter plot created in this project displays the frequencies of all tracks in descending order. This visualization helps in understanding the distribution and identifying the most frequent tracks within the dataset.

## Reproducibility
To ensure that the results are reproducible, random seeds are set using the `random.seed` and `np.random.seed` functions. This guarantees that the analysis can be repeated with consistent results.

## Usage
This project can be used as a template for similar data analysis tasks involving frequency analysis and visualization of categorical data. It demonstrates the use of various Python libraries to load, process, and visualize data effectively.

## Conclusion
By leveraging the mentioned technologies and data analysis techniques, this project provides a comprehensive approach to analyzing and visualizing track frequencies in a playlist dataset. The insights gained from this analysis can be useful for understanding the popularity and trends of tracks within the given data.
