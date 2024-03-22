# CNN-Architectures-on-Breast-Ultrasound-Images-Dataset
Comparative analysis of CNN architectures on Breast Ultrasound Images Dataset. Explored 9 CNN models for classifying images into normal, benign, malignant categories. MobileNet and Inception-ResNet-V2 emerged as top performers with 83% and 80% accuracy, respectively. Insights aid in early breast cancer detection.

## Introduction

We utilized a publicly available dataset, "Dataset of breast ultrasound images," for this study. This dataset comprises breast ultrasound images from 600 female patients aged 25 to 75, categorized into normal, benign, and malignant classes. The dataset consists of 780 images with an average resolution of 500 × 500 pixels. Our objective was to explore the efficacy of various convolutional neural network (CNN) architectures for classifying these ultrasound images into the aforementioned categories.

## Dataset Characteristics

- **Subjects**: 600 female patients aged 25 to 75.
- **Image Categories**: Normal (2), Benign (0), Malignant (1).
- **Image Count**: 780 images (Benign: 487, Malignant: 210, Normal: 133).
- **Image Resolution**: Average size of 500 × 500 pixels.
- **Data Collection**: Images collected using LOGIQ E9 and LOGIQ E9 Agile ultrasound systems.
- **Preprocessing**: Removed duplicates, corrected annotations, and converted DICOM to PNG.
- **Ground Truth Annotation**: Accurate delineation of image boundaries.
![alt text](https://github.com/aparnabg/CNN-Architectures-on-Breast-Ultrasound-Images-Dataset/blob/main/breast%20cancer%20data%20images/daat%20distribution.png?raw=true)
![alt text](https://github.com/aparnabg/CNN-Architectures-on-Breast-Ultrasound-Images-Dataset/blob/main/breast%20cancer%20data%20images/data%20after%20augmentation.png?raw=true)
## Data Augmentation

To address class imbalance, we employed data augmentation techniques including rotation, shifting, zooming, shearing, and flipping. This approach generated additional samples, balancing the dataset and enhancing model robustness.

## Implemented CNN Architectures

We implemented the following CNN architectures:
- EfficientNet
- Inception-ResNet-V2
- ResNet50
- MobileNet
- VGG16
- Depth-based CNN
- AlexNet
- VGG19
- PolyNet

## Results and Conclusion

The accuracy of the implemented models ranged from 15% to 83%. 

### Top Performers:
- **MobileNet**: 83% accuracy. Efficient feature extraction due to its lightweight architecture.
- **Inception-ResNet-V2**: 80% accuracy. Impressive due to its innovative combination of Inception and ResNet architectures.

### Other Observations:
- **VGG16 and VGG19**: Achieved high accuracies but exhibited higher losses, suggesting potential overfitting.
- **Depth-based CNN and AlexNet**: Showed lower accuracies.
- **PolyNet**: Encountered difficulty learning discriminative features.
- **EfficientNet**: Relatively low accuracy but suitable for resource-constrained environments due to its efficiency.

### Conclusion

Choosing the right CNN architecture is crucial for accurately classifying breast ultrasound images. While some models excel in efficiency or feature extraction, others may struggle with overfitting. Fine-tuning strategies could further enhance performance, aiding early detection strategies for breast cancer and improving healthcare outcomes.

