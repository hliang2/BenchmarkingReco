## Introduction
In this research project, we propose an experimental method for measuring bias in face recognition systems. Existing methods to measure bias depend on benchmark datasets that are collected in the wild and annotated for protected (e.g., race, gender) and non-protected (e.g., pose, lighting) attributes. Such observational datasets only permit correlational conclusions, e.g., "Algorithm A's accuracy is different on female and male faces in dataset X.". By contrast, experimental methods manipulate attributes individually and thus permit causal conclusions, e.g., "Algorithm A's accuracy is affected by gender and skin color."

Our method is based on generating synthetic faces using a neural face generator, where each attribute of interest is modified independently while leaving all other attributes constant. Human observers crucially provide the ground truth on perceptual identity similarity between synthetic image pairs. We validate our method quantitatively by evaluating race and gender biases of three research-grade face recognition models. Our synthetic pipeline reveals that for these algorithms, accuracy is lower for Black and East Asian population subgroups. Our method can also quantify how perceptual changes in attributes affect face identity distances reported by these models. Our large synthetic dataset, consisting of 48,000 synthetic face image pairs (10,200 unique synthetic faces) and 555,000 human annotations (individual attributes and pairwise identity comparisons) is available to researchers in this important area.

<div align="center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/extHERuTB_I" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<!-- </div>

Below, we use the [tipiX](https://github.com/adalca/tipiX) interactive visualization tool for some time lapses. The first row shows real time lapses created by artists, the second row shows videos synthesized by the <i>visual deprojection</i> baseline, and the third row shows videos synthesized by our method. To use the tipiX tool, click on the image to pause/start the autoplay feature, and move your mouse from left to right to move through each time lapse. 
<div align="center">
<iframe src="https://www.mit.edu/~adalca/tipiXnightly/?path=http://people.csail.mit.edu/xamyzhao/timelapse_outputs/sample_watercolor_results/preds_frame$.png&xBins=40&nDims=1&iframe=500x310&play=150" height="310" width="500"></iframe>
</div> -->

<!-- ## Paper
**Painting Many Pasts: Synthesizing Time Lapse Videos of Paintings**  
[Amy Zhao](https://people.csail.mit.edu/xamyzhao), [Guha Balakrishnan](https://people.csail.mit.edu/balakg/), [Kathleen M. Lewis](https://katiemlewis.github.io/), [Fredo Durand](https://people.csail.mit.edu/fredo), [John Guttag](https://people.csail.mit.edu/guttag), [Adrian V. Dalca](adalca.mit.edu)  
To appear in CVPR 2020.  -->

<!-- <sub>Repo name inspired by Magic: The Gathering.</sub> -->

<!-- ![Timecrafting](https://gatherer.wizards.com/Handlers/Image.ashx?multiverseid=129012&type=card) -->
