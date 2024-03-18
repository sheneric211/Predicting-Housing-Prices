# Predicting-Housing-Prices

## Project Overview
This project focuses on predicting housing prices in Barcelona using a variety of machine learning models. We explored and engineered features from housing data, including location, size, room count, and detailed descriptions, to train our models effectively.

## Feature Engineering
We meticulously processed and transformed the housing data to enhance model performance:
- **Location Processing**: Extracted and utilized town names from the `loc_string` feature for geographical insights.
- **Text Analysis**: Analyzed housing descriptions, creating a dictionary of 300 relevant lemmas, and vectorized descriptions for model input.
- **One-Hot Encoding**: Applied one-hot encoding to categorical variables, excluding inherently numerical features like size, rooms, and bathrooms.

Our final feature set comprised 325 distinct features, providing a comprehensive basis for our predictive models.

## Models and Techniques
We employed a range of machine learning models, each subjected to rigorous tuning and validation:
- **Random Forests**: Achieved a validation R-squared score of 0.64 with optimized hyperparameters.
- **Lasso and Ridge Regression**: Fine-tuned regularization parameters, obtaining R-squared scores of 0.56 and 0.58, respectively.
- **Support-Vector Regression**: Configured with optimal settings for a performance comparable to Lasso.
- **Neural Networks**: Experimented with a 4-layer architecture, though it did not surpass traditional models in effectiveness.
- **XGBoost and Catboost**: These gradient boosting models stood out, with Catboost leading at an R-squared score of 0.67.
- **Stacked Model**: A meta-regressor approach, using Catboost as the meta-regressor, achieved a superior R-squared score of 0.69.

## Lessons Learned
Our exploration into housing price prediction reinforced several key insights:
- Gradient-boosting methods, particularly Catboost, exhibit remarkable predictive power.
- Random forests, with minimal tuning, can yield robust predictions.
- Ensemble techniques like blending and stacking significantly enhance model reliability and reduce variance.
- Neural networks may be less suited for structured tabular data compared to more specialized algorithms.

## Visualizations and Artifacts
![Feature Importance](https://github.com/sheneric211/Predicting-Housing-Prices/assets/103718326/3cf6a352-f0bd-4c67-af67-4a076792176f)


## Contributors
- [Eric Shen](https://github.com/sheneric211) - Feature Engineering, Model Development & Tuning
- [Ireri Avila](https://github.com/ireriavila) - Feature Engineering, Model Tuning
