# Visual-Based-Localization-Papers

Contributed by Dehao Zhang.

The relocalization task aims to estimate the 6-DoF pose of a novel (unseen) frame in the coordinate system given by the prior model of the world.  The most related topics are SLAM and SfM.


<h1 id="Surveys">Survey papers</h1>

- <b>[Image-based camera localization: an overview]</b> Yihong Wu. Visual Computing for Industry, Biomedicine, and Art, 2018. <a href="https://arxiv.org/abs/1610.03660">[paper]</a> 


<h1 id="system">System</h1>

- <b>[Wide area localization on mobile phones]</b> Clemens Arth. ISMAR, 2009. <a href="https://www.researchgate.net/publication/221221483_Wide_Area_Localization_on_Mobile_Phones">[paper]</a> 

- <b>[Real-time self-localization from panoramic images on mobile devices]</b> Clemens Arth. ISMAR, 2011. 

- <b>[Parallel Tracking and Mapping on a Camera Phone]</b> ISMAR, 2009. 

- <b>[Pose Tracking from Natural Features on Mobile Phones]</b> ISMAR, 2008.

- <b>[Scalable 6-DOF Localization on Mobile Devices]</b> Iven Middelberg, Torsten Sattler. ECCV, 2014. 

- <b>[6D dynamic camera relocalization from single reference image]</b> Feng W. CVPR 2016.

- <b>[A Dataset for Benchmarking Image-based Localization]</b> Xun Sun. Baidu Autonomous Driving Business Unit. CVPR, 2017. 

- <b>[Image Matching Across Wide Baselines: From Paper to Practice]</b> Yuehe, Jin. CVPR, 2020. <a href="https://github.com/ubc-vision/image-matching-benchmark">[Code]</a> 

- <b>[Unpublished][Using Image Sequences for Long-Term Visual Localization]</b> Erik Stenborg, Torsten Sattler and Lars Hammarstrand. 3DV, 2020. <a href="https://github.com/rulllars/SequentialVisualLocalization">[Code]</a> 


<h1 id="FeatureExtration">Feature Extracting</h1>

<h1 id="FeatureMatch">Feature Matching</h1>

- <b>[SuperGlue: Learning Feature Matching with Graph Neural Networks]  </b> Paul-Edouard Sarlin. CVPR, 2020. <a href="https://github.com/magicleap/SuperGluePretrainedNetwork">[Code]</a>

- <b>[Unread][Learning Feature Descriptors using Camera Pose Supervision]  </b> Qianqian Wang. ECCV, 2020(oral). <a href="https://github.com/qianqianwang68/caps">[Code]</a>


<h1 id="Retrieval">Retrieval Methods</h1>

- <b>[Visual Categorization with Bags of Keypoints]</b> G. Csurka. ECCV, 2004. 

- <b>[Unread][Total Recall: Automatic Query Expansion
with a Generative Feature Model for Object Retrieval]</b> Chum, O. ICCV, 2007. 

- <b>[Fisher Kernels on Visual Vocabularies for Image Categorization]</b> F. Perronnin and C. Dance. CVPR, 2007. 

- <b>[Aggregating Local Descriptors Into a Compact Image Representation]</b> H. Jegou. CVPR, 2010. 

- <b>[Fast image-based localization using direct 2D to-3D matching]</b> Sattler T. ICCV, 2011. <a href="https://www.graphics.rwth-aachen.de/software/image-localization/">[Code]</a>

- <b>[Improving image-based localization by active correspondence search]</b> ECCV, 2012.

- <b> [Aggregating Deep Convolutional Features for Image Retrieval]</b> A. Babenko and V. Lempitsky. ICCV, 2015. 

- <b>[A Vote-and-Verify Strategy for Fast Spatial Verification in Image Retrieval]</b> Johannes L. Sch¨onberger. ACCV, 2016. <a href="https://github.com/vote-and-verify">[Code]</a>

- <b>[NetVLAD: CNN Architecture for Weakly Supervised Place Recognition]</b> R. Arandjelovic. CVPR, 2016.

- <b>[Crossdimensional Weighting for Aggregated Deep Convolutional Features]</b> Y. Kalantidis. ECCV, 2016. <a href="https://github.com/yahoo/crow">[Code]</a> 

- <b>[Fine-Tuning CNN Image Retrieval with no Human Annotation]</b> F. Radenovic, G. PAMI, 2017. <a href="http://cmp.felk.cvut.cz/cnnimageretrieval">[Code]</a>

- <b>[Efficient diffusion on region manifolds: Recovering small objects with compact cnn representations]</b> A. Iscen. CVPR, 2017. 

