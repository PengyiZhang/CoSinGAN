# Learning Diagnosis of COVID-19 from a Single Radiological Image

![](/CoSinGAN/figures/generation01.png)

## Abstract

Radiological image is currently adopted as the visual evidence for COVID-19 diagnosis in clinical. Using deep models to realize automated infection measurement and COVID-19 diagnosis is important for faster examination based on radiological imaging. Unfortunately, collecting large training data systematically in the early stage is difficult. To address this problem, we explore the feasibility of learning deep models for COVID-19 diagnosis from a single radiological image by resorting to synthesizing diverse radiological images. Specifically, we propose a novel conditional generative model, called CoSinGAN, which can be learned from a single radiological image with a given condition, i.e., the annotations of the lung and COVID- 19 infection. Our CoSinGAN is able to capture the conditional distribution of the lung and COVID-19 infection, and further synthesize diverse and high-resolution (512×512) radiological images that match the input conditions precisely. Both deep classification and segmentation networks trained on synthesized samples from CoSinGAN achieve notable detection accuracy of COVID-19 infection. Such results are significantly better than the counterparts trained on the same extremely small number of real samples (1 or 2 real samples) by using strong data augmentation, and approximate to the counterparts trained on large dataset (2846 real images). It confirms our method can significantly reduce the performance gap between deep models trained on extremely small dataset and on large dataset, and thus has the potential to realize learning COVID-19 diagnosis from few radiological images in the early stage of COVID- 19 pandemic. Our codes are made publicly available at https://github.com/PengyiZhang/CoSinGAN.

## [CoSinGAN](/CoSinGAN)

### Multi-scale architecture
![](/CoSinGAN/figures/multi-scale_architecture.png)

### Two-stage GAN

![](/CoSinGAN/figures/two-stage_GANa.png)
![](/CoSinGAN/figures/two-stage_GANb.png)

## [classification](/classification)


## [segmentation](/segmentation)


