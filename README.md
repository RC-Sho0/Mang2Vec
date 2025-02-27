# Mang2Vec: Vectorization of Raster Manga by Primitive-based Deep Reinforcement Learning
A PyTorch implementation of "***Vectorization of Raster Manga by Deep Reinforcement Learning***".
 If the paper or code is useful for your research, please cite
```
 @article{su2023marvel,
  title={MARVEL: Raster Gray-level Manga Vectorization via Primitive-wise Deep Reinforcement Learning},
  author={Su, Hao and Liu, Xuefeng and Niu, Jianwei and Cui, Jiahe and Wan, Ji and Wu, Xinghao and Wang, Nana},
  journal={IEEE Transactions on Circuits and Systems for Video Technology},
  year={2023},
  publisher={IEEE}
}
```
or
```
@article{su2021vectorization,
  title={Vectorization of Raster Manga by Deep Reinforcement Learning},
  author={Su, Hao and Niu, Jianwei and Liu, Xuefeng and Cui, Jiahe and Wan, Ji},
  journal={arXiv preprint arXiv:2110.04830},
  year={2021}
}
```

<div align=center><img src="https://github.com/SwordHolderSH/Mang2Vec/blob/main/image/main.jpg" width="1000" /></div>

## Demos

<div align=center><img src="https://github.com/SwordHolderSH/Mang2Vec/blob/main/image/demo1.jpg" width="1000" /></div>
<div align=center><img src="https://github.com/SwordHolderSH/Mang2Vec/blob/main/image/demo2.jpg" width="1000" /></div>
<div align=center><img src="https://github.com/SwordHolderSH/Mang2Vec/blob/main/image/demo3.jpg" width="1000" /></div>


## Prerequisites
 
 * Linux or Windows
 * CPU or NVIDIA GPU + CUDA CuDNN
 * Python 3
 * Pytorch 1.7.0

## Getting Started

### Installation

* Clone this repo:
```
    git clone https://github.com/SwordHolderSH/Mang2Vec.git
    cd Mang2Vec
```
* Install PyTorch and other dependencies.
* Download ```actor.pkl``` from [Google Drive](https://drive.google.com/file/d/1NFyUiP0FcJ6HxK3eB2w2yPmQoz2xeNFN/view?usp=share_link) to path ```'./model/'```.

### Quick Start
* Get detailed information about all parameters using
```
    python main.py -h
```
* Generate your customized vectorized mangas:
```
    python main.py --img=./image/Naruto.png --actor=./model/actor.pkl  --max_step=40 --divide=32
```
## Acknowledge

Thanks for the reference codes of [ICCV2019-LearningToPaint](https://github.com/megvii-research/ICCV2019-LearningToPaint).
