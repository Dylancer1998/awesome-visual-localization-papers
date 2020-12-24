# Visual-Based-Localization-Papers

Contributed by Dehao Zhang.

The relocalization task aims to estimate the 6-DoF pose of a novel (unseen) frame in the coordinate system given by the prior model of the world.  The most related topics are SLAM and SfM.


<h1 id="Surveys">Survey papers</h1>

<details>
<summary> <b>[Image-based camera localization: an overview]</b> Yihong Wu. Visual Computing for Industry, Biomedicine, and Art, 2018. </summary>
</details>


<h1 id="system">System</h1>

<details>
<summary> <b>[Wide area localization on mobile phones]</b> Clemens Arth. ISMAR, 2009.</summary> 
The first step is reconstruction and save the result by PVS(potentially visible sets). Then feature matching and pose etismation... In a normal relocalization way.
</details>

<details>
<summary> <b>[Real-time self-localization from panoramic images on mobile devices]</b> Clemens Arth. ISMAR, 2011.  </summary>
This paper focused on the outdoor scene. The differences of the method and traditional methods are using image stiching to get panoramic images.
</details>
<details>
<summary> <b>[Parallel Tracking and Mapping on a Camera Phone]</b> ISMAR, 2009.</summary>
</details>

<details>
<summary> <b>[Pose Tracking from Natural Features on Mobile Phones]</b> ISMAR, 2008.</summary>
</details>

<details>
<summary> <b>[Scalable 6-DOF Localization on Mobile Devices]</b> Iven Middelberg, Torsten Sattler. ECCV, 2014. </summary>
This work combines the local tracking and global relocalization so they throwed the loop closuring in the tracking. The main contributions of this paper are the three align methods: alignment only once, alignment using the global keyframe positions and alignmnet Using the global 2D-3D matches.
</details>

<details>
<summary> <b>[6D dynamic camera relocalization from single reference image]</b> Feng W. CVPR 2016. </summary>
</details>

<details>
<summary> <b>[A Dataset for Benchmarking Image-based Localization]</b> Xun Sun. Baidu Autonomous Driving Business Unit. CVPR, 2017. </summary>
This paper proposed a dataset of BaiduMall and gave a summary about how to improve the recall of retrieval methods and match methods.
</details>


<details>
<summary> <b>[Image Matching Across Wide Baselines: From Paper to Practice]</b> Yuehe, Jin. CVPR, 2020. <a href="https://github.com/ubc-vision/image-matching-benchmark">[Code]</a> </summary>
This paper thought there were lots of fake "state of the art", so it gave a modular pipeline which incorporate dozens of methods for feature extraction, matching, and pose estimation. It's worth to read!!!
</details>

<details>
<summary> <b>[Unpublished][Using Image Sequences for Long-Term Visual Localization]</b> Erik Stenborg, Torsten Sattler and Lars Hammarstrand. 3DV, 2020. <a href="https://github.com/rulllars/SequentialVisualLocalization">[Code]</a> </summary>

</details>


<h1 id="FeatureExtration">Feature Extracting</h1>

<h1 id="FeatureMatch">Feature Matching</h1>

<details>
<summary> <b>[SuperGlue: Learning Feature Matching with Graph Neural Networks]  </b> Paul-Edouard Sarlin. CVPR, 2020. <a href="https://github.com/magicleap/SuperGluePretrainedNetwork">[Code]</a></summary>
A deep learning method to instead middle-end of SLAM.
</details>

<details>
<summary> <b>[Unread][Learning Feature Descriptors using Camera Pose Supervision]  </b> Qianqian Wang. ECCV, 2020(oral). <a href="https://github.com/qianqianwang68/caps">[Code]</a></summary>
</details>


<h1 id="Retrieval">Retrieval Methods</h1>

<details>
<summary> <b>[Visual Categorization with Bags of Keypoints]</b> G. Csurka. ECCV, 2004. </summary>
Very famous framework: Bag of Words.
</details>

<details>
<summary> <b>[Unread][Total Recall: Automatic Query Expansion
with a Generative Feature Model for Object Retrieval]</b> Chum, O. ICCV, 2007. </summary>

</details>

<details>
<summary> <b>[Fisher Kernels on Visual Vocabularies for Image Categorization]</b> F. Perronnin and C. Dance. CVPR, 2007. </summary>
Very famous framework: fisher vector.
</details>

<details>
<summary> <b>[Aggregating Local Descriptors Into a Compact Image Representation]</b> H. Jegou. CVPR, 2010. </summary>
Very famous framework: VLAD.
</details>

<details>
<summary> <b>[Fast image-based localization using direct 2D to-3D matching]</b> Sattler T. ICCV, 2011. <a href="https://www.graphics.rwth-aachen.de/software/image-localization/">[Code]</a></summary>
</details>

