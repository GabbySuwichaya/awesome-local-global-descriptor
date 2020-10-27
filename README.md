# awesome-local-global-descriptor
***This repo will be constantly updated.***
This repo is forked from https://github.com/shamangary/awesome-local-global-descriptor that is written by  

> ***Author: Tsun-Yi Yang (shamangary@hotmail.com)***
This is my personal note about local and global descriptor. Trying to make anyone can get in to these fields more easily.
If you find anything you want to add, feel free to post on issue or email me.

Here, I have modifed the original repo for my own personal use. If there any questions, please feel free to leave some messages. 

# Local matching pipeline

In this section, I focus on the review about the sparse keypoint matching and it's pipeline.

#### 1. Keypoint detection
This subsection includes the review about keypoint detection and it's orientation, scale, or affine transformation estimation.

| Year | Paper | link | Code |
| --- | --- | --- | --- |
|[ICCV19]|  Key.Net: Keypoint Detection by Handcrafted and Learned CNN Filters   |  [PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Barroso-Laguna_Key.Net_Keypoint_Detection_by_Handcrafted_and_Learned_CNN_Filters_ICCV_2019_paper.pdf) |  [Github](https://github.com/axelBarroso/Key.Net)  |
|[ECCV18]| Repeatability Is Not Enough: Learning Discriminative Affine Regions via Discriminability | [arXiv](https://arxiv.org/abs/1711.06704)|[Github](https://github.com/ducha-aiki/affnet)|
|[CVPR17]| Quad-networks: unsupervised learning to rank for interest point detection | [PDF](https://inf.ethz.ch/personal/ladickyl/quad_cvpr17.pdf)| - |
|[CVPR16]| Learning to Assign Orientations to Feature Poitns | - |[Github](https://github.com/vcg-uvic/learn-orientation)|
|[CVPR15]| TILDE: a Temporally Invariant Learned DEtector|[arXiv](https://arxiv.org/abs/1411.4568)|[Github](https://github.com/vcg-uvic/TILDE)|

+ 3D

| Year | Paper | link | Code |
| --- | --- | --- | --- |
|[ICCV19]|USIP: Unsupervised Stable Interest Point Detection from 3D Point Clouds|[arXiv](https://arxiv.org/abs/1904.00229)|[Github](https://github.com/lijx10/USIP)|
|[arXiv19]|Self-Supervised 3D Keypoint Learning for Ego-motion Estimation|[arXiv](https://arxiv.org/abs/1912.03426)|[Github](https://github.com/TRI-ML/KP3D)|

#### 2. Keypoint description (local descriptor)
In the last few decades, people focus on the patch descriptor

+ Hand-crafted

| Year | Paper | link | Code |
| --- | --- | --- | --- |
| [CVPR16] | Accumulated Stability Voting: A Robust Descriptor from Descriptors of Multiple Scales  | [PDF](https://zpascal.net/cvpr2016/Yang_Accumulated_Stability_Voting_CVPR_2016_paper.pdf)  |  [Github](https://github.com/shamangary/asv)  |
|[CVPR15]|Domain-Size Pooling in Local Descriptors: DSP-SIFT|[PDF](https://zpascal.net/cvpr2015/Dong_Domain-Size_Pooling_in_2015_CVPR_paper.pdf)|-|
| [CVPR15] | BOLD - Binary Online Learned Descriptor For Efficient Image Matching  | [PDF](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Balntas_BOLD_-_Binary_2015_CVPR_paper.pdf) |  [Github](https://github.com/vbalnt/bold)  |
|[CVPR13]| Boosting binary keypoint descriptors|-|-|
|[CVPR12]|Freak: Fast retina keypoint|-|-|
|[CVPR12]| Three things everyone should know to improve object retrieval|[PDF](https://www.robots.ox.ac.uk/~vgg/publications/2012/Arandjelovic12/arandjelovic12.pdf)|-|
|[IPOL11]| ASIFT: An Algorithm for Fully Affine Invariant Comparison|-|-|
|[ICCV11]| BRISK: Binary robust invariant scalable keypoints|-|-|
|[ICCV11]| Orb: An efficient alternative to sift or surf|-|-|
|[ICCV11]| Local  inten-sity  order  pattern  for  feature  description |-|-|
|[CVIU06]| Speeded-up robust features (SURF) |-|-|
|[ECCV06]| Surf:Speeded up robust features |-|-|
|[IJCV04]| Distinctive  image  features  from  scale-invariant keypoints |-|[Github](https://github.com/ducha-aiki/pytorch-sift)|
+ Deep learning

| Year | Paper | link | Code |
| --- | --- | --- | --- |
|[TIP19]|Learning Local Descriptors by Optimizing the Keypoint-Correspondence Criterion: Applications to Face Matching, Learning from Unlabeled Videos and 3D-Shape Retrieval|[arXiv](https://arxiv.org/abs/1603.09095)|[Github](https://github.com/nenadmarkus/wlrn)|
|[ICCV19]|Beyond Cartesian Representations for Local Descriptors|[PDF](https://etrulls.github.io/pdf/iccv-2019-logpol.pdf)|-|
|[CVPR19] |SOSNet: Second Order Similarity Regularization for Local Descriptor Learning|[arXiv](https://arxiv.org/abs/1904.05019),[Page](https://research.scape.io/sosnet/)|[Github](https://github.com/scape-research/SOSNet)|
|[ECCV18]| GeoDesc: Learning Local Descriptors by Integrating Geometry Constraints|-|[Github](https://github.com/lzx551402/geodesc)|
|[CVPR18]| Local Descriptors Optimized for Average Precision|[Page](http://cs-people.bu.edu/hekun/papers/DOAP/index.html)|-|
|[NIPS17]| Working hard to know your neighbor's margins: Local descriptor learning loss |[arXiv](https://arxiv.org/abs/1705.10872)|[Github](https://github.com/DagnyT/hardnet)|
|[ICCV17]|DeepCD: Learning Deep Complementary Descriptors for Patch Representations | [PDF](https://www.csie.ntu.edu.tw/~cyy/publications/papers/Yang2017DLD.pdf)|[Github](https://github.com/shamangary/DeepCD)|
|[CVPR17] |L2-Net: Deep Learning of Discriminative Patch Descriptor in Euclidean Space|[PDF](http://openaccess.thecvf.com/content_cvpr_2017/papers/Tian_L2-Net_Deep_Learning_CVPR_2017_paper.pdf)|[Github](https://github.com/yuruntian/L2-Net)|
| [arXiv16] |PN-Net: Conjoined Triple Deep Network for Learning Local Image Descriptors  |  [arXiv](https://arxiv.org/abs/1601.05030) |   [Github](https://github.com/vbalnt/pnnet)  |
|[BMVC16]| Learning local feature descriptors with triplets and shallow convolutional neural networks|[PDF](http://www.bmva.org/bmvc/2016/papers/paper119/paper119.pdf)|[Github](https://github.com/vbalnt/tfeat)|
|[ICCV15]|Discriminative Learning of Deep Convolutional Feature Point Descriptors|[Page](https://esslab.jp/~ess/en/research/deepdesc/)|[Github](https://github.com/etrulls/deepdesc-release)|
|[CVPR15]|MatchNet: Unifying Feature and Metric Learning for Patch-Based Matching|[PDF](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Han_MatchNet_Unifying_Feature_2015_CVPR_paper.pdf)|-|
|[CVPR15]|Learning to compare image patches via convolutional neural networks|[PDF](http://openaccess.thecvf.com/content_cvpr_2015/supplemental/Zagoruyko_Learning_to_Compare_2015_CVPR_supplemental.pdf)|[Github](https://github.com/szagoruyko/cvpr15deepcompare)|



+ 3D

| Year | Paper | link | Code |
| --- | --- | --- | --- |
|[arXiv19]|DEEPPOINT3D: LEARNING DISCRIMINATIVE LOCAL DESCRIPTORS USING DEEP METRIC LEARNING ON 3D POINT CLOUDS|[arXiv](https://arxiv.org/abs/1904.00817)|-|


#### 3. Feature extraction pipeline
#### 3.1 End-to-end feature extraction pipeline
Recently, more and more papers try to embed the whole matching pipeline (keypoint detection, keypoint description) into one framework. 

| Year | Paper | link | Code |
| --- | --- | --- | --- |
|[arXiv19]|Reinforced Feature Points: Optimizing Feature Detection and Description for a High-Level Task|[arXiv](https://128.84.21.199/abs/1912.00623)|-|
|[NIPS19]|R2D2: Repeatable and Reliable Detector and Descriptor|[arXiv](https://arxiv.org/abs/1906.06195),[Page](https://nips.cc/Conferences/2019/Schedule?showEvent=15782)|[Github](https://github.com/naver/r2d2)|
|[ICCV19]|ELF: Embedded Localisation of Features in Pre-Trained CNN|[PDF](http://openaccess.thecvf.com/content_ICCV_2019/papers/Benbihi_ELF_Embedded_Localisation_of_Features_in_Pre-Trained_CNN_ICCV_2019_paper.pdf)|[Github](https://github.com/abenbihi/elf)|
|[CVPR19]|RF-Net: An End-to-End Image Matching Network based on Receptive Field|[arXiv](https://arxiv.org/abs/1906.00604)|[Github](https://github.com/Xylon-Sean/rfnet)|
| [CVPR19] |  D2-Net: A Trainable CNN for Joint Description and Detection of Local Features   |  [arXiv](https://arxiv.org/pdf/1905.03561),[Page](https://dsmn.ml/publications/d2-net.html)  |  [Github](https://github.com/mihaidusmanu/d2-net)  |
| [CVPRW18] | SuperPoint: Self-Supervised Interest Point Detection and Description | [arXiv](https://arxiv.org/abs/1712.07629)|[Github](https://github.com/rpautrat/SuperPoint)|
| [NIPS18] | LF-Net: Learning Local Features from Images |[PDF](https://papers.nips.cc/paper/7861-lf-net-learning-local-features-from-images.pdf)|[Github](https://github.com/vcg-uvic/lf-net-release)|
| [ECCV16] | LIFT: Learned Invariant Feature Points |-|[Github](https://github.com/cvlab-epfl/LIFT)|

#### 3.2 End-to-end matching pipeline


#### 4. Geometric verification or learning based matcher
After the matching, standard RANSAC and it's variants are usually adopted for outlier removal.

+ Algorithm based

| Year | Paper | link | Code |
| --- | --- | --- | --- | 
| [Arxiv2020] | AdaLAM: Revisiting Handcrafted Outlier Detection |[PDF](https://arxiv.org/pdf/2006.04250.pdf) | [Github](https://github.com/cavalli1234/AdaLAM) |
| [ECCV20] | Multi-View Optimization of Local Feature Geometry |[PDF](https://arxiv.org/abs/2003.08348) |[Github](https://github.com/mihaidusmanu/local-feature-refinement) | 
| [CVPR19] |  MAGSAC: Marginalizing Sample Consensus  | [PDF](http://openaccess.thecvf.com/content_CVPR_2019/papers/Barath_MAGSAC_Marginalizing_Sample_Consensus_CVPR_2019_paper.pdf)  | [Github](https://github.com/danini/magsac)  |
|[ECCV12]| Improving Image-Based Localization by Active Correspondence Search| [PDF](https://www.graphics.rwth-aachen.de/media/papers/sattler_eccv12_preprint_1.pdf)| - |
| [CVPR05] | Matching with PROSAC – Progressive Sample Consensus |[PDF](https://dspace.cvut.cz/bitstream/handle/10467/9496/2005-Matching-with-PROSAC-progressive-sample-consensus.pdf;jsessionid=F52133C01BA4F1B36C718896C0F335A1?sequence=1) |- |


+ Deep learning based

| Year | Paper | link | Code |
| --- | --- | --- | --- |
| [CVPR2020] | SuperGlue: Learning Feature Matching with Graph Neural Networks |[arXiv](https://arxiv.org/abs/1911.11763)|[Official Github](https://github.com/magicleap/SuperGluePretrainedNetwork) [Trainingscript with License](https://github.com/HeatherJiaZG/SuperGlue-pytorch)|
|[ICCV19]|NG-RANSAC for Epipolar Geometry from Sparse Correspondences|[arXiv](https://arxiv.org/abs/1905.04132)|[Github](https://github.com/vislearn/ngransac)|
| [ICCV19] | Learning Two-View Correspondences and Geometry Using Order-Aware Network (OANet) | [arXiv](https://arxiv.org/abs/1908.04964) |[Github](https://github.com/zjhthu/OANet)|
| [CVPR18] | Learning to Find Good Correspondences |  -  |  [Github](https://github.com/vcg-uvic/learned-correspondence-release) |

+ Image registration

| Year | Paper | link | Code |
| --- | --- | --- | --- |
|[Access18]|Multi-Temporal Remote Sensing Image Registration Using Deep Convolutional Features|[PDF](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8404075)|[Github](https://github.com/yzhq97/cnn-registration)|


# Global retrieval

Consider global retrieval usually targets on a lot of candidates, there are several way to generate one single description for one image.

#### 1. Feature aggregation

+ Hand-crafted

When there is only hand-crafted local descriptors, people usually uses feature aggregation from a set of local descriptors and output a single description.

| Year | Paper | link | Code |
| --- | --- | --- | --- |
|[CVPR13]|All about VLAD|[PDF](https://www.robots.ox.ac.uk/~vgg/publications/2013/arandjelovic13/arandjelovic13.pdf)|-|
|[ECCV10]|Improving the fisher kernel for large-scale image classification|[PDF](https://lear.inrialpes.fr/pubs/2010/PSM10/PSM10_0766.pdf)|-|
|[CVPR07]|Object retrieval with large vocabularies and fast spatial matching|[PDF](http://www.robots.ox.ac.uk:5000/~vgg/publications/2007/Philbin07/philbin07.pdf)|-|
|[CVPR06]|Fisher kenrels on visual vocabularies for image categorizaton|[PDF](http://www.ee.oulu.fi/research/imag/courses/Vedaldi/2006-034.pdf)|-|

+ Deep learning

Similar idea but use deep learning to adapt classical algorithm

| Year | Paper | link | Code |
| --- | --- | --- | --- |
|[ECCV16]|CNN Image Retrieval Learns from BoW: Unsupervised Fine-Tuning with Hard Examples. |[PDF](http://cmp.felk.cvut.cz/~chum/papers/Radenovic-ECCV16.pdf)|-|
|[CVPR16]|NetVLAD: CNN architecture for weakly supervised place recognition|[Page](https://www.di.ens.fr/willow/research/netvlad/)|[Github](https://github.com/Relja/netvlad)|




#### 2. Real-valued descriptor

One single representation from the image.

| Year | Paper | link | Code |
| --- | --- | --- | --- |
|[ECCV'20]|Learning and aggregating deep local descriptors for instance-level recognition | [arxiv](https://arxiv.org/abs/2007.13172) | | [Github](https://github.com/jenicek/asmk)  |
|[arXiv20]|Unifying Deep Local and Global Features for Efficient Image Search|[arXiv](https://arxiv.org/abs/2001.05027)|-|
|[arXiv19]|ACTNET: end-to-end learning of feature activations and multi-stream aggregation for effective instance image retrieval|[arXiv](https://arxiv.org/abs/1907.05794?fbclid=IwAR1R6HbcmocY_Goso5K8W8rhjmtNIxyGw2tUXObw12JR3QIbjEAVQGXZL8Q)|-|
|[TIP19]|REMAP: Multi-layer entropy-guided pooling of dense CNN features for image retrieval|[arXiv](https://arxiv.org/abs/1906.06626)|-|
|[ICCV19]|Learning with Average Precision: Training Image Retrieval with a Listwise Loss |[arXiv](https://arxiv.org/abs/1906.07589)|[Github](https://github.com/almazan/deep-image-retrieval)|
| [CVPR19] | Detect-to-Retrieve: Efficient Regional Aggregation for Image Search | [PDF](http://openaccess.thecvf.com/content_CVPR_2019/papers/Teichmann_Detect-To-Retrieve_Efficient_Regional_Aggregation_for_Image_Search_CVPR_2019_paper.pdf) |[Github](https://github.com/tensorflow/models/tree/master/research/delf)|
| [TPAMI18] |   Fine-tuning CNN Image Retrieval with No Human Annotation |[arXiv](https://arxiv.org/abs/1711.02512)  |  [Github](https://github.com/filipradenovic/cnnimageretrieval-pytorch)  |
|[IJCV17]| End-to-end Learning of Deep Visual Representations for Image Retrieval |[arXiv](https://arxiv.org/abs/1610.07940)|[Github](https://github.com/almazan/deep-image-retrieval)|
|[ICCV17]| Large-Scale Image Retrieval with Attentive Deep Local Features|-|[Github](https://github.com/tensorflow/models/tree/master/research/delf)|
| [ECCV16] | CNN Image Retrieval Learns from BoW: Unsupervised Fine-Tuning with Hard Examples  |   [arXiv](https://arxiv.org/abs/1604.02426) |  [Github](https://github.com/filipradenovic/cnnimageretrieval-pytorch)  |

#### 3. Binary descriptor and quantization
For more compact representation, a binary descriptor can be generated from hashing or thresholding. Quantization is also very popular in large-scale image retrieval.

| Year | Paper | link | Code |
| --- | --- | --- | --- |
| [ICCVW19] | DAME WEB: DynAmic MEan with Whitening Ensemble Binarization for Landmark Retrieval without Human Annotation | [PDF](http://openaccess.thecvf.com/content_ICCVW_2019/papers/CEFRL/Yang_DAME_WEB_DynAmic_MEan_with_Whitening_Ensemble_Binarization_for_Landmark_ICCVW_2019_paper.pdf) | [Github](https://github.com/scape-research/DAME-WEB)|
|[CVPR19]|FastAP: Deep Metric Learning to Rank|[PDF](http://openaccess.thecvf.com/content_CVPR_2019/papers/Cakir_Deep_Metric_Learning_to_Rank_CVPR_2019_paper.pdf)|[Github](https://github.com/kunhe/FastAP-metric-learning)|
|[CVPR18]|Hashing as Tie-Aware Learning to Rank|[PDF](http://openaccess.thecvf.com/content_cvpr_2018/papers/He_Hashing_as_Tie-Aware_CVPR_2018_paper.pdf)|[Github](https://github.com/kunhe/TALR)|
|[AAAI18]| Deep Region Hashing for Generic Instance Search from Image| - | - |
|[TPAMI18]| Supervised Learning of Semantics-Preserving Hash via Deep Convolutional NeuralNetworks |-|-|
|[TPAMI13]| Iterative Quantization: A Procrustean Approach to Learning Binary Codes for Large-Scale Image Retrieval|[PDF](http://refbase.cvc.uab.es/files/GLG2012b.pdf)|-|
|[TPAMI10]| Product quantization for nearest neighbor search  |[PDF](https://core.ac.uk/download/pdf/48207765.pdf)|  -  |


#### 5. Post-processing
Anything can boost the performance in the post-processing stage such as re-ranking or query expansion.

| Year | Paper | link | Code |
| --- | --- | --- | --- |
| [CVPR19] | Local features and visual words emerge in activations |[PDF](https://zpascal.net/cvpr2019/Simeoni_Local_Features_and_Visual_Words_Emerge_in_Activations_CVPR_2019_paper.pdf) | -  |
|[CVPR12]|Object retrieval and localization with spatially-constrained similarity measure and k-NN re-ranking|[PDF](https://www.researchgate.net/profile/Jonathan_Brandt/publication/261168759_Object_retrieval_and_localization_with_spatially-constrained_similarity_measure_and_k-NN_re-ranking/links/5613d2c608ae983c1b4019d7.pdf)|-|

#### 6. 3d point cloud

| Year | Paper | link | Code |
| --- | --- | --- | --- |
|[CVPR18]|PointNetVLAD: Deep Point Cloud Based Retrieval for Large-Scale Place Recognition|[arXiv](https://arxiv.org/abs/1804.03492)|[Github](https://github.com/mikacuy/pointnetvlad)|


# Multi-tasking local and global descriptors
Some works try to cover both local descriptor and global retrieval due to the shared similarity about the activation and the applications.

| Year | Paper | link | Code |
| --- | --- | --- | --- |
|[arXiv20]|UR2KiD: Unifying Retrieval, Keypoint Detection, and Keypoint Description without Local Correspondence Supervision|[arXiv](https://arxiv.org/abs/2001.07252)|-|
| [CVPR19] | ContextDesc: Local Descriptor Augmentation with Cross-Modality Context | - |[Github](https://github.com/lzx551402/contextdesc)|
| [CVPR19] | From Coarse to Fine: Robust Hierarchical Localization at Large Scale with HF-Net  |   [arXiv](https://arxiv.org/pdf/1812.03506)  |  [Github](https://github.com/ethz-asl/hfnet)  |
|[ICCV17]| Large-Scale Image Retrieval with Attentive Deep Local Features (DELF)|-|[Github](https://github.com/tensorflow/models/tree/master/research/delf)|

# Benchmarks

#### Local matching

| Year | Paper | link | Code | Note |
| --- | --- | --- | --- | --- |
|[CVPR17]| HPatches: A benchmark and evaluation of handcrafted and learned local descriptors | [arXiv](https://arxiv.org/pdf/1704.05939) |[Github](https://github.com/hpatches) |Hpatches|
|[TPAMI11]| Discriminative learning of local image descriptors|[Page](http://matthewalunbrown.com/patchdata/patchdata.html)|-|UBC/Brown dataset (subsets:Liberty (New York), Notre Dame (Paris) and Half Dome (Yosemite))|
|[CVPR08]|On Benchmarking Camera Calibration and MultiView Stereo for High Resolution Imagery|||

#### Global retrieval

| Year | Paper | link | Code | Note |
| --- | --- | --- | --- | --- |
|[CVPR18]|Revisiting Oxford and Paris: Large-Scale Image Retrieval Benchmarking|[Page](http://cmp.felk.cvut.cz/revisitop/)|[Github](https://github.com/filipradenovic/revisitop)| ROxford5k, RParis6k |
|[CVPR07]|Object retrieval with large vocabularies and fast spatial matching |[Page](https://www.robots.ox.ac.uk/~vgg/data/oxbuildings/)|-|Oxford5k|
|[CVPR08]|Lost in Quantization: Improving Particular Object Retrieval in Large Scale Image Databases  |[Page](https://www.robots.ox.ac.uk/~vgg/data/parisbuildings/)|-|Paris6k|

#### Localization (both local matching and global retrieval)

| Year | Paper | link | Code | Note |
| --- | --- | --- | --- | --- |
| [CVPR18]|Benchmarking 6DOF Outdoor Visual Localization in Changing Conditions|[PDF](http://openaccess.thecvf.com/content_cvpr_2018/papers/Sattler_Benchmarking_6DOF_Outdoor_CVPR_2018_paper.pdf),[Page](https://www.visuallocalization.net/)| [Github](https://github.com/tsattler/visuallocalizationbenchmark)|Aachen-day-night, Robotcar, CMU-seasons|


## Awsome UR2KiD Summary

<img src="https://github.com/shamangary/awesome-local-global-descriptor/blob/master/ur2kid_summary.png" height="540"/>

This repo is also a side product when I was doing the survey of our paper UR2KID. If you find this repo useful, please also consider to cite our paper.
```
@article{yang2020ur2kid,
  title={UR2KiD: Unifying Retrieval, Keypoint Detection, and Keypoint Description without Local Correspondence Supervision},
  author={Yang*, Tsun-Yi; Nguyen*, Duy-Kien; Heijnen, Huub; Balntas, Vassileios},
  journal={arXiv preprint arXiv:2001.07252},
  year={2020}
}
```
