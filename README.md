# Alzheimer's MRI Classification using ResNet 

This project explores the use of a pretrained ResNet34 model to classify different stages of Alzheimer's Disease from MRI brain scans. It includes both multiclass and binary classification tasks, with experiments comparing augmented and original datasets. 

# Dataset:

The dataset comprises both augmented and original MRI brain scans, categorized into four diagnostic groups: **Non-Demented, Very Mildly Demented, Mildly Demented,** and **Moderately Demented.** The data is organized in the ImageFolder format. I used PyTorch to train and evaluate the models on the MRI dataset.

# Experiments:

<img width="702" alt="Image" src="https://github.com/user-attachments/assets/4e013f4a-6956-4793-9902-19fce2cced0e" />

I focused on "Non-Demented" and "Very Mildly Demented" categories for the binary classification task, as distinguishing between healthy individuals and those in the earliest stage of cognitive decline is particularly valuable. Timely intervention can significantly slow progress of Alzheimer's Disease. 

In the later experiments, I trained the model on the augmented data and validated it on the original data. This was done to test how well the model generalizes to real, unaltered MRI scans. Augmentation helps increase data diversity during training, while using original images for validation ensures that performance is measured on realistic, clinically relevant inputs.

# Results:

<img width="696" alt="Image" src="https://github.com/user-attachments/assets/4685a192-0231-472c-a926-773a20edc560" />

While the **full dataset multiclass model** achieved the **highest validation accuracy** overall, the **binary classification model trained on augmented data** generalized best to original scans suggesting that early detection tasks benefit most from augmentation.

## Tech Stack:

- `torch`
- `torchvision`
- `pandas`
- `matplotlib`


