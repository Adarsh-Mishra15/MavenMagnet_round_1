# Body Wash Review Analysis Project

## Brief Description

This project focuses on analyzing customer reviews for body wash products. It involves processing review data, performing predictive modeling to identify key factors influencing customer satisfaction, and generating insights from the analysis. The project utilizes machine learning techniques to predict factors such as fragrance, brand value, efficacy, and skin care based on review text.

The analysis is conducted using Jupyter notebooks, with datasets for training and testing models. Results include predicted factors for test reviews, stored in CSV format.

## Process

### 1. Data Collection and Preparation
- **Datasets**: The project uses two primary datasets:
  - `datasets/bodywash-train.xlsx`: Training data containing body wash reviews with labeled factors.
  - `datasets/bodywash-test.xlsx`: Test data for evaluating model predictions.
- Data preprocessing involves cleaning review text, handling missing values, and preparing features for modeling.

### 2. Model Development
- **Notebooks**:
  - `notebook/bodyWash.ipynb`: Main notebook for data exploration, model training, and evaluation using traditional machine learning approaches.
- Techniques may include natural language processing (NLP), classification models, and AI-driven factor prediction.

### 3. Prediction and Evaluation
- Models are trained on the training dataset to predict factors from review text.
- Predictions are generated for the test dataset and saved to `result/bodywash-test-final.csv`.
- Evaluation metrics assess model performance, such as accuracy, precision, and recall for each predicted factor.

### 4. Results Interpretation
- The final results file (`result/bodywash-test-final.csv`) contains original reviews paired with predicted factors, enabling insights into common themes in body wash reviews.

## Data Analysis

### Key Insights from Reviews
Based on the analysis of the provided data, common factors predicted in body wash reviews include:
- **Fragrance**: Scent quality and longevity.
- **Brand Value**: Overall brand perception and loyalty.
- **Efficacy**: Effectiveness in cleaning and moisturizing.
- **Skin Care**: Impact on skin health, dryness, and irritation.
- **Cleansing**: Ability to remove dirt and residue.
- **Price**: Value for money and affordability.
- **Product Texture**: Lather quality and consistency.

### Example Analysis
- Reviews often highlight positive aspects like pleasant scents and skin softness, while negative feedback focuses on dryness, strong odors, or ingredient concerns.
- Predictive models achieve varying accuracy depending on the factor, with fragrance and efficacy being commonly well-predicted.

### Visualizations and Further Exploration
- Notebooks include exploratory data analysis (EDA) with plots for factor distributions, word clouds for review themes, and model performance charts.
- Use the notebooks to reproduce analysis or experiment with different models.

## Summary

This project demonstrates the application of data science and AI in consumer product review analysis. By predicting key factors from text, it provides valuable insights for product development, marketing, and customer satisfaction improvement in the body wash market.

### Getting Started
1. Clone or download the repository.
2. Ensure Python and required libraries (e.g., pandas, scikit-learn, transformers for Gemini integration) are installed.
3. Open the notebooks in Jupyter and run cells sequentially.
4. Review the results in `result/bodywash-test-final.csv`.

### Dependencies
- Python 3.x
- Jupyter Notebook
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn (for analysis)
- For Gemini notebook: google-generativeai or relevant API access

### Future Enhancements
- Integrate more advanced NLP models.
- Expand dataset for better generalization.
- Add real-time prediction capabilities.

For questions or contributions, feel free to reach out.
