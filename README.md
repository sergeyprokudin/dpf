# Dynamic Point Fields

### Towards Efficient and Scalable Dynamic Surface Representations

This is an official code for the paper ["Dynamic Point Fields" (ICCV 2023)](https://arxiv.org/abs/2304.02626). Please visit [the project page](https://sergeyprokudin.github.io/dpf/) for more details, or watch a [5-minute tutorial video](https://www.youtube.com/watch?v=i-9eAgS8HEA) covering the main ideas behind the approach.

**In a nutshell**: we propose to model dynamic surfaces with a _**point-based model**_, where the motion of a point over time is represented by an _**implicit deformation field**_. Working directly with points (rather than SDFs) allows us to easily incorporate various well-known deformation constraints, e.g. [as-isometric-as-possible (AIAP)](http://graphics.stanford.edu/~niloy/research/shape_space/shape_space_sig_07.html). We showcase the usefulness of this approach for creating animatable avatars in complex clothing.

## Colab Demos

| Description      | Link |
| ----------- | ----------- |
| Static Surface Reconstruction with Optimised CLouds| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github//sergeyprokudin/smplpix/blob/main/colab_notebooks/Convert_Video_to_SMPLpix_Dataset.ipynb)|
| Surface Deformation (with AIAP regularisation) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sergeyprokudin/smplpix/blob/main/colab_notebooks/SMPLpix_training.ipynb)|
| Single Scan Animation (ReSynth)| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sergeyprokudin/smplpix/blob/main/colab_notebooks/SMPLpix_training.ipynb)|
| Loading and Evaluating Original Paper Results (Sections 4.1-4.2) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sergeyprokudin/smplpix/blob/main/colab_notebooks/SMPLpix_training.ipynb)|


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