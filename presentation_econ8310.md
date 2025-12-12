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
- Best performance came from:
  - Pre-trained neural network 
  - blah 
  - blah 

**Overall Result:** The model... blah blah blah

---

# Visual Examples

**Sample predictions:**  

- Provide some sample predictions


---

# Project Challenges 

- Building the dataset
- Data pipeline issues
- Training obstacles 


---

# The Problem
NOT SURE IF NEEDED

- x
- y
- z

---

# Data Labeling (CVAT)
NOT SURE IF NEEDED

- x
- y
- z

**Challenges:**  
- x, y, z

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

- Model from scratch
- Pretrained neural network

**Why a neural network?**  
- x, y, z

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