<details>
<summary> <b>[Improving image-based localization by active correspondence search]</b> ECCV, 2012. </summary>
A more efficient version of the "Fast image-based localization using direct 2D to 3D machting". With 2D to 3D match onece and then do 3D to 2D.
Beacause using 2D points for find 3D points is not efficient, but using 3D points to find 2D points is efficient for the less number of 2D points.
</details>

<details>
<summary> <b> [Aggregating Deep Convolutional Features for Image Retrieval]</b> A. Babenko and V. Lempitsky. ICCV, 2015. </summary>
This paper gave a decriptor called SPoC which is based on the
aggregation of raw deep convolutional features without embedding. Sum pooling all deep features weighted by Gaussian scheme, because objects of interest tend to be located close to the geometrical center of an image.
</details>

<details>
<summary> <b>[A Vote-and-Verify Strategy for Fast Spatial Verification in Image Retrieval]</b> Johannes L. Sch¨onberger. ACCV, 2016. <a href="https://github.com/vote-and-verify">[Code]</a></summary>
Although the paper's name is retrieval, but the verification method is closer to feature matching. Previous verification frameworks based on RANSAC were too slow. This paper gave a hypothesize-and-verify approaches which was very fast. This paper is integrated to the colmap framework.
</details>

<details>
<summary> <b>[NetVLAD: CNN Architecture for Weakly Supervised Place Recognition]</b> R. Arandjelovic. CVPR, 2016. </summary>
By using GPS, this paper got the potential positives and definite negative training examples. The difference between NetVLAD and VLAD is aggregation step, NetVLAD use a VLAD layer to learned the weight of each centroid. So that NetVLAD provide a fully differential pipeline to apply on the weakly supervised task.
</details>

<details>
<summary> <b>[Crossdimensional Weighting for Aggregated Deep Convolutional Features]</b> Y. Kalantidis. ECCV, 2016. <a href="https://github.com/yahoo/crow">[Code]</a> </summary>
Provided a Cross-dimensional Weighted framework(CroW) as: 1. Perform spatially-local pooling; 2. Compute spatial weighting factors; 3. Compute channel weighting factors; 4. Perform weighted-sum aggregation; 5. Perform vector normalization; 6. Perform dimensionality reduction; 7. Perform final normalization. The difference between "Aggregating Deep Convolutional Features for Image Retrieva" is the weighted summing.
Another fancy technology is the sparsity-sensitive channel weights, like the inverse document frequency.
</details>

<details>
<summary> <b>[Fine-Tuning CNN Image Retrieval with no Human Annotation]</b> F. Radenovic, G. PAMI, 2017. <a href="http://cmp.felk.cvut.cz/cnnimageretrieval">[Code]</a></summary>
Three contributions: 1.A geometry verification method to construct the dataset; 2.A new pooling method called GeM pooling; 3.Combine QE into the pipeline. (also introduce some QE tricks)
</details>

<details>
<summary> <b>[Efficient diffusion on region manifolds: Recovering small objects with compact cnn representations]</b> A. Iscen. CVPR, 2017. </summary>
A novel version of query expansion(QE).
</details>

<details>
<summary> <b>[Revisiting Oxford and Paris: Large-scale Image Retrieval Benchmarking]</b> F. Radenovic, G. CVPR, 2018. </summary>
</details>

<details>
<summary> <b>[Unread][Learning with Average Precision: Training Image Retrieval with a Listwise Loss]</b> J. Revaud. ICCV, 2019. </summary>
</details>


<details>
<summary> <b>[Benchmarking Image Retrieval for Visual Localization]</b> Noé Pion,..., Torsten Sattler. 3DV, 2020. <a href="https://github.com/naver/kapture-localization">[code]</a> </summary>
A detailed survey for image retrieval but more focused on localization. And this paper gives a very useful codebase to evaluate different algorithm.
</details>

<h1 id="Pose">Pose Estimation</h1>

<details>
<summary> <b>[Fixing the Locally Optimized RANSAC]</b>  Karel Lebeda. BMVC, 2012. </summary>

</details>

<details>
<summary> <b>[DSAC - Differentiable RANSAC for Camera Localization]</b>E. Brachmann. CVPR, 2017. </summary>
propose Differentiable Sample Consensus and make RANSAC method available for camera localization in an end-to-end-trained deep learning pipeline
</details>

<details>
<summary> <b>[MAGSAC: marginalizing sample consensus]</b>  Barath, D. CVPR, 2019. </summary>
ad
</details>


<h1 id="Fusion">Multi-sensors Fusion</h1>
<h2 id="Fusion with IMU">Fusion with IMU</h2>
<details>
<summary> <b>[DARNavi: An Indoor-Outdoor Immersive Navigation System with Augmented Reality]</b>Didi Chuxing. CVPR, 2020. </summary>
Proposed a framwork which combined the **PDR**(Pedestrian Dead Reckoning), ARKit and visual localization. But the details about the fusion strategy were not introduced in the paper.
</details>

