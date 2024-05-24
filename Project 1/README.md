# Project 1: Locality-Sensitive Hashing (LSH) for Article Similarity

## Overview

This project implements a Locality-Sensitive Hashing (LSH) algorithm to find similar articles based on their signature matrices. LSH is an efficient algorithm for approximate nearest neighbor search in high-dimensional spaces, making it suitable for tasks like document similarity and recommendation systems.

## Introduction

Locality-Sensitive Hashing (LSH) is a technique used to hash input items in such a way that similar items map to the same buckets with high probability. This project demonstrates the use of LSH for finding similar articles by hashing their signature matrices and identifying articles with the same hash bucket.

## Installation

To run this project, you'll need the following dependencies:
- Python 3.x
- numpy
- matplotlib
- Jupyter Notebook

## Algorithm Details

The key steps of the algorithm are as follows:

1. **Signature Matrix Creation**: The input data is transformed into a signature matrix, where each item (article) has a set of signatures.
2. **Hash Function**: The `g_hash_function_k8` function hashes the signature matrix. Random coefficients and a prime number are used to compute the hash values.
3. **Signature Extraction**: The signatures of each article are extracted from the signature matrix.
4. **Finding Same Bucket**: Articles with the same bucket number as the target article are retrieved.
5. **Evaluation**: The true positives (TP), false positives (FP), and false negatives (FN) are calculated for different values of `k`.

## Evaluation

The evaluation is performed by calculating the TP, FP, and FN for different values of `k` (2, 4, 8). The average FP and FN values are computed and printed.

## Results

The results are visualized using matplotlib, showing the average FP and FN values against `k`. This helps in understanding the performance of the LSH algorithm for different band sizes.
