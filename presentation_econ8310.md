---
marp: true
title: "Econ 8310 – Semester Project"
---

<style>
  /* Target images within slides */
  img {
    max-height: 400px;
    display: block; /* Helps with centering */
    margin: auto;
  }
</style>

# **Hey Batta Batta... _Train a Neural Network_**
### ECON 8310 Semester Project
### Presented by _Aziz, Qi Qi, and Joe_

---

# How it started...

![Mind Blown](nn_explosion.png)

---

# How it ended...

![Mind Blown](nn_happy_ending.png)

---

# Key Findings

- Did our final model successfully identify moving baseballs?
- Pre-trained neural network performed better (obviously)
  - blah 
  - blah 

**Overall Result:** The model... blah blah blah

---

# Visual Examples

**Sample predictions:**  

- Provide some sample predictions

---

# Project Obstacles 

Our challenges can be broken down into three categories:

- Data engineering
- Model training
- Evaluation 


---

# Data engineering
Most difficult part of the project

- Misalignment between videos and annotations (indexing errors)
- Inconsistent annotations 
- Dataset & batching issues (targets were in different shapes)

**Insight:** The brunt of the work was turning the videos and annotations into something a model could actually use

---

# Model & training 
The model only works when the data pipeline works...

- Incorrect inout types (expecting float tensors but images in uint8)
- Class imbalance: "moving" was rare 
- Training loop crashes: incorrect ndexing, stacking errors, mismatched shapes
- Memory constraints: large frames + batch loading = crash

**Insight:**  Get a better computer... just kidding

---

# Model evaluation

- Checkpoint loading issues (unpickling errors)
- Validation confusion: unsure where/how to build a validation data loader
- Model paramaters: trying to figure out what information a model object gives

**Insight:**  Evaluating, saving, and reloading a neural network model is its own engineering problem 

---

# Data Preparation Pipeline

1. Extracted frames from videos  
2. Resized frames for model efficiency  
3. Normalized pixel intensities 
4. Manually created train and validation sets  
5. Applied transformations

---

# Additional Data Request

We requested:

- **Side-angle and high-angle views**  
- **Videos with different lighting**  
- **Higher FPS** footage

**Reason:**  
Why'd we request additional data?  More videos, more data, higher performance. 

---

# Modeling Approach

Homegrown model vs. Pretrained 

**Why a neural network?**  
- CNNs excel at small-object detection  
- Handle variations in scale, lighting, and speed  
- Pretrained backbones reduce data requirements  

**Model inputs:**  
- input features

**Model outputs:**  
- resulting output

---

# Training the Neural Network

- Loss function: **Smooth L1 + BCE**  
- Optimizer: **Adam**
- Learning rate: **1e-3**
- Batch size: **8**
- Trained for **20 epochs**

---

# Results

**Performance Metrics:**

- Mean IoU: **0.00**  
- Precision: **0%**  
- Recall: **0%**

**Insights:**

- x, y, z

---

# Limitations

- Small object + fast motion = natural difficulty  
- Limited labeled data compared to typical object detection tasks  
- Ball occasionally blends into background at high speed  
- Indoor videos with artificial light reduced model confidence

---

# Recommendations

To improve detection further:

- Collect **more high-FPS footage**
- Add **multiple camera angles**  
- Expand training set

Future goal: realtime ball-tracking system for coaches.

---

# Template Slide

- 
-  
- 
-   

---

<style scoped>
section {
display: flex;
flex-direction: column;
justify-content: center; 
align-items: center; 
text-align: center; 
}
</style>

# Thank you for listening!
### _Questions or commentary?_