<h2 id="Fusion with GPS">Fusion with GPS</h2>
<details>
<summary> <b>[Multi-sensor navigation algorithm using monocular camera, imu and gps for large scale augmented reality]</b> T. Oskiper. ISMAR, 2012. </summary>
IMU and camera fusion is performed in a tightly coupled manner by an error-state extended Kalman filter (EKF). GPS is also fused by a optimization framework.
</details>

<details>
<summary> <b>[Intermittent GPS-aided VIO: Online Initialization and Calibration]</b> Woosik Lee. ICRA, 2020. </summary>
The constraint is MSCKF-based estimator to fuse inertial, camera and asynchronous GPS measurements and this paper tried to solve the time offset problem. The method is tightly-coupled so it is not very suitable for map-based relocalization.
</details>

<details>
<summary> <b>[Vins Fusion —— A General Optimization-based Framework for Global
Pose Estimation with Multiple Sensors]</b> Tong Qin. </summary>
Propose a general framework to fuse various global sensors with local estimations, which support multiple global sensors. Finally, use ceres to solve the graph optimization problems.
</details>

<details>
<summary> <b>[Gomsf: Graph-optimization based multi-sensor fusion for robust uav pose estimation]</b> R. Mascaro, L. ICRA 2018 </summary>
Propose an optimization-based framework to fuse local VIO (Visual
Inertial Odometry) with GPS measurements.
</details>


<h1 id="SLAM">SLAM</h1>
<details>
<summary> <b>[Neural Topological SLAM for Visual Navigation]</b> Devendra Singh Chaplot. CVPR, 2020. </summary>
The goal is giving a image in a house and then navigate the robot to find the right place.
</details>


<h1 id="SfM">SfM</h1>
<details>
<summary> <b>[Consistent Video Depth Estimation]</b> XUAN LUO. SIGGRAPH 2020. </summary>
Using colmap to do sparse reconstruction, using deep learning methods to do dense reconstrution.
</details>


<h1 id="Wait">Wait to sort</h1>

<details>
  <summary> <b>[FREAK:Fast Retina Keypoint.]</b> A. Amit. CVPR, 2012.</summary>
</details>

<details>
  <summary> <b>[Three things evereyone should know to improve object retrieval]</b> R. Arandjelovic. CVPR, 2012. </summary>
</details>

<details>
  <summary> <b>[Learning local feature descriptors with triplets and shallow convolutional neural networks]</b> V. Balntas. BMVC, 2016. </summary>
</details>

<details>
  <summary> <b>[Learning 6D Object Pose Estimation Using 3D Objet Coordinates]</b> E.Brachmann. ECCV, 2014.</summary>
</details>

<details>
  <summary> <b>[DSAC-Differentiable RANSAC for Camera Localization]</b> E.Brachmann. CVPR, 2017. </summary>
</details>

<details>
  <summary> <b>[Discriminative Learning of Local Image Descriptors]</b> TPAMI, 2011.</summary>
</details>


<details>
  <summary> <b>[MatchNet: Unifying feature and metric learning for patch-based matching]</b>X. Han. CVPR, 2015. </summary>
</details>

<details>
  <summary> <b>[Comparative evaluation of binary features]</b>J. Heinly. ECCV. </summary>
</details>

<details>
  <summary> <b>[PoseNet: A Convolutional Network for Real-Time 6-DOF Camera Relocalization]</b>A. Kendall, M. ICCV, 2015. </summary>
</details>

<details>
  <summary> <b>[LIFT: Learned Invariant Feature Transform]</b> M.Kwang. ECCV, 2016. </summary>
</details>

<details>
  <summary> <b>[Semantic Visual Localization]</b> J. L. Schonberger. CVPR, 2018. </summary>
</details>

<details>
  <summary> <b>[Camera Pose Voting for Large-Scale Image-Based Localization]</b> B. Zeisl. ICCV, 2015.. </summary>
</details>

<details>
  <summary> <b>[ASLFeat: Learning Local Features of Accurate Shape and Localization]</b> Zixin, Lup. CVPR, 2020. </summary>
</details>

<details>
  <summary> <b>[City-Scale Localization for Cameras with Known Vertical Direction]</b> Linus Svarm. TAPMI, 2016. </summary>
</details>
[ACNe: Attentive Context Normalization for Robust PermutationEquivariant Learning] Sun, W. CVPR, 2020.
[Is there anything new to say about SIFT matching?]Fabio Bellavia. IJCV, 2020.
[Learning to Find Good Correspondences]Kwang Moo Yi. CVPR, 2018, oral.
