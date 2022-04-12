## Introduction
In this repository, you will find the source code of all the scripts developed for the experimental phase of the paper &quot;**Artificial intelligence-based banana ripeness detection**&quot;.

## Content
- ** 1. Image Preprocessing**
In this file, you will find the procedures carried out for the preprocessing of the images, which were: Data Augmentation for unbalanced data, NLM Filter for Image Denoising and Rembg tool for background removal.

- ** 2. Color Features**
The extraction of the color features from the images was performed by converting to HSV (Hue, Saturation, Value) color space to calculate the histogram representing the color distribution of an image. The information generated in this file is located in the Features_Data/Color_Features folder.

- ** 3. Textural Features**
The extraction of textural features from the images was performed through the gray level co-occurrence matrices (GLCMs) technique. The information generated in this file is located in the Features_Data/Textural_Features folder.

- ** 4. First Experiment**
In this experiment, the concatenated color and textural features obtained from the images above were used. These features were employed to feed the models that implemented the Multiclass SVM techniques based on OVO classification (VBMSVM, DAGMSVM) and Random Forest.

- ** 5. Second Experiment**
For the second experiment, the concatenated color and textural features were used, applying the PCA dimensionality reduction technique. The methods that were implemented in this experiment are Multiclass SVM based on OVO classification (VBMSVM, DAGMSVM) and Random Forest.

- ** 6. Third Experiment**
In the third experiment, the implementation of the CNN-based TL deep learning technique was performed.

## Principal Libraries
- OpenCV
- Tensorflow
- Rembg
- Keras
