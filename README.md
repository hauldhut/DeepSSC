# DeepSSC: A Semi-Supervised Deep Learning Framework for Multi-Omics Cancer Subtype Classification and Biomarker Discovery

---
This repository contains source code and original/preprocessed datasets for the paper "DeepSSC: A Semi-Supervised Deep Learning Framework for Multi-Omics Cancer Subtype Classification and Biomarker Discovery". 
#### 1. Introduction
---
Advances in high-throughput -omics technologies have enabled comprehensive molecular characterization of cancer, creating new opportunities for subtype classification and biomarker discovery. However, multi-omics integration remains challenging due to heterogeneous data modalities and the limited availability of labeled samples for training deep learning models.

To address these challenges, we propose DeepSSC, a biphasic semi-supervised deep learning framework for multi-omics cancer subtype classification and biomarker identification. By learning modality-specific representations and integrating them through a post-concatenation strategy, DeepSSC leverages both labeled and unlabeled samples to improve predictive performance. Extensive evaluations across multiple cancer types demonstrate that DeepSSC achieves robust classification accuracy while identifying biologically meaningful subtype-specific biomarkers, highlighting the value of semi-supervised learning for precision oncology.

#### 2. Analysis Pipeline
---
![Figure1](https://github.com/hauldhut/DeepSSC/blob/main/Figure1.png)
** Figure 1 | Framework of DeepSSC. ** In phase 1, the two preprocessed profiles (GE and CNA) from TCGA were fed into their own denoising autoencoders to generate two independent representations, zGE and zCNA . Then, zGE and zCNA  were concatenated into a single input layer attached with two FC layers to create a neural network classifier. Finally, this neural network classifier became the input of our BGI procedure in phase 2 to detect candidate biomarkers. To demonstrate the efficacy of DeepSSC, those biomarkers should help classify cancer patients into different subtypes well by only using simple machine learning models. Besides, those biomarkers also were further investigated in terms of their biological functions. Note that labeled and unlabeled data were defined clearly at the ‘Materials and Methods’ section in the work. Abbreviation: GE, mRNA expression; CNA, copy-number alterations; FC, fully-connected layer.

#### 3. Contact
---
Feel free to contact [Quang-Huy Nguyen](https://github.com/huynguyen250896) (huynguyen96.dnu@gmail.com) or [Duc-Hau Le](https://github.com/hauldhut) (hauld@soict.hust.edu.vn) for any questions about the paper, datasets, code and results.


