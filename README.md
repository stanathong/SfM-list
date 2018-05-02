# List of SfM approaches based on their category<br>

## SfM
### •	Global SfM<br>
While Incremental SfM approaches repeatedly executes bundle adjustment whenever a new image is added to the model, Global SfMs usually calls the bundle adjustment once in which all image parameters are optimised at the same time.<br>

•	Global Structure-from-Motion by Similarity Averaging (ICCV 2015) [Paper](http://openaccess.thecvf.com/content_iccv_2015/papers/Cui_Global_Structure-From-Motion_by_ICCV_2015_paper.pdf)  [Link](https://zhpcui.github.io/projects/ICCV2015_SfM/index.html)<br>
•	Optimizing the viewing graph for structure-from-motion (ICCV 2015) [Paper](http://openaccess.thecvf.com/content_iccv_2015/papers/Sweeney_Optimizing_the_Viewing_ICCV_2015_paper.pdf)  [TheiaSfM-Github](https://github.com/sweeneychris/TheiaSfM)  [Theia-Library-Page](http://www.theia-sfm.org/)<br>
•	Robust global translations with 1dsfm. (ECCV 2014) [Paper](http://www.cs.cornell.edu/projects/1dsfm/docs/1DSfM_ECCV14.pdf)   [Link](http://www.cs.cornell.edu/projects/1dsfm/)<br>
•	Global fusion of relative motions for robust, accurate and scalable structure from motion. (ICCV 2013) [Paper](http://openaccess.thecvf.com/content_iccv_2013/papers/Moulon_Global_Fusion_of_2013_ICCV_paper.pdf)<br>
    A new robust global SfM for unordered images is proposed.<br>
•	A Global Linear Method for Camera Pose Registration (ICCV 2013)<br>
### •	Incremental SfM<br>
The approach repeatedly perform bundle adjustment when new images (typically one image) are added to the existing model.<br>

•	Structure-from-Motion Revisited (CVPR 2016) - COLMAP<br>
•	Towards linear-time incremental structure from motion (3DV 2013) - VisualSFM<br>
•	Building Rome on a cloudless day (ECCV 2010) [Paper](http://cs.unc.edu/~jmf/publications/Frahm_et_al_ReconstructionFromPhotoCollection.pdf) <br>
•	Photo Tourism - Exploring Photo Collections in 3D (SIGGRAPH 2006) - Bundler<br>
### •	Hierarchical SfM
### •	Hybrid SfM
