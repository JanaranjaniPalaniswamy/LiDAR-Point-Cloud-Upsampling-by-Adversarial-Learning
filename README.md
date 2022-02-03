# Lidar Point Cloud Up-sampling using GAN

In this work I built a framework called Lidar Super-Resolution GAN (LSRGAN) a GAN-based network with geometric losses to upsample the LiDAR point clouds.
Achieved the goal of obtaining a dense up-sampled point cloud that retains the LiDAR lines structure. This is widely regarded as the first step of LiDAR processing
and scene understanding and has shown to contribute in improving the efficiency in many applications such as: object detection, semantic segmentation, and localization and mapping.

## Datasets

KITTI and Nuscenes datasets were used for training

## Baseline Models
Five different models that work on point clouds are choosed as baselines.

### Point Cloud based Architectures
```
- PU-Net
- PU-GAN
- Deep Generative Model- VAE (DGML-VAE)
```
### Range Image based Architectures
```
- CNN-based High-Resolution LiDAR Synthesis (LHRCNN)
- U-Net
```

## Sample Results
All the baseline models are compared using the output point cloud data and range images depending on the architecture.

### <p align="center"> Work Flow </p>
<p align="center"> <img src="sample_results/workflow.png" width="40%" /> </p>

### <p align="center"> PU-Net Results </p>
<p align="center"> <img src="sample_results/PU-net.png" width="70%" /> </p>

### <p align="center"> PU-GAN Results </p>
<p align="center"> <img src="sample_results/pu-gan.png" width="70%" /> </p>

### <p align="center"> DGML-VAE Results </p>
<p align="center"> <img src="sample_results/dgml.png" width="70%" /> </p>

### <p align="center"> LHRCNN Results </p>
<p align="center"> <img src="sample_results/lhrcnn.png" width="70%" /> </p>

### <p align="center"> U-Net Results </p>
<p align="center"> <img src="sample_results/u-net.png" width="70%" /> </p>

### <p align="center"> LSRGAN Results </p>
<p align="center"> <img src="sample_results/LSRGAN.png" width="70%" /> </p>


## Quantitative Results

Point cloud based architectures are evaluated using EMD and CD metrics.
Range image based architectures are evaluated using EMD, CD and PSNR metrics.

### <p align="center"> Point Cloud based architecture </p>
<p align="center"> <img src="sample_results/metric_pc.png" width="40%" /> </p>

### <p align="center"> Range Image based architecture </p>
<p align="center"> <img src="sample_results/metric.png" width="40%" /> </p>


