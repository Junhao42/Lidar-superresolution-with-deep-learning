This repository houses the code and resources for my final degree project, which focuses on enhancing Lidar sensor resolution through deep learning techniques in an image superresolution approach.

The data used for this project has been obtained from **The KITTI Vision Benchmark Suite** and a new dataset from **Escuela Técnica Superior de Ingeniería de Sistemas Informáticos (ETSISI)** specifically made for this project, which will be publicly available for future works.

- KITTI data can be found through the following link:
  ```
  https://www.cvlibs.net/datasets/kitti/index.php
  ```

- ETSISI data can be found through the following link:
  ```
  in process
  ```

## Project description
In this project we propose to explore the posibility of applying superresolution techniques to LiDAR data with the purpose of simulating higher quality sensors by artifitially adding pointcloud channels with deep learning. Different aproaches may be taken to process pointcloud data, in this case an image projection of the 3 dimensional space will be applied, turning this problem into a more developed image superresolution field.
<p align="center">
<img src="https://github.com/Junhao42/Lidar-resolution-enhancement-with-machine-learning/blob/main/images/rotonda_etsisi.png" height="250" width="500">
</p>
State of the art neural network architectures will be studied, and the results of autoencoder and U-Net models will be compared with classical superresolution methods such as pointcloud interpolation. Furthermore, in order to achieve these goals we will assess how to visualize LiDAR pointclouds in a 2D image and the methodolody applied for a proper layer reduction of the data to simulate sensors with a lower quality.

<p align="center">
  <img src="https://github.com/Junhao42/Lidar-resolution-enhancement-with-machine-learning/blob/main/images/comparison3.png" height="250" width="900">
</p>

<p align="center">
  <img src="https://github.com/Junhao42/Lidar-resolution-enhancement-with-machine-learning/blob/main/images/comparison_kitti.png" height="250" width="900">
</p>

The obtained results show that a successful quality increase can be achieved with up to 32 point cloud channels in an image representation. U-Net architectures are well suited for superresolution purposes and display better results than classical models but may require significant computational resources to obtain a sharp image.


## Folders
The ```data``` folder contains examples of point cloud data and images from the ETSISI dataset. Due to copyright related issues, KITTI data should not be uploaded outside of its official domain, in order to use its data it is advised to visit KITTIs official website.

The ```notebook``` folder contains the code used in this project. They are divided in .ipynb notebooks and each one of them is dedicated to a specific process, but may share common functions for extracting, reading and managing LiDAR data.

The notebooks are divided by:
- 3D to image proyection
- Image data preprocessing for deep learning models
- point cloud channels reduction
- Last iterations for deep learning models applied to KITTI data
- Last iterations for deep learning models applied to ETSISI data

A copy of the project memory is also provided as a .pdf file ```"Superresolución_en_Sensores_LiDAR__Un_enfoque_desde_el_deep_learning"```

## References

To cite this project, you can use the following BibText entry:

```latex
@mastersthesis{citekey,
title = {Superresolución en Sensores LiDAR: Un enfoque desde el deep learning},
author = {Ge-Yang, J. y Díaz-Álvarez, A. y Sánchez-Gutierrez-Cabello, G.},
school = {E.T.S. de Ingeniería de Sistemas Informáticos , Universidad Politécnica
de Madrid},
year = {2024},
month = {7},
type = {Proyecto Fin de Grado}
}
```




