# DeepSSC: A Semi-Supervised Deep Learning Framework for Multi-Omics Cancer Subtype Classification and Biomarker Discovery

---
This repository contains source code and original/preprocessed datasets for the paper "DeepSSC: A Semi-Supervised Deep Learning Framework for Multi-Omics Cancer Subtype Classification and Biomarker Discovery". 
#### 1. Highlights
---
-	DeepSSC integrates semi-supervised learning for multi-omics cancer subtype classification. 
-	Modality-specific denoising autoencoders learn representations from labeled and unlabeled samples. 
-	Post-concatenation fusion enables effective integration of complementary omics representations. 
-	Integrated Gradients-based biomarker identification reveals subtype-specific molecular features. 
-	Identified biomarkers retain predictive utility and show biological relevance across cancer cohorts.

#### 2. Analysis Pipeline
---
![Figure1](https://github.com/hauldhut/DeepSSC/blob/main/Figure1.png)
** Figure 1 | Overview of the DeepSSC framework. DeepSSC consists of two phases. In Phase 1 (semi-supervised classifier training), preprocessed gene expression (GE) and copy-number alteration (CNA) profiles from TCGA are separately input into two denoising autoencoders (DAEs) to learn omics-specific latent representations, denoted as ZGE and ZCNA. These latent features are concatenated and passed through two fully connected (FC) layers to construct a neural network classifier for cancer subtype prediction. In Phase 2 (Biomarker Gene Identification, BGI), the trained classifier is used to identify candidate subtype-specific biomarkers. The resulting biomarker set is evaluated using conventional machine learning models to assess its discriminative power for subtype classification and is further analyzed for biological relevance through functional investigation.

#### 3. Contact
---
Feel free to contact [Quang-Huy Nguyen](https://github.com/huynguyen250896) (huynguyen96.dnu@gmail.com) or [Duc-Hau Le](https://github.com/hauldhut) (hauld@soict.hust.edu.vn) for any questions about the paper, datasets, code and results.


