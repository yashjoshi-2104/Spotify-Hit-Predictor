# Spotify-Hit-Predictor
This project analyzes a Spotify 2023 dataset to predict whether a track appears in Spotify charts using a Decision Tree Classifier. It demonstrates classification, feature encoding, and handling class imbalance.

1. Preprocessing

      Removed irrelevant text columns (e.g., song titles).
      
      Converted numeric columns using pd.to_numeric(errors='coerce').
      
      Label encoded categorical columns (key, mode).
      
      Split data into training and testing sets using train_test_split.

2. Model

      Algorithm: Decision Tree Classifier
      
      Parameters: max_depth=3, random_state=42
      
      Objective: Predict in_spotify_charts (binary classification)

3. Results
   
      Accuracy	0.90
   
      Precision (In Charts)	0.76
   
      Recall (In Charts)	0.61

The model performs well overall but underperforms for minority (in-charts) tracks due to class imbalance.

4. Visualizations

      Feature importance plot.
      
      Decision tree visualization.
      
      Confusion matrix heatmap.
