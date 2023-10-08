# Dynamic Point Fields (ICCV 2023)

### Towards Efficient and Scalable Dynamic Surface Representations

### [Project Page](https://sergeyprokudin.github.io/dpf/) | [Paper](https://arxiv.org/abs/2304.02626) | [Video](https://www.youtube.com/watch?v=i-9eAgS8HEA)

[![Open Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github//sergeyprokudin/dpf/blob/main/colab_notebooks/Single_Scan_Animation.ipynb)<br> 

This is an official code for the paper "Dynamic Point Fields" (ICCV 2023 Oral).

![figure1_cropped](https://github.com/sergeyprokudin/dpf/assets/8117267/9fb279d9-b518-4cc7-82e6-3ccfd4bee48c)

**In a nutshell**: we propose to model dynamic surfaces with a _**point-based model**_, where the motion of a point over time is represented by an _**implicit deformation field**_. Working directly with points (rather than SDFs) allows us to easily incorporate various well-known deformation constraints, e.g. [as-isometric-as-possible (AIAP)](http://graphics.stanford.edu/~niloy/research/shape_space/shape_space_sig_07.html). We showcase the usefulness of this approach for creating animatable avatars in complex clothing:


https://github.com/sergeyprokudin/dpf/assets/8117267/804b0778-dd21-4573-99de-440da766dc4f


Please see Section 4.3 of the paper for more details.

## Colab Demos

We release our code as a bundle of Colab notebooks covering the main experiments and applications discussed in the paper.

| Description      | Link |
| ----------- | ----------- |
| Static Surface Reconstruction with Optimised Clouds| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github//sergeyprokudin/dpf/blob/main/colab_notebooks/Static_Surface_Reconstruction_with_Optimised_Clouds.ipynb)|
| Learning Surface Deformations | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github//sergeyprokudin/dpf/blob/main/colab_notebooks/Learning_Surface_Deformations.ipynb)|
| Single Scan Avatar Animation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github//sergeyprokudin/dpf/blob/main/colab_notebooks/Single_Scan_Animation.ipynb)|
| Loading and Evaluating Original Paper Results (Sections 4.1, Table 1) | TBD |
| Loading and Evaluating Original Paper Results (Sections 4.2, Table 2) | TBD |

## Point-based surface representations [&#128279; code](https://colab.research.google.com/github//sergeyprokudin/dpf/blob/main/colab_notebooks/Static_Surface_Reconstruction_with_Optimised_Clouds.ipynb)

We begin this work by revisiting point clouds as surface modeling primitives, and demonstrate how surfaces of arbitrary complexity can be efficiently modeled as sets of 3D points with associated features, such as normal directions:

![image](https://github.com/sergeyprokudin/dpf/assets/8117267/07d75b51-90cb-47f8-ba09-96338bbfa05a)

Compared to the state-of-the-art implicit models for 3D surface representations ([NGLOD](https://nv-tlabs.github.io/nglod/), [NGP](https://nvlabs.github.io/instant-ngp/), optimised point cloud model offers better reconstruction quality on all metrics, while taking zero inference time thanks to its explicit nature:

![image](https://github.com/sergeyprokudin/dpf/assets/8117267/da4ab24d-37c7-4462-9b79-9b67f50c6eb1)


## Citation

If you find our work useful in your research, please consider citing:

```
@article{prokudin2023dynamic,
                  title={Dynamic Point Fields},
                  author={Prokudin, Sergey and Ma, Qianli and Raafat, Maxime and Valentin, Julien and Tang, Siyu},
                  journal={arXiv preprint arXiv:2304.02626},
                  year={2023}
                }
```

## License

See the [LICENSE](https://github.com/sergeyprokudin/dpf/blob/main/LICENSE) file.
