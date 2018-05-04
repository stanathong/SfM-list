# List of SfM approaches based on their category<br>

## SfM
### •	Global SfM<br>
While Incremental SfM approaches repeatedly executes bundle adjustment whenever a new image is added to the model, Global SfMs usually calls the bundle adjustment once in which all image parameters are optimised at the same time.<br>

•	Global Structure-from-Motion by Similarity Averaging (ICCV 2015) [Paper](http://openaccess.thecvf.com/content_iccv_2015/papers/Cui_Global_Structure-From-Motion_by_ICCV_2015_paper.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[Link](https://zhpcui.github.io/projects/ICCV2015_SfM/index.html)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	Implementation may have been included in [OpenMVG](https://github.com/openMVG/openMVG) as found in this [issue](https://github.com/openMVG/openMVG/issues/1241). <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	My summary (in pdf) can be found [here](https://github.com/stanathong/SfM-list/blob/master/paper-review/Review%20-%20Global%20Structure-from-Motion%20by%20Similarity%20Averaging.pdf).<br>
•	Optimizing the viewing graph for structure-from-motion (ICCV 2015) [Paper](http://openaccess.thecvf.com/content_iccv_2015/papers/Sweeney_Optimizing_the_Viewing_ICCV_2015_paper.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[TheiaSfM-Github](https://github.com/sweeneychris/TheiaSfM)&nbsp;&nbsp;&nbsp;&nbsp;[Theia-Library-Page](http://www.theia-sfm.org/)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	__Note:__ __TheiaSfM__ offers the ability to perform either incremental and global SfM.<br>
•	Robust global translations with 1dsfm. (ECCV 2014) [Paper](http://www.cs.cornell.edu/projects/1dsfm/docs/1DSfM_ECCV14.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[Link](http://www.cs.cornell.edu/projects/1dsfm/)<br>
•	Global fusion of relative motions for robust, accurate and scalable structure from motion. (ICCV 2013) [Paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Moulon_Global_Fusion_of_2013_ICCV_paper.pdf)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	In this paper, a new robust global SfM for unordered images is proposed.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	[OpenMVG](https://github.com/openMVG/openMVG)'s main global SfM is based on this paper, as can be seen in [openMVG_main_GlobalSfM](http://openmvg.readthedocs.io/en/latest/software/SfM/GlobalSfM/).<br>
•	A Global Linear Method for Camera Pose Registration (ICCV 2013) [Paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Jiang_A_Global_Linear_2013_ICCV_paper.pdf)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	Part of this work has been implemented in [TheiaSfM](https://github.com/sweeneychris/TheiaSfM), see this [file](https://github.com/sweeneychris/TheiaSfM/blob/master/src/theia/sfm/global_pose_estimation/linear_position_estimator.h).<br>

### •	Incremental SfM<br>
The approach repeatedly perform bundle adjustment when new images (typically one image) are added to the existing model.<br>

•	Structure-from-Motion Revisited (CVPR 2016) [Paper](http://openaccess.thecvf.com/content_cvpr_2016/papers/Schonberger_Structure-From-Motion_Revisited_CVPR_2016_paper.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[COLMAP-Github](https://github.com/colmap/colmap)&nbsp;&nbsp;&nbsp;&nbsp;[COLMAP-Page](https://colmap.github.io/)<br>
•	Towards linear-time incremental structure from motion (3DV 2013) [Paper](http://ccwu.me/vsfm/vsfm.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[VisualSFM](http://www.ccwu.me/vsfm/)<br>
•	Building Rome on a cloudless day (ECCV 2010) [Paper](http://cs.unc.edu/~jmf/publications/Frahm_et_al_ReconstructionFromPhotoCollection.pdf) <br>
•	Photo Tourism - Exploring Photo Collections in 3D (SIGGRAPH 2006) - Bundler<br>
### •	Hierarchical SfM
### •	Hybrid SfM
