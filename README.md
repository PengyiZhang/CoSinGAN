# CoSinGAN: Learning COVID-19 Infection Segmentation from a Single Radiological Image

![](/CoSinGAN/figures/generation01.png)

## Abstract

Computed tomography (CT) images are currently adopted as the visual evidence for COVID-19 diagnosis in clinical practice. Automated detection of COVID-19 infection from CT images based on deep models is important for faster examination. Unfortunately, collecting large-scale training data systematically in the early stage is difficult. To address this problem, we explore the feasibility of learning deep models for lung and COVID-19 infection segmentation from a single radiological image by resorting to synthesizing diverse radiological images. Specifically, we propose a novel conditional generative model, called CoSinGAN, which can be learned from a single radiological image with a given condition, i.e., the annotation mask of the lungs and infected regions. Our CoSinGAN is able to capture the conditional distribution of the single radiological image, and further synthesize high-resolution (512×512) and diverse radiological images that match the input conditions precisely. We evaluate the efficacy of CoSinGAN in learning lung and infection segmentation from very few radiological images by performing 5-fold cross validation on COVID-19-CT-Seg dataset (20 CT cases) and independent testing on MosMed dataset (50 CT cases). Both 2D U-Net and 3D U-Net, learned from 4 CT slices by using our CoSinGAN, have achieved notable infection segmentation performance, surpassing the COVID-19-CT-Seg-Benchmark, i.e., the counterparts trained on an average of 704 CT slices, by a large margin. Such results strongly confirm that our method has the potential to learn COVID-19 infection segmentation from few radiological images in the early stage of COVID-19 pandemic. Our codes will be made publicly available at https://github.com/PengyiZhang/CoSinGAN.

## [CoSinGAN](/CoSinGAN)

### Multi-scale architecture
![](/CoSinGAN/figures/multi-scale_architecture.png)

### Two-stage GAN

![](/CoSinGAN/figures/two-stage_GANa.png)
![](/CoSinGAN/figures/two-stage_GANb.png)

## [segmentation](/segmentation)



--------

We use [COVID-19-CT-Seg dataset](https://zenodo.org/record/3757476#.XvR5DPgzZPY) with 20 CT cases for 5-fold cross validation (4 cases for training and 16 cases for testing) and [MosMed dataset](https://mosmed.ai/datasets/covid19_1110) with 50 CT cases for independent test.


-------------

If you find it useful, please cite:

    @misc{zhang2020learning,
        title={Learning Diagnosis of COVID-19 from a Single Radiological Image},
        author={Pengyi Zhang and Yunxin Zhong and Xiaoying Tang and Yunlin Deng and Xiaoqiong Li},
        year={2020},
        eprint={2006.12220},
        archivePrefix={arXiv},
        primaryClass={eess.IV}
    }

-------------

## Acknowledgement

We thank the providers of [COVID-19-CT-Seg dataset](https://zenodo.org/record/3757476#.XvR5DPgzZPY) and [MosMed dataset](https://mosmed.ai/datasets/covid19_1110).