- <b>[Revisiting Oxford and Paris: Large-scale Image Retrieval Benchmarking]</b> F. Radenovic, G. CVPR, 2018. 

- <b>[Unread][Learning with Average Precision: Training Image Retrieval with a Listwise Loss]</b> J. Revaud. ICCV, 2019. 


- <b>[Benchmarking Image Retrieval for Visual Localization]</b> Noé Pion,..., Torsten Sattler. 3DV, 2020. <a href="https://github.com/naver/kapture-localization">[code]</a> 

<h1 id="Pose">Pose Estimation</h1>

- <b>[Fixing the Locally Optimized RANSAC]</b>  Karel Lebeda. BMVC, 2012. 

- <b>[DSAC - Differentiable RANSAC for Camera Localization]</b>E. Brachmann. CVPR, 2017. 

- <b>[MAGSAC: marginalizing sample consensus]</b>  Barath, D. CVPR, 2019. 


<h1 id="Fusion">Multi-sensors Fusion</h1>
<h2 id="Fusion with IMU">Fusion with IMU</h2>
- <b>[DARNavi: An Indoor-Outdoor Immersive Navigation System with Augmented Reality]</b>Didi Chuxing. CVPR, 2020. 

<h2 id="Fusion with GPS">Fusion with GPS</h2>

- <b>[Multi-sensor navigation algorithm using monocular camera, imu and gps for large scale augmented reality]</b> T. Oskiper. ISMAR, 2012. 

- <b>[Intermittent GPS-aided VIO: Online Initialization and Calibration]</b> Woosik Lee. ICRA, 2020. 

- <b>[Vins Fusion —— A General Optimization-based Framework for Global
Pose Estimation with Multiple Sensors]</b> Tong Qin. 

- <b>[Gomsf: Graph-optimization based multi-sensor fusion for robust uav pose estimation]</b> R. Mascaro, L. ICRA 2018.


<h1 id="SLAM">SLAM</h1>

- <b>[Neural Topological SLAM for Visual Navigation]</b> Devendra Singh Chaplot. CVPR, 2020. 


<h1 id="SfM">SfM</h1>

- <b>[Consistent Video Depth Estimation]</b> XUAN LUO. SIGGRAPH 2020. 

- <b>[unread][DeepSFM: Structure From Motion Via Deep Bundle Adjustment]</b> ECCV 2020. 



<h1 id="Wait">Waiting to sort</h1>

- <b>[FREAK:Fast Retina Keypoint.]</b> A. Amit. CVPR, 2012.

- <b>[Three things evereyone should know to improve object retrieval]</b> R. Arandjelovic. CVPR, 2012. 

- <b>[Learning local feature descriptors with triplets and shallow convolutional neural networks]</b> V. Balntas. BMVC, 2016. 

- <b>[Learning 6D Object Pose Estimation Using 3D Objet Coordinates]</b> E.Brachmann. ECCV, 2014.

- <b>[DSAC-Differentiable RANSAC for Camera Localization]</b> E.Brachmann. CVPR, 2017. 

- <b>[Discriminative Learning of Local Image Descriptors]</b> TPAMI, 2011.


- <b>[MatchNet: Unifying feature and metric learning for patch-based matching]</b>X. Han. CVPR, 2015. 

- <b>[Comparative evaluation of binary features]</b>J. Heinly. ECCV. 

- <b>[PoseNet: A Convolutional Network for Real-Time 6-DOF Camera Relocalization]</b>A. Kendall, M. ICCV, 2015. -

- <b>[LIFT: Learned Invariant Feature Transform]</b> M.Kwang. ECCV, 2016.

- <b>[Semantic Visual Localization]</b> J. L. Schonberger. CVPR, 2018. 

- <b>[Camera Pose Voting for Large-Scale Image-Based Localization]</b> B. Zeisl. ICCV, 2015.. 

- <b>[ASLFeat: Learning Local Features of Accurate Shape and Localization]</b> Zixin, Lup. CVPR, 2020. 

- <b>[City-Scale Localization for Cameras with Known Vertical Direction]</b> Linus Svarm. TAPMI, 2016. 

- <b>[ACNe: Attentive Context Normalization for Robust PermutationEquivariant Learning]</b> Sun, W. CVPR, 2020.

- <b>[Is there anything new to say about SIFT matching?]</b> Fabio Bellavia. IJCV, 2020.

- <b>[Learning to Find Good Correspondences]</b> Kwang Moo Yi. CVPR, 2018, oral.

- <b> [LM-Reloc: Levenberg-Marquardt Based Direct Visual Relocalization] </b> [paper](https://arxiv.org/abs/2010.06323)




