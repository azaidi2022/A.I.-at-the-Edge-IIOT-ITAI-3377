# A06 – Time-Series Forecasting Using Nixtla AutoML

## Overview

The goal of this assignment was to apply machine learning techniques to time-series data collected from IoT devices. The dataset consisted of temperature readings over time, making it suitable for forecasting future values based on historical patterns.

This assignment focused on data preprocessing, feature engineering, model selection using AutoML, and evaluation of forecasting performance.

---

## Problem

Time-series data is different from regular datasets because the order of data points matters. In IoT systems, predicting future values such as temperature or system behavior is important for monitoring and decision-making.

The challenge was to build a model that can accurately predict future values while handling issues like missing data, noise, and sudden changes.

---

## Approach

The workflow included:

- Cleaning the dataset (handling missing values and outliers)
- Converting timestamps into datetime format
- Creating time-based features (hour, day, month)
- Using Nixtla AutoML to select and train a forecasting model
- Adding custom features:
  - Rolling mean (to smooth trends)
  - Temperature difference (rate of change)
- Evaluating the model using MAE and MSE
- Applying rolling-origin cross-validation

In addition, a Variational Autoencoder (VAE) was used to generate synthetic data to improve model performance.

---

## Results

The model was able to capture overall trends and patterns in the data.

- Consistent performance across validation windows  
- Good ability to follow long-term trends  
- Some difficulty handling sudden fluctuations  

The use of feature engineering and synthetic data helped improve generalization and reduce overfitting :contentReference[oaicite:0]{index=0}.

---

## Lessons to be Learned

This assignment shows one that time-series forecasting requires a different approach compared to standard machine learning.

Some key takeaways:

- Data must be kept in chronological order  
- Feature engineering is critical for performance  
- AutoML simplifies model selection but does not replace understanding the data  
- Synthetic data can help improve model robustness  

---

## Challenges

- Handling missing values without breaking time continuity  
- Understanding how AutoML selects models  
- Interpreting forecasting errors during sudden changes  

---

## Real-World Relevance

Time-series forecasting is widely used in IIoT systems for:

- Predictive maintenance  
- Environmental monitoring  
- Energy consumption prediction  

These applications rely on accurate predictions to make better operational decisions.

---

## Conclusion

This assignment strengthens one's understanding of time-series forecasting and shows how multiple techniques—data preprocessing, feature engineering, AutoML, and generative modeling work together to improve performance.
