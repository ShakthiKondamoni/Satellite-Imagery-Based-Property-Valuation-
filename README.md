Project Overview
-------------------------------------------

Traditional models rely on either:

Satellite imagery (CNN-based) or

Tabular geospatial features (ML-based)

This project fuses both modalities to capture:

Spatial patterns from images

Structured numerical insights from metadata (latitude, longitude, etc.)

📈 Result: Improved predictive performance compared to unimodal models.

📂 Dataset Used
--------------------------------------

The dataset consists of structured data collected from reliable sources.

It includes both input features and target variables relevant to the prediction task.

Preprocessing steps applied:

Handling missing values

Feature scaling/normalization

Train–test split for evaluation

🧠 Approach and Models Used
--------------------------------------------------------------------------------

Multimodal Learning Pipeline
Satellite Images (.tif) ──► CNN Backbone ──► Image Embedding
                                              │
Tabular Features (CSV) ──► MLP / Dense ──► Tabular Embedding
                                              │
                                Feature Fusion (Concatenation)
                                              │
                               Fully Connected Regression Head
                                              │
                                     Continuous Prediction



Process Flow
----------------------------------------------------------------------------------------
1. Data Collection
2. Image Preprocessing (Resize, Normalize)
3. Tabular Data Cleaning & Scaling
4. CNN-based Image Feature Extraction
5. Feature Fusion (Image + Tabular)
6. Model Training
7. Model Evaluation (MSE, R²)

📈 Evaluation Metrics
----------------------------------------------------------------------------------------------------

The performance of the models was evaluated using the following metrics:

Root Mean Squared Error (RMSE)

R2 score

The best-performing model was selected based on these evaluation metrics.

🚀 Results
------------------------------------------------------------------------------------------------

The models demonstrated consistent performance across training and test datasets.

predicts price value based on the tabular data and the satillite images

🛠️ Technologies Used
-------------------------------------------------------------------------------------

Python

NumPy

Pandas

Scikit-learn

pytorch

Matplotlib / Seaborn (for visualization)

📌 Conclusion

This project demonstrates an end-to-end machine learning pipeline, from data preprocessing to model evaluation, providing insights into model performance and predictive accuracy.
