# L06 – Time-Series Forecasting Using Nixtla AutoML

## Overview

The goal of this lab was to apply time-series forecasting techniques to IoT sensor data. The dataset consisted of temperature readings collected over time, which made it suitable for analyzing patterns such as trends and fluctuations.

In this lab,Nixtla AutoML was used to automatically select and train a forecasting model, and then improved performance through feature engineering and evaluation techniques.

---

## What Was Done

- Loaded and explored a time-series dataset (temperature readings)
- Cleaned the data by handling missing values and outliers
- Converted timestamps into proper datetime format
- Created additional time-based features (hour, day, month, etc.)
- Used Nixtla AutoML to train a forecasting model
- Engineered custom features (rolling averages, rate of change)
- Evaluated the model using MAE and MSE
- Applied rolling-origin cross-validation
- Implemented a Variational Autoencoder (VAE) for synthetic data generation

---

## Lessons to be Learned

This lab helps one understand how machine learning works differently for time-series data compared to regular datasets.

Some key takeaways:

- Time order matters — you cannot randomly split data like in standard ML problems  
- Feature engineering plays a major role in forecasting performance  
- AutoML tools can simplify model selection, but understanding the data is still critical  
- Synthetic data generation (VAE) can help improve model generalization  

In addition, forecasting models need to capture:
- Trends  
- Seasonality  
- Sudden changes  

which makes them more complex than typical regression problems :contentReference[oaicite:0]{index=0}.

---

## Challenges

- Handling missing values without breaking time continuity  
- Ensuring data was sorted correctly by time  
- Understanding how AutoML selects models  
- Interpreting forecasting errors during sudden fluctuations  

---

## Key Insight

One important insight from this lab is that **better features often matter more than choosing a different model**.

By adding features like:
- Rolling mean (to smooth trends)
- Temperature change (to capture variation)

the model was able to perform better and capture more meaningful patterns :contentReference[oaicite:1]{index=1}.

---

## Real-World Relevance

Time-series forecasting is widely used in IIoT systems for:

- Predictive maintenance  
- Environmental monitoring  
- Energy usage prediction  
- Anomaly detection  

Accurate forecasting helps systems make better decisions based on expected future behavior.

---

## Conclusion

This lab strengthens one's understanding of time-series modeling and showed how AutoML, feature engineering, and evaluation techniques work together.

It also served as an introduction to generative models like VAEs, which can improve performance by creating additional training data when real data is limited.
