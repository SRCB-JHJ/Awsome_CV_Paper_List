# Awsome_CV_Paper_List

VCL page (https://github.com/VCL3D)

## 1. Depth and Surface normal
基于学习方法的单帧图像深度图、表面法向量图预测综述 (https://zhuanlan.zhihu.com/p/68903112;https://zhuanlan.zhihu.com/p/68902039;https://zhuanlan.zhihu.com/p/62248924;https://zhuanlan.zhihu.com/p/68363491) 

(3DV2019)Spherical View Synthesis for Self-Supervised **360** Depth Estimation [[code]](https://github.com/VCL3D/SphericalViewSynthesis)

(3DV2019)Pano Popups: Indoor 3D Reconstruction with a Plane-Aware Network⭐️

(3DV2019)**360** Surface Regression with a Hyper-Sphere Loss [[code]](https://github.com/VCL3D/HyperSphereSurfaceRegression) [[project]](https://vcl3d.github.io/HyperSphereSurfaceRegression/)⭐️

(CVPR2019) Learning Single-Image Depth from **Videos** using Quality Assessment Networks [[code]](https://github.com/princeton-vl/YouTube3D) [[project]](http://www-personal.umich.edu/~wfchen/youtube3d/)

(ECCV2018)OmniDepth: Dense Depth Estimation for Indoors ***Spherical Panoramas*** [[code]](https://github.com/meder411/OmniDepth-PyTorch)

 (CVPR2018)Deep **depth completion** of a single rgb-d image [[code]](https://github.com/yindaz/DeepCompletionRelease) [[project]](http://deepcompletion.cs.princeton.edu/)

 (CVPR2018)GeoNet: Geometric Neural Network for Joint Depth and Surface Normal Estimation [[code]](https://github.com/xjqi/GeoNet)
 
 GeoNet++: Interative Geometric Neural network with Edge-aware Refinement Joint Depth and Surface Normal Estimation. (In preparation)
 
 (CVPR2018)Deep Depth Completion of a Single RGB-D Image [[code]](https://github.com/yindaz/DeepCompletionRelease)
 
 (CVPR2017)Physically-based rendering for indoor scene understanding using convolutional neural networks [[code]](https://github.com/yindaz/surface_normal)
 
 (ICCV2015)Predicting Depth, Surface Normals and Semantic Labels with a Common Multi-Scale Convolutional Architecture [[code/project]](https://cs.nyu.edu/~deigen/dnl/)
 
 (ECCV2012)Indoor Segmentation and Support Inference from RGBD Images [[GT generation code/project]](https://cs.nyu.edu/~silberman/projects/indoor_scene_seg_sup.html)
 
 ## 2. Planar
 (CVPR2019 oral)PlaneRCNN: 3D Plane Detection and Reconstruction from a Single Image [[code]](https://github.com/NVlabs/planercnn)🔥
 
 ## 3. Layout
(ECCV2014)PanoContext: A Whole-room 3D Context Model for Panoramic Scene Understanding [[code]](https://github.com/yindaz/PanoBasic)
 
 
 # Dataset
 ## Depth and Surface (segmentation)
 3D60:The 3D60 dataset is split in three parts, each one representing a different viewpoint (i.e. left/down/center, right and up), and each one containing all three available modalities (i.e. color image, depth and normal maps) [[github]](https://vcl3d.github.io/3D60/)[[github]](https://vcl.iti.gr/360-dataset/)[[toolset]](https://github.com/VCL3D/3D60)
 
 ## Planar
 ScanNet[[github]](https://github.com/ScanNet/ScanNet):RGB-D sequence. Each sequence is stored under a directory with named scene<spaceId>_<scanId>, or scene%04d_%02d, where each space corresponds to a unique location (0-indexed). The raw data captured during scanning, camera poses and surface mesh reconstructions, and annotation metadata are all stored together for the given sequence. The directory has the following structure:
 
 <scanId>
|-- <scanId>.sens
    RGB-D sensor stream containing color frames, depth frames, camera poses and other data
|-- <scanId>_vh_clean.ply
    High quality reconstructed mesh
|-- <scanId>_vh_clean_2.ply
    Cleaned and decimated mesh for semantic annotations
|-- <scanId>_vh_clean_2.0.010000.segs.json
    Over-segmentation of annotation mesh
|-- <scanId>.aggregation.json, <scanId>_vh_clean.aggregation.json
    Aggregated instance-level semantic annotations on lo-res, hi-res meshes, respectively
|-- <scanId>_vh_clean_2.0.010000.segs.json, <scanId>_vh_clean.segs.json
    Over-segmentation of lo-res, hi-res meshes, respectively (referenced by aggregated semantic annotations)
|-- <scanId>_vh_clean_2.labels.ply
    Visualization of aggregated semantic segmentation; colored by nyu40 labels (see img/legend; ply property 'label' denotes the ScanNet label id)
|-- <scanId>_2d-label.zip
    Raw 2d projections of aggregated annotation labels as 16-bit pngs with ScanNet label ids
|-- <scanId>_2d-instance.zip
    Raw 2d projections of aggregated annotation instances as 8-bit pngs
|-- <scanId>_2d-label-filt.zip
    Filtered 2d projections of aggregated annotation labels as 16-bit pngs with ScanNet label ids
|-- <scanId>_2d-instance-filt.zip
    Filtered 2d projections of aggregated annotation instances as 8-bit pngs
 
 
 
 


