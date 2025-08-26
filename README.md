# Echo Flow-induced Temporal Correlation Learning for Ultrasound Video Object Segmentation (EchoSAM2)

> **Authors:**
> [Dongfang Wang](),
> [Tao Zhou](https://taozh2017.github.io/)
> [Shangbing Gao](), and
> [Jian Yang](https://scholar.google.com/citations?user=6CIDtZQAAAAJ&hl=en), 



## 1. Preface

- This repository provides code for "_**Echo Flow-induced Temporal Correlation Learning for Ultrasound Video Object Segmentation (EchoSAM2)**_". 
([paper](https://doi.org/10.1109/TBME.2025.3594704))

## 2. Overview

### 2.1. Introduction

Objective: The segmentation of ultrasound video objects aims to delineate specific anatomical structures or area of injury in sequential ultrasound imaging data. Current methods exhibit promising results, but struggle with key aspects of ultrasound video analysis. They insufficiently capture inter-frame object motion, resulting in unsatisfactory segmentation for dynamic or low-contrast scenarios. With the release of SAM2, video object segmentation has advanced significantly. However, its performance in ultrasound videos remains suboptimal due to its design bias toward natural videos and lack of consideration for ultrasound-specific characteristics. We propose a novel EchoSAM2 method to achieve more accurate object segmentation in ultrasound videos. Methods: We propose Echo Flow, which captures motion trends between frames to enhance the modeling of temporal relationships. It also helps suppress interference from non-object regions by leveraging object motion patterns. Furthermore, we propose an Echo Modulation Block (EMB) to seamlessly incorporate Echo Flow into the SAM2 framework, improving the quality of feature representation. To further optimize SAM2’s performance during fine-tuning, we present a Gaussian Adapter specifically designed for ultrasound image characteristics. Results: Extensive experiments on three ultrasound video datasets confirm the effectiveness of our method, achieving state-of-the-art results. On the EUDP dataset, our model achieves a Dice of 85.49%, outperforming the second-best method by 3.19\%. Models trained on HMC-QU and CAMUS achieve the best generalization when tested on each other's unseen test sets. Conclusion: The introduction of Echo Flow, along with other supporting modules, enhances both segmentation accuracy and the generalizability of the model. Significance: Accurate segmentation of ultrasound video objects enhances diagnostic accuracy and consistency, thereby increasing overall clinical value.

### 2.2. Framework Overview

<p align="center">
    <img src="./Imgs/framework.svg"/> <br />
    <em> 
    Figure 1: Overview of the proposed EchoSAM2.
    </em>
</p>

## 3. Proposed Method
### Code coming soon!
<!-- ### 3.1. Training/Testing

The training and testing experiments are conducted using [PyTorch](https://github.com/pytorch/pytorch) with 
a single NVIDIA GeForce RTX 3090 with 24 GB of Memory.

> Note that our model also supports other GPUs, which means you can adjust the batch size.

1. Configuring your environment
    - Create conda environment: `conda create -n FINet python=3.8`
    - Activate environment：`conda activate FINet`
    - Install requirements: `pip install -r requirements.txt`

3. Downloading data
    - Download the ultrasound datasets [BUSI](https://scholar.cu.edu.eg/?q=afahmy/pages/dataset), [TN3K](https://github.com/haifangong/TRFE-Net-for-thyroid-nodule-segmentation), [TG3K](https://github.com/haifangong/TRFE-Net-for-thyroid-nodule-segmentation), and [MMOTU](https://github.com/cv516Buaa/MMOTU_DS2Net).
    - Edge maps can be referred to `./utils/edge.py`
4. Load the pre-trained parameters
    - Download the backbone checkpoint of FINet from the following [Google Drive](https://drive.google.com/file/d/1wlJEtRpn3ekdKRA_WP6tcYxREw6LNeto/view?usp=sharing) and move it into `./FINet/pretrained/`
6. Training Configuration
    - Assigning your costumed path, like `--dataset_root` and `--dataset_name` in `Train.py`
8. Testing Configuration
    - Assigning your costumed path, like `--pth_path` and `--test_save` in `Test.py` -->

## 4. Citation

Please cite our paper if you find the work useful: 

    @ARTICLE{11123471,
      author={Wang, Dongfang and Zhou, Tao and Gao, Shangbing and Yang, Jian},
      journal={IEEE Transactions on Biomedical Engineering}, 
      title={Echo Flow-Induced Temporal Correlation Learning for Ultrasound Video Object Segmentation}, 
      year={2025},
      pages={1-10},
      doi={10.1109/TBME.2025.3594704}}




## 5. License

The source code is free for research and educational use only. Any commercial use should get formal permission first.

