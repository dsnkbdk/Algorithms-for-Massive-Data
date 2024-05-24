# Project 4: Latent Factor Model with Stochastic Gradient Descent

## Overview
This project implements a collaborative filtering recommendation system using a Latent Factor Model (LFM) optimized with Stochastic Gradient Descent (SGD). The model aims to predict user ratings for items by factorizing the user-item interaction matrix into two lower-dimensional matrices that represent user preferences and item attributes.

## Key Features
- **Latent Factor Model (LFM)**: Decomposes the user-item matrix into latent factors to capture the underlying patterns in the data.
- **Stochastic Gradient Descent (SGD)**: Utilized to optimize the latent factor matrices by minimizing the prediction error iteratively.
- **Bias Terms**: Incorporates global, user-specific, and item-specific biases to enhance prediction accuracy.
- **Evaluation Metrics**: Uses Root Mean Square Error (RMSE) to evaluate the model's performance on validation and test datasets.

## Methodology
1. **Data Preprocessing**: 
   - Loads training, validation, and test datasets.
   - Calculates global bias, user-specific bias, and item-specific bias.

2. **Model Training**:
   - Initializes user and item latent factor matrices with random values.
   - Uses SGD to update the latent factors by minimizing the squared error between the predicted and actual ratings.
   - Applies regularization to prevent overfitting.

3. **Model Evaluation**:
   - Computes RMSE to assess the model's performance on the validation and test sets.
   - Plots RMSE for different values of the latent factors (`k`) to analyze the model's accuracy.

## Results
- The model's performance is evaluated using RMSE on the validation and test datasets.
- RMSE is computed for various values of latent factors to determine the optimal dimensionality for the latent space.
- The impact of incorporating bias terms on the model's accuracy is also analyzed.

## Conclusion
This project demonstrates the effectiveness of Latent Factor Models and Stochastic Gradient Descent in building a recommendation system. By factorizing the user-item interaction matrix and incorporating bias terms, the model achieves accurate predictions of user ratings. The evaluation results highlight the importance of selecting appropriate values for the latent factors and the benefits of including bias terms.

## Acknowledgments
This project is inspired by collaborative filtering techniques used in recommendation systems. The implementation and evaluation are based on common practices in the field of machine learning and data science.
