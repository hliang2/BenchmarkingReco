## Benchmarking Algorithmic Bias in Face Recognition

In this project, we propose an **experimental framework** for measuring bias in face recognition systems.  
Existing approaches rely on benchmark datasets collected in the wild, annotated for protected (e.g., race, gender) and non-protected (e.g., pose, lighting) attributes. Such observational datasets only allow **correlational conclusions**, e.g., *"Algorithm A's accuracy differs between female and male faces in dataset X."*  

By contrast, our **experimental approach** manipulates attributes individually, enabling **causal conclusions**, e.g., *"Algorithm A's accuracy is affected by gender and skin color."*  

Our method is based on generating synthetic faces using a neural face generator, where each attribute of interest is modified independently while keeping all other attributes constant. Human observers provide ground truth on perceptual identity similarity between synthetic image pairs. We validate the method by evaluating race and gender biases of three research-grade face recognition models, and further show how perceptual attribute changes affect face identity distances reported by these models.  

---

## Dataset

We release **CausalFace**, a large synthetic dataset consisting of:  
- **48,000 synthetic face image pairs** (10,200 unique synthetic faces)  
- **555,000 human annotations** (individual attributes and pairwise identity comparisons)  

This dataset enables causal benchmarking of face recognition algorithms.  
The full dataset (images + annotations) is available here:  
👉 [**Download CausalFace Dataset**](https://rice.box.com/s/0t7dtfurh8jf80mhq3f7s8nbya2g58w9)  

<div align="center">
  <img src="prototype.png" alt><br>
  <em>Figure 1. Prototype faces spanning sensitive attributes of race and gender. Starting from random seeds sampled in the latent space of our face generator, we traverse latent directions correlated with sensitive attributes to generate faces across demographic groups (M = Male, F = Female, W = White, B = Black, A = East Asian).</em>
</div>

<div align="center">
  <img src="attributes.png" alt><br>
  <em>Figure 2. Examples of modifying non-sensitive attributes (pose, lighting, age, expression) while keeping identity consistent.</em>
</div>

---

## Paper

- [**Benchmarking Algorithmic Bias in Face Recognition: An Experimental Approach Using Synthetic Faces and Human Evaluation**](https://arxiv.org/abs/2308.05441)  
  Hao Liang, Pietro Perona, Guha Balakrishnan  
  *ICCV 2023*

- [**Towards Causal Benchmarking of Face Analysis Algorithms**](https://arxiv.org/abs/2007.06570)  
  Guha Balakrishnan, Yuanjun Xiong, Wei Xia, Pietro Perona  
  *ECCV 2020*

---

## Codebase

The supporting codebase and project materials are available on GitHub:  
👉 [**View Code Repository**](https://github.com/your-repo-link)
