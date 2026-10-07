# Adversarial Attacks on Semantic Segmentation

Adversarial attacks on pretrained semantic segmentation models (PyTorch, torchvision) and a study of their transferability across architectures, on images from MS-COCO.

ENSTA Paris, MI201 course project (2024), supervised by Pol Labarbarie and Adrien Chan-Hon-Tong.
Authors: Cedric Darel Dada Simeu and Cedrick Tchakonte Tchiegue.

## What is in the notebook

1. **Untargeted attack**: perturbs intermediate features to break the segmentation.
2. **Targeted attack (FGSM)**: forces DeepLabV3-ResNet50 to predict a chosen class (person, cat, dog) everywhere.
3. **Effect of the L∞ budget ε**: trade-off between how visible the noise is and how effective the attack is.
4. **Transferability**: the perturbation is tested on a model it was not computed on (DeepLabV3-MobileNetV3).
5. **Multi-model attack**: a perturbation optimized jointly on DeepLabV3-ResNet50 and FCN-ResNet50, then evaluated on DeepLabV3-ResNet50, FCN-ResNet50 and DeepLabV3-MobileNetV3.

## Files

- `DADA_TCHAKONTE_Projet1.ipynb`: code, results and explanations (French). It can be opened in Google Colab.
- `DADA_TCHAKONTE_Projet1.pdf`: the report.
- `coco_sample.pth`: the MS-COCO sample used in the experiments.

Originally published at [CedricDada/attack_segmentation](https://github.com/CedricDada/attack_segmentation).
