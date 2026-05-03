# L03 – CNN and Transfer Learning (Puppy vs Bagel Classification)

## Overview

The goal of this lab was to build and evaluate image classification models using both a custom Convolutional Neural Network (CNN) and a transfer learning approach.

The dataset consisted of images of puppies and bagels. While this seems simple, the lab highlighted how difficult image classification can be when working with small datasets.

This lab focused not only on building models, but also understanding why models succeed or fail.

---

## What I Did

- Prepared an image dataset for classification (puppy vs bagel)
- Organized data into proper folder structure for training
- Applied data augmentation techniques
- Built a custom CNN model from scratch
- Trained the model and evaluated performance
- Implemented transfer learning using a pretrained model (ResNet50)
- Compared results between both approaches

---

## What I Learned

One of the biggest lessons from this lab is that **data matters more than the model**.

Even though I used:
- A custom CNN  
- A pretrained model (ResNet50)  

Both models performed poorly, with accuracy around 50%, which is essentially random guessing :contentReference[oaicite:0]{index=0}.

This showed me that:
- Deep learning models require **large datasets** to perform well  
- Transfer learning is powerful, but **not a guaranteed solution**  
- Validation metrics are critical for understanding real performance  

I also learned how CNNs rely heavily on visual patterns like shape and color. In this case, puppies and bagels can look similar in certain images (round shapes, similar colors), which caused confusion for the model.

---

## Challenges

- Dataset was very small (only a few images per class)
- Initial dataset structure caused errors (Keras detected 0 classes)
- Model performance was unstable and inconsistent
- Transfer learning did not improve results due to lack of data

These challenges helped me understand that poor results can still provide valuable learning.

---

## Key Insight

Before this lab, I assumed that using a more advanced model would automatically improve performance.

This lab proved that:
> A better model cannot fix a weak dataset.

Understanding the limitations of data is just as important as building the model itself.

---

## Real-World Relevance

In real-world applications, image classification systems require:
- Large, high-quality datasets  
- Proper labeling and validation  
- Careful evaluation of model performance  

This lab reflects real challenges faced in industry, where data quality and availability often limit model effectiveness.

---

## Conclusion

This lab helped me shift from a “model-focused” mindset to a “data-focused” mindset.

Even though the results were not strong, the lab was successful in demonstrating:
- How CNNs work  
- The importance of validation  
- The limitations of small datasets  
- The role of transfer learning  

Understanding these limitations is essential for building better AI systems.
