# Camera-relocalization-papers

Contributed by Dehao Zhang.

The relocalization task aims to estimate the 6-DoF pose of a novel (unseen) frame in the coordinate system given by the prior model of the world. 



**TOC**

| Section | # of Papers |
|:---:|:---:|
|[Survey papers](#Surveys) | 1|
|[System](#system) | 6 |
|[Retrieval methods](#Retrieval) | 4 |
|[Pose Estimation](#Pose) | 0 |

\* 📒 means there are detailed notes in the notes branch,



<h1 id="Surveys">Survey papers</h1>

<details>
<summary> <b>【[Image-based camera localization: an overview】</b> ihong Wu. Visual Computing for Industry, Biomedicine, and Art, 2018. 📒</summary>
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
<summary> <b>【Parallel Tracking and Mapping on a Camera Phone】</b> ISMAR, 2009</summary>
</details>

<details>
<summary> <b>【Pose Tracking from Natural Features on Mobile Phones】</b> ISMAR, 2008</summary>
</details>
<details>
<summary> <b>【Scalable 6-DOF Localization on Mobile Devices】</b> Iven Middelberg, Torsten Sattler. ECCV, 2014. 📒</summary>
This work combines the local tracking and global relocalization so they throwed the loop closuring in the tracking. The main contributions of this paper are the three align methods: alignment only once, alignment using the global keyframe positions and alignmnet Using the global 2D-3D matches.
</details>


<details>
<summary> <b>【6D dynamic camera relocalization from single reference image】</b> Feng W. CVPR 2016. </summary>
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




