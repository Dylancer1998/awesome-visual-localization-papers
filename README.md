# Camera-relocalization-papers

Contributed by Dehao Zhang.

The relocalization task aims to estimate the 6-DoF pose of a novel (unseen) frame in the coordinate system given by the prior model of the world. 



**TOC**

| Section | # of Papers |
|:---:|:---:|
|[Survey papers](#Surveys) | 1|
|[System](#system) | 6 |
|[Retrieval methods](#Retrieval) | 4 |
|[Pose Estimation](#Pose) | 1 |
|[SLAM](#SLAM) | 1 |
|[SfM](#SfM) | 1 |
|[Feature Extracting and Matching](#Feature) | 1 |

\* 📒 means which are most import in this are and there are detailed notes in the notes branch, others are not most important and scan roughly.



<h1 id="Surveys">Survey papers</h1>

<details>
<summary> <b>【[Image-based camera localization: an overview】</b> Yihong Wu. Visual Computing for Industry, Biomedicine, and Art, 2018. 📒</summary>
 <b> More detailed notes in the notes branch.</b>
</details>



<h1 id="system">System</h1>

<details>
<summary> <b>【Wide area localization on mobile phones】</b> Clemens Arth. ISMAR, 2009. 📒</summary> 
<b> More detailed notes in the notes branch.</b> The first step is reconstruction and save the result by PVS(potentially visible sets). Then feature matching and pose etismation... In a normal relocalization way.
</details>
<details>
<summary> <b>【Real-time self-localization from panoramic images on mobile devices】</b> Clemens Arth. ISMAR, 2011. 📒</summary>
<b> More detailed notes in the notes branch.</b> This paper focused on the outdoor scene. The differences of the method and traditional methods are using image stiching to get panoramic images.
</details>

<details>
<summary> <b>【Parallel Tracking and Mapping on a Camera Phone】</b> ISMAR, 2009.</summary>
</details>

<details>
<summary> <b>【Pose Tracking from Natural Features on Mobile Phones】</b> ISMAR, 2008.</summary>
</details>

<details>
<summary> <b>【Scalable 6-DOF Localization on Mobile Devices】</b> Iven Middelberg, Torsten Sattler. ECCV, 2014. 📒</summary>
This work combines the local tracking and global relocalization so they throwed the loop closuring in the tracking. The main contributions of this paper are the three align methods: alignment only once, alignment using the global keyframe positions and alignmnet Using the global 2D-3D matches.
</details>
<details>
<summary> <b>【6D dynamic camera relocalization from single reference image】</b> Feng W. CVPR 2016. </summary>
</details>


<h1 id="Feature">Feature Extracting and Matching</h1>

<details>
<summary> <b>【SuperGlue: Learning Feature Matching with Graph Neural Networks】Paul-Edouard Sarlin. CVPR, 2020. </b>  <a href="https://github.com/magicleap/SuperGluePretrainedNetwork">【Code】📒</a></summary>
<b> More detailed notes in the notes branch.</b> A deep learning method to instead middle-end of SLAM.
</details>



<h1 id="Retrieval">Retrieval Methods</h1>

<details>
<summary> <b>【Fast image-based localization using direct 2D to-3D matching】</b> Sattler T. ICCV, 2011. <a href="https://www.graphics.rwth-aachen.de/software/image-localization/">【Code】📒</a></summary>
<b> More detailed notes in the notes branch.</b> The direct means use the descriptors of 2D
  points to match the descriptors of 3D points.
</details>

<details>
<summary> <b>【Image Retrieval for Image-Based Localization Revisited】</b> Sattler T. BMVC, 2012. <a href="https://www.graphics.rwth-aachen.de/software/image-localization/">【Code】</a></summary>
</details>

<details>
<summary> <b>【A Vote-and-Verify Strategy for Fast Spatial Verification in Image Retrieval】</b> ACCV, 2016. </summary>
</details>
<details>
<summary> <b>【Improving image-based localization by active correspondence search】</b> ECCV, 2012. 📒</summary>
A more efficient version of the "Fast image-based localization using direct 2D to 3D machting". With 2D to 3D match onece and then do 3D to 2D.
Beacause using 2D points for find 3D points is not efficient, but using 3D points to find 2D points is efficient for the less number of 2D points.
</details>


<h1 id="Pose">Pose Estimation</h1>
<details>
<summary> <b>【DSAC - Differentiable RANSAC for Camera Localization】</b>E. Brachmann. CVPR, 2017. </summary>
propose **Differentiable SAmple Consensus** and make RANSAC method available for camera localization in an **end-to-end-trained** deep learning pipeline
</details>


<h1 id="SLAM">SLAM</h1>
<details>
<summary> <b>【Neural Topological SLAM for Visual Navigation】</b>Devendra Singh Chaplot. CVPR, 2020. </summary>
The goal is giving a image in a house and then navigate the robot to find the right place.
</details>


<h1 id="SfM">SfM</h1>
<details>
<summary> <b>【Consistent Video Depth Estimation】</b>XUAN LUO. SIGGRAPH 2020. </summary>
Using colmap to do sparse reconstruction, using deep learning methods to do dense reconstrution.
</details>



<h1 id="Wait">Wait to sort</h1>

<details>
  <summary> <b>【FREAK:Fast Retina Keypoint.】</b> A. Amit. CVPR, 2012.</summary>
</details>

<details>
  <summary> <b>【NetVLAD: CNN architecture for weakly supervised place recognition】</b> R. Arandjelovic. CVPR, 2016. </summary>
</details>

<details>
  <summary> <b>【Three thins evereyone should know to improve object retrieval】</b> R. Arandjelovic. CVPR, 2012. </summary>
</details>

<details>
  <summary> <b>【Learning local feature descriptors with triplets and shallow convolutional neural networks】</b> V. Balntas. BMVC, 2016. </summary>
</details>

<details>
  <summary> <b>【Learning 6D Object Pose Estimation Using 3D Objet Coordinates】</b> E.Brachmann. ECCV, 2014.</summary>
</details>

<details>
  <summary> <b>【DSAC-Differentiable RANSAC for Camera Localization】</b> E.Brachmann. CVPR, 2017. </summary>
</details>

<details>
  <summary> <b>【Discriminative Learning of Local Image Descriptors】</b> TPAMI, 2011.</summary>
</details>

<details>
  <summary> <b>【Deep Image Retrieval: Learning global representations for image search】</b> A. Gordo. arkiv, 2016. </summary>
</details>

<details>
  <summary> <b>【MatchNet: Unifying feature and metric learning for patch-based matching】</b>X. Han. CVPR, 2015. </summary>
</details>

<details>
  <summary> <b>【Comparative evaluation of binary features】</b>J. Heinly. ECCV. </summary>
</details>

<details>
  <summary> <b>【PoseNet: A Convolutional Network for Real-Time 6-DOF Camera Relocalization】</b>A. Kendall, M. ICCV, 2015. </summary>
</details>

<details>
  <summary> <b>【LIFT: Learned Invariant Feature Transform】</b> M.Kwang. ECCV, 2016. </summary>
</details>

<details>
  <summary> <b>【Semantic Visual Localization】</b> J. L. Schonberger. CVPR, 2018. </summary>
</details>

<details>
  <summary> <b>【Camera Pose Voting for Large-Scale Image-Based Localization】</b> B. Zeisl. ICCV, 2015.. </summary>
</details>

<details>
  <summary> <b>【Image Matching Across Wide Baselines: From Paper to Practice】</b> Yuehe, Jin. CVPR, 2020. </summary>
</details>

<details>
  <summary> <b>【ASLFeat: Learning Local Features of Accurate Shape and Localization】</b> Zixin, Lup. CVPR, 2020. </summary>
</details>

<details>
  <summary> <b>【City-Scale Localization for Cameras with Known Vertical Direction】</b> Linus Svarm. TAPMI, 2016. </summary>
</details>