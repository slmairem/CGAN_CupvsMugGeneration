# CGAN- Cup vs Mug Generation

**Collaboration:** Selma İrem Özdemir & Alp Onat Topçam

---

## Overview
This project explores the use of **Conditional GANs (cGANs)** for generating cup and mug images conditioned on class labels. The goal is to generate realistic images of cups and mugs across two categories:

- **Colored**
- **Black & White (BW)**

---

## Dataset
The dataset for this project was **curated manually** from multiple sources, including:

- GoogleImageCrawler  
- DuckDuckGo  
- Bing  
- Kaggle  

### Dataset Collection & Preprocessing
- Specifically searched for images of **cups and mugs**.  
- Manually categorized images into **Colored** and **BW** classes based on visual characteristics.  
- Filtered out low-resolution or irrelevant images to ensure quality.  

### Final Dataset Statistics
| Class                     | Image Count |
|----------------------------|------------|
| Black & White Cups         | 597        |
| Colored Cups               | 909        |
| Black & White Mugs         | 269        |
| Colored Mugs               | 931        |

This curated dataset provides a **clean and well-balanced structure** for training a CGAN to generate **class- and style-specific images**.
  
---

## Challenges
- **Difficulty in Generating BW Cups Using RGB Output:** The model struggled to synthesize BW cups correctly.
- **Mode Collapse:** Recurring issue during training requiring mitigation strategies.

---

## Methodology
- **Conditional GAN (cGAN)** with class conditioning.
- **Hinge Loss** to improve training stability.
- **LPIPS (Learned Perceptual Image Patch Similarity)** for perceptual quality.
- Extensive experimentation with architectures, hyperparameters, and training strategies.

---

## Results
- Generated realistic colored cups and mugs.
- Documented challenges with BW output.
- Mode collapse partially mitigated using hinge loss and perceptual similarity.
