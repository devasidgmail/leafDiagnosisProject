Plant Leaf Disease Identification

Feb/18/2026 
Prelimenary Report . There is more to be done. 


This project implements a high-accuracy computer vision pipeline using TensorFlow/Keras to 
identify 38 classes of plant diseases from the PlantVillage dataset.

1. Preprocessing Pipeline

   Data Split: Partitioned into Training (70%), Validation (15%), and Test (15%).
   Augmentation: Applied RandomResizedCrop and HorizontalFlip to increase model robustness.
   Normalization: Standardized images using ImageNet mean/std statistics.

2. Model Architecture & Training
   I utilized Transfer Learning with the ResNet50 architecture in two distinct phases.
   Phase 1 Feature Extraction
   Base model weights frozen; only custom Dense and Dropout layers trained.
   Accuracy: ~97.8% (Val).

   Phase 2 Fine-Tuning
   Unfroze the top 30 layers and re-trained with a lower learning rate.
   Accuracy: ~99.1% (Val).

3. Results so far.
   The model achieved a final Test Accuracy of 99.25%.

4. Link to Google Colab Notebooks.
   
   PreProcessing 
   https://colab.research.google.com/drive/1AcfjIR24M1xhrg_bjjfrYb0TyzNbb8Iv?usp=drive_link
   
   Training 
   https://colab.research.google.com/drive/1r09XhsShPOnnQVfskbtl08Rh7XEg7PLm?usp=drive_link
