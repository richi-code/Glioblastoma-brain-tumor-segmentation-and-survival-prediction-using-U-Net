# Glioblastoma-brain-tumor-segmentation-and-survival-prediction-using-U-Net
Overview

1. Dataset
2. Pre-processing
3. Architecture
4. Training Process
5. Results
6. Usage

i. Dataset

The BraTS data set is used for training and evaluating the model. This dataset contains four modalities for each individual brain, namely, T1, T1c (post-contrast T1), T2, and Flair which were skull-stripped, resampled and coregistered. For more information, please refer to the main site.

ii. Pre-processing

For pre-processing the data, firstly, N4ITK algorithm is adopted on each MRI modalities to correct the inhomogeneity of these images. Secondly, 1% of the top and bottom intensities is removed, and then each modality is normalized to zero mean and unit variance.
