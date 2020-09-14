# The list of vision-based SLAM / Visual Odometry open source projects, libraries, dataset, tools, and studies

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/tzutalin/awesome-visual-slam)

## Index
* [Libraries](#libraries)
* [Dataset](#dataset)
* [Tools](#tools)
* [Projects](#projects)
* [Learn](pages/learn.md)
* [Miscellaneous](pages/miscellaneous.md)

## Libraries
###### Basic vision and trasformation libraries
- [OpenCV](http://opencv.org/)
- [Eigen](http://eigen.tuxfamily.org/index.php?title=Main_Page)
- [Sophus](https://github.com/strasdat/Sophus)
- [ROS](http://www.ros.org/)
- [PointCloud](http://pointclouds.org/)

###### Thread-safe queue libraries
- [concurrentqueue](https://github.com/cameron314/concurrentqueue)
- [Intel® TBB](https://www.threadingbuildingblocks.org/)
- [Facebook folly PC](https://github.com/facebook/folly/blob/master/folly/ProducerConsumerQueue.h)

###### Loop detection
- [dorian3d](https://github.com/dorian3d)

###### Graph Optimization
- [ceres-solver](https://github.com/ceres-solver/ceres-solver)
- [g2o](https://github.com/RainerKuemmerle/g2o)
- [gtsam](https://collab.cc.gatech.edu/borg/gtsam?destination=node%2F299)
- [Vertigo](http://openslam.org/vertigo.html)

###### Map library
- [ETHZ ASL/Grip Map](https://github.com/ethz-asl/grid_map)
- [OmniMapper](https://github.com/CognitiveRobotics/omnimapper/wiki)
- [OctoMap](https://github.com/OctoMap/octomap)

## Dataset

Dataset for benchmark/test/experiment/evalutation

- [TUM Universtiy](http://vision.in.tum.de/data/datasets/rgbd-dataset/download)
- [KITTI Vision benchmark](http://www.cvlibs.net/datasets/kitti/eval_odometry.php)
- [UNI-Freiburg](http://kaspar.informatik.uni-freiburg.de/~slamEvaluation/datasets.php)
- [ADVIO](https://github.com/AaltoVision/ADVIO)
- [Oxford RobotCar Dataset](https://robotcar-dataset.robots.ox.ac.uk/)
- [HRI (Honda Research Institute) Driving Datasets](https://usa.honda-ri.com/honda-driving-datasets)
- [Argoverse](https://www.argoverse.org/data.html)
- [nuScenes](https://www.nuscenes.org)
- [Waymo Open Dataset](https://waymo.com/open/)
- [Lyft Level 5 AV Dataset 2019](https://level5.lyft.com/dataset/)
- [KAIST Urban Dataset](https://irap.kaist.ac.kr/dataset/)

## Tools
- [rgbd-dataset tool from TUM](https://vision.in.tum.de/data/datasets/rgbd-dataset/tools)
- [evo - evaluation tool for different trajectory formats](https://github.com/MichaelGrupp/evo)
- [VDO_SLAM - A Visual Object-aware Dynamic SLAM library](https://github.com/halajun/vdo_slam) 

## Projects

###### RGB (Monocular):

- [Kimera](https://github.com/MIT-SPARK/Kimera). Available on ROS
> A. Rosinol, M. Abate, Y. Chang, L. Carlone. Kimera: an Open-Source Library for Real-Time Metric-Semantic Localization and Mapping. arXiv preprint arXiv:1910.02490.

- [PTAM](https://github.com/Oxford-PTAM/PTAM-GPL)
> [1] Georg Klein and David Murray, "Parallel Tracking and Mapping for Small AR Workspaces", Proc. ISMAR 2007
> [2] Georg Klein and David Murray, "Improving the Agility of Keyframe-based SLAM", Proc. ECCV 2008


- [DSO](https://github.com/JakobEngel/dso_ros). Available on ROS
>Direct Sparse Odometry, J. Engel, V. Koltun, D. Cremers, In arXiv:1607.02565, 2016
>A Photometrically Calibrated Benchmark For Monocular Visual Odometry, J. Engel, V. Usenko, D. Cremers, In arXiv:1607.02555, 2016

- [LSD-SLAM](https://github.com/tum-vision/lsd_slam). Available on ROS
>LSD-SLAM: Large-Scale Direct Monocular SLAM, J. Engel, T. Schöps, D. Cremers, ECCV '14
>Semi-Dense Visual Odometry for a Monocular Camera, J. Engel, J. Sturm, D. Cremers, ICCV '13

- [ORB-SLAM](https://github.com/raulmur/ORB_SLAM). Available on ROS
> [1] Raúl Mur-Artal, J. M. M. Montiel and Juan D. Tardós. ORB-SLAM: A Versatile and Accurate Monocular SLAM System. IEEE > Transactions on Robotics, vol. 31, no. 5, pp. 1147-1163, 2015. (2015 IEEE Transactions on Robotics Best Paper Award). PDF.
> [2] Dorian Gálvez-López and Juan D. Tardós. Bags of Binary Words for Fast Place Recognition in Image Sequences. IEEE > Transactions on Robotics, vol. 28, no. 5, pp. 1188-1197, 2012. PDF.

- [Nister's Five Point Algorithm for Essential Matrix estimation, and FAST features, with a KLT tracker](https://github.com/avisingh599/mono-vo)
>D. Nister, “An efficient solution to the five-point relative pose problem,” Pattern Analysis and Machine Intelligence, IEEE Transactions on, vol. 26, no. 6, pp. 756–770, 2004.

- [SVO-SLAM](https://github.com/uzh-rpg/rpg_svo). Available on ROS
> Christian Forster, Matia Pizzoli, Davide Scaramuzza, "SVO: Fast Semi-direct Monocular Visual Odometry," IEEE International Conference on Robotics and Automation, 2014.

###### RGB and Depth (Called RGBD):
- [OpenCV RGBD-Odometry (Visual Odometry based RGB-D images)](https://github.com/tzutalin/OpenCV-RgbdOdometry)
> Real-Time Visual Odometry from Dense RGB-D Images, F. Steinbucker, J. Strum, D. Cremers, ICCV, 2011

- [Dense Visual SLAM for RGB-D Cameras](https://github.com/tum-vision/dvo_slam). Available on ROS
>[1]Dense Visual SLAM for RGB-D Cameras (C. Kerl, J. Sturm, D. Cremers), In Proc. of the Int. Conf. on Intelligent Robot Systems (IROS), 2013.
[2]Robust Odometry Estimation for RGB-D Cameras (C. Kerl, J. Sturm, D. Cremers), In Proc. of the IEEE Int. Conf. on Robotics and Automation (ICRA), 2013
[3]Real-Time Visual Odometry from Dense RGB-D Images (F. Steinbruecker, J. Sturm, D. Cremers), In Workshop on Live Dense Reconstruction with Moving Cameras at the Intl. Conf. on Computer Vision (ICCV), 2011.


- [RTAB MAP - Real-Time Appearance-Based Mapping](https://github.com/introlab/rtabmap). Available on ROS
> Online Global Loop Closure Detection for Large-Scale Multi-Session Graph-Based SLAM, 2014
> Appearance-Based Loop Closure Detection for Online Large-Scale and Long-Term Operation, 2013

- [ORB2-SLAM](https://github.com/raulmur/ORB_SLAM2). Available on ROS
> [1] Raúl Mur-Artal, J. M. M. Montiel and Juan D. Tardós. ORB-SLAM: A Versatile and Accurate Monocular SLAM System. IEEE > Transactions on Robotics, vol. 31, no. 5, pp. 1147-1163, 2015. (2015 IEEE Transactions on Robotics Best Paper Award).
> [2] Dorian Gálvez-López and Juan D. Tardós. Bags of Binary Words for Fast Place Recognition in Image Sequences. IEEE Transactions on Robotics, vol. 28, no. 5, pp. 1188-1197, 2012.

- [InfiniTAM∞ v2](http://www.robots.ox.ac.uk/~victor/infinitam/index.html)
> Kahler, O. and Prisacariu, V.~A. and Ren, C.~Y. and Sun, X. and Torr, P.~H.~S and Murray, D.~W. Very High Frame Rate Volumetric Integration of Depth Images on Mobile Device. IEEE Transactions on Visualization and Computer Graphics (Proceedings International Symposium on Mixed and Augmented Reality 2015

- [Kintinuous](https://github.com/mp3guy/Kintinuous)
> Real-time Large Scale Dense RGB-D SLAM with Volumetric Fusion, T. Whelan, M. Kaess, H. Johannsson, M.F. Fallon, J. J. Leonard and J.B. McDonald, IJRR '14

- [ElasticFusion](https://github.com/mp3guy/ElasticFusion)
> [1] ElasticFusion: Real-Time Dense SLAM and Light Source Estimation, T. Whelan, R. F. Salas-Moreno, B. Glocker, A. J. Davison and S. Leutenegger, IJRR '16
> [2] ElasticFusion: Dense SLAM Without A Pose Graph, T. Whelan, S. Leutenegger, R. F. Salas-Moreno, B. Glocker and A. J. Davison, RSS '15

- [Co-Fusion](http://visual.cs.ucl.ac.uk/pubs/cofusion/index.html)
> Martin Rünz and Lourdes Agapito. Co-Fusion: Real-time Segmentation, Tracking and Fusion of Multiple Objects. 2017 IEEE International Conference on Robotics and Automation (ICRA)

###### RGBD and LIDAR:
- [Google's cartographer](https://github.com/googlecartographer/cartographer). Available on ROS


## Other open source projects
[DynaSLAM](https://github.com/BertaBescos/DynaSLAM) A SLAM system robust in dynamic environments for monocular, stereo and RGB-D setups

[openvslam](https://github.com/xdspacelab/openvslam) A Versatile Visual SLAM Framework


## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
