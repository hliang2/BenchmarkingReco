## Benchmarking Algorithmic Bias in Face Recognition
In this research project, we propose an experimental method for measuring bias in face recognition systems. Existing methods to measure bias depend on benchmark datasets that are collected in the wild and annotated for protected (e.g., race, gender) and non-protected (e.g., pose, lighting) attributes. Such observational datasets only permit correlational conclusions, e.g., "Algorithm A's accuracy is different on female and male faces in dataset X.". By contrast, experimental methods manipulate attributes individually and thus permit causal conclusions, e.g., "Algorithm A's accuracy is affected by gender and skin color."

Our method is based on generating synthetic faces using a neural face generator, where each attribute of interest is modified independently while leaving all other attributes constant. Human observers crucially provide the ground truth on perceptual identity similarity between synthetic image pairs. We validate our method quantitatively by evaluating race and gender biases of three research-grade face recognition models. Our synthetic pipeline reveals that for these algorithms, accuracy is lower for Black and East Asian population subgroups. Our method can also quantify how perceptual changes in attributes affect face identity distances reported by these models. 

## Paper
[**Benchmarking Algorithmic Bias in Face Recognition: An Experimental Approach Using Synthetic Faces and Human Evaluation**](https://arxiv.org/abs/2308.05441)<br>
Hao Liang, Pietro Perona, Guha Balakrishnan<br>
ICCV 2023

[**Towards causal benchmarking of face analysis algorithms**](https://arxiv.org/abs/2007.06570)<br>
Guha Balakrishnan, Yuanjun Xiong, Wei Xia, Pietro Perona<br>
ECCV 2020

## Dataset
Our large synthetic dataset, **CausalFace**, consisting of 48,000 synthetic face image pairs (10,200 unique synthetic faces) and 555,000 human annotations (individual attributes and pairwise identity comparisons) is available to researchers in this important area. Below is an example of, the full version as well as the annotations are available [here](https://rice.box.com/s/0t7dtfurh8jf80mhq3f7s8nbya2g58w9).

<div align="center">
<img src = "https://github.com/hliang2/BenchmarkingReco/blob/main/attributes.png">
</div>

<div align="center">
<img src = "https://github.com/hliang2/BenchmarkingReco/blob/main/attributes.png">
</div>

