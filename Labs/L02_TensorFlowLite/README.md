# L02 – Converting and Deploying AI Models using TensorFlow Lite

## Overview

The purpose of this lab was to understand how machine learning models are deployed in real-world environments, not just trained.

In this lab, I trained a neural network using TensorFlow/Keras on the MNIST dataset and then converted the model into TensorFlow Lite format. After that, I used the TensorFlow Lite interpreter to run inference and simulate how models work on edge devices.

This lab helped me understand the full pipeline from training a model to actually deploying it.

---

## What I Did

- Loaded the MNIST dataset (handwritten digits)
- Normalized the data for better model performance
- Built a simple neural network using Keras
- Trained the model and evaluated accuracy
- Converted the model into `.tflite` format
- Loaded the model using the TensorFlow Lite interpreter
- Ran inference step-by-step on test images

---

## What I Learned

One of the biggest takeaways from this lab is that training a model is only part of the process. In real-world applications, models need to be converted into formats that can run efficiently on devices with limited resources.

I also learned that TensorFlow Lite works differently from regular TensorFlow/Keras. Instead of just calling `model.predict()`, I had to manually:
- Load the interpreter  
- Allocate tensors  
- Set input data  
- Invoke the model  
- Retrieve output  

This helped me better understand what actually happens during inference.

Another important lesson was how critical preprocessing is. The input data during inference must match what was used during training, or the model’s predictions can become inaccurate.

---

## Challenges

One of the main challenges was making sure the input shape and data type matched what the TensorFlow Lite model expected. For example, forgetting to include the batch dimension (using 28×28 instead of 1×28×28) caused errors during inference.

Another challenge was adjusting from high-level Keras functions to the lower-level TensorFlow Lite workflow.

---

## Real-World Relevance

TensorFlow Lite is commonly used to deploy machine learning models on:
- Mobile devices  
- IoT systems  
- Embedded hardware  

Running models locally on edge devices allows for:
- Faster response times (low latency)  
- Better privacy (data stays on device)  
- Reduced reliance on cloud systems  

This is especially important in IIoT environments where real-time decision-making is required.

---

## Conclusion

This lab showed me that building a model is only one part of machine learning. Deployment is just as important, especially when working with edge devices.

Understanding how to convert and run models using TensorFlow Lite is an essential skill for real-world AI applications.
