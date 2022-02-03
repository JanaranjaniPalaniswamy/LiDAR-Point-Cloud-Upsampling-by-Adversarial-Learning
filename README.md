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

```
![workflow](https://github.com/JanaranjaniPalaniswamy/LiDAR-Point-Cloud-Upsampling-by-Adversarial-Learning/blob/main/sample_results/workflow.png?raw=true "Work Flow")

![pu-net](https://github.com/JanaranjaniPalaniswamy/LiDAR-Point-Cloud-Upsampling-by-Adversarial-Learning/blob/main/sample_results/PU-net.png?raw=true "PU-Net Results")

![pu-gan](https://github.com/JanaranjaniPalaniswamy/LiDAR-Point-Cloud-Upsampling-by-Adversarial-Learning/blob/main/sample_results/pu-gan.png?raw=true "PU-GAN Results")

![dgml](https://github.com/JanaranjaniPalaniswamy/LiDAR-Point-Cloud-Upsampling-by-Adversarial-Learning/blob/main/sample_results/dgml.png?raw=true "DGML-VAE Results")

![lhrcnn](https://github.com/JanaranjaniPalaniswamy/LiDAR-Point-Cloud-Upsampling-by-Adversarial-Learning/blob/main/sample_results/lhrcnn.png?raw=true "LHRCNN Results")

![unet](https://github.com/JanaranjaniPalaniswamy/LiDAR-Point-Cloud-Upsampling-by-Adversarial-Learning/blob/main/sample_results/u-net.png?raw=true "U-Net Results")

![lsrgan](https://github.com/JanaranjaniPalaniswamy/LiDAR-Point-Cloud-Upsampling-by-Adversarial-Learning/blob/main/sample_results/LSRGAN.png?raw=true "LSRGAN Results")
```

## Quantitative Results

Point cloud based architectures are evaluated using EMD and CD metrics.
Range image based architectures are evaluated using EMD, CD and PSNR metrics.

```
![Alt text](sample_results/metric.png?raw=true "Range Image based architecture")

![Alt text](sample_results/metric_pc.png?raw=true "Point Cloud based architecture")
```
