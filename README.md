# List of SfM approaches based on their category<br>

## SfM
### •	Global SfM<br>
While Incremental SfM approaches repeatedly executes bundle adjustment whenever a new image is added to the model, Global SfMs usually calls the bundle adjustment once in which all image parameters are optimised at the same time.<br>

•	Global Structure-from-Motion by Similarity Averaging (ICCV 2015) [Paper](http://openaccess.thecvf.com/content_iccv_2015/papers/Cui_Global_Structure-From-Motion_by_ICCV_2015_paper.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[Link](https://zhpcui.github.io/projects/ICCV2015_SfM/index.html)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	Implementation may have been included in [OpenMVG](https://github.com/openMVG/openMVG) as found in this [issue](https://github.com/openMVG/openMVG/issues/1241). <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	My summary (in pdf) can be found [here](https://github.com/stanathong/SfM-list/blob/master/paper-review/Review%20-%20Global%20Structure-from-Motion%20by%20Similarity%20Averaging.pdf).<br>
•	Optimizing the viewing graph for structure-from-motion (ICCV 2015) [Paper](http://openaccess.thecvf.com/content_iccv_2015/papers/Sweeney_Optimizing_the_Viewing_ICCV_2015_paper.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[TheiaSfM-Github](https://github.com/sweeneychris/TheiaSfM)&nbsp;&nbsp;&nbsp;&nbsp;[Theia-Library-Page](http://www.theia-sfm.org/)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	_Additional Note:_ [TheiaSfM](https://github.com/sweeneychris/TheiaSfM) offers the ability to perform either incremental and global SfM.<br>
•	Robust global translations with 1dsfm. (ECCV 2014) [Paper](http://www.cs.cornell.edu/projects/1dsfm/docs/1DSfM_ECCV14.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[Link](http://www.cs.cornell.edu/projects/1dsfm/)<br>
•	Global fusion of relative motions for robust, accurate and scalable structure from motion. (ICCV 2013) [Paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Moulon_Global_Fusion_of_2013_ICCV_paper.pdf)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	In this paper, a new robust global SfM for unordered images is proposed.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	[OpenMVG](https://github.com/openMVG/openMVG)'s main global SfM is based on this paper, as can be seen in [openMVG_main_GlobalSfM](http://openmvg.readthedocs.io/en/latest/software/SfM/GlobalSfM/).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• _Note on Georeferencing:_	[OpenMVG](https://github.com/openMVG/openMVG) reads GPS data from exif and uses them in the pose optimisation process. (Using GPS is not a default option) <br>
•	A Global Linear Method for Camera Pose Registration (ICCV 2013) [Paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Jiang_A_Global_Linear_2013_ICCV_paper.pdf)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	Part of this work has been implemented in [TheiaSfM](https://github.com/sweeneychris/TheiaSfM), see this [file](https://github.com/sweeneychris/TheiaSfM/blob/master/src/theia/sfm/global_pose_estimation/linear_position_estimator.h).<br>

### •	Incremental SfM<br>
The approach repeatedly perform bundle adjustment when new images (typically one image) are added to the existing model.<br>

•	Structure-from-Motion Revisited (CVPR 2016) [Paper](http://openaccess.thecvf.com/content_cvpr_2016/papers/Schonberger_Structure-From-Motion_Revisited_CVPR_2016_paper.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[COLMAP-Github](https://github.com/colmap/colmap)&nbsp;&nbsp;&nbsp;&nbsp;[COLMAP-Page](https://colmap.github.io/)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• _Note on Georeferencing:_	[COLMAP](https://github.com/colmap/colmap) does not use GPS priors in their pose optimisation process, referred to this [question](https://github.com/colmap/colmap/issues/98) _(April 2017)_. <br>
•	Towards linear-time incremental structure from motion (3DV 2013) [Paper](http://ccwu.me/vsfm/vsfm.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[VisualSFM](http://www.ccwu.me/vsfm/)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• _Note on Georeferencing:_	[VisualSFM](http://www.ccwu.me/vsfm/) does not use GPS priors in the incremental SfM process. The poses and scales are arbitrary and like many tools it offers similarity transformation to adjust the final poses to align with the GPS data. <br>
•	Adaptive structure from motion with a contrario model estimation (ACCV 2012) [Paper](http://imagine.enpc.fr/~marletr/publi/ACCV-2012-Moulon-et-al.pdf)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	[OpenMVG](https://github.com/openMVG/openMVG)'s implementation of incremental SfM is based on this paper.<br>
•	Building Rome on a cloudless day (ECCV 2010) [Paper](http://cs.unc.edu/~jmf/publications/Frahm_et_al_ReconstructionFromPhotoCollection.pdf) <br>
•	Photo Tourism - Exploring Photo Collections in 3D (SIGGRAPH 2006) [Paper](http://phototour.cs.washington.edu/Photo_Tourism.pdf)&nbsp;&nbsp;&nbsp;&nbsp;[Bundler-Github](https://github.com/snavely/bundler_sfm)&nbsp;&nbsp;&nbsp;&nbsp;[Project Page](http://www.cs.cornell.edu/~snavely/bundler/)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• _Note on Georeferencing:_	[Bundler-Github](https://github.com/snavely/bundler_sfm) does not use GPS priors in their pose optimisation process, referred to this [question](https://github.com/snavely/bundler_sfm/issues/38) _(September 2016)_. <br>
•	OpenSfM : Open Source Structure from Motion [OpenSfM-Github](https://github.com/mapillary/OpenSfM)&nbsp;&nbsp;&nbsp;&nbsp;[OpenSfM Page](http://opensfm.readthedocs.io/en/latest/)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	Documentation in _PDF_ can be found [here](https://media.readthedocs.org/pdf/opensfm/latest/opensfm.pdf).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	Incremental SfM pipeline implementation in OpenSfM is discussed [here](http://opensfm.readthedocs.io/en/latest/reconstruction_module.html).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•	The Mapillary Blog is [here](https://blog.mapillary.com/update/2016/10/31/denser-3d-point-clouds-in-opensfm.html).<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;• _Note on Georeferencing:_	[OpenSfM](https://github.com/mapillary/OpenSfM) can be configured to use GPS data in the image exif as pose prior in the optimisation process. <br>

### •	Hybrid SfM
A combination approach of incremental SfM and global SfM.<br>

•	HSfM: Hybrid Structure-from-Motion (CVPR 2017) [Paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Cui_HSfM_Hybrid_Structure-from-Motion_CVPR_2017_paper.pdf)<br>

### •	Hierarchical SfM
