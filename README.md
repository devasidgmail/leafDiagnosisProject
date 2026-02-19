### Plant Leaf Disease Identification

Feb/18/2026  
Prelimenary Report . There is more to be done. 


This project implements a high-accuracy computer vision pipeline using TensorFlow/Keras to  
identify 38 classes of plant diseases from the PlantVillage dataset.  


  Preprocessing Pipeline <br>
  Data Split: Partitioned into Training (70%), Validation (15%), and Test (15%). <br>
  Augmentation: Applied RandomResizedCrop and HorizontalFlip to increase model robustness.<br>
  Normalization: Standardized images using ImageNet mean/std statistics. <br> 
   
   

   Model Architecture & Training  <br>
   I utilized Transfer Learning with the ResNet50 architecture in two distinct phases.  <br>

   
   Phase 1 Feature Extraction  <br>
   Base model weights frozen; only custom Dense and Dropout layers trained.  <br>
   Accuracy: ~97.8% (Val).  <br>

   Phase 2 Fine-Tuning  <br>
   Unfroze the top 30 layers and re-trained with a lower learning rate  <br>
   Accuracy: ~99.1% .  <br>


   Results so far.   <br>
   The model achieved a Test Accuracy of 99.25%.  <br>

   Link to Google Colab Notebooks.  <br>
   
   PreProcessing  <br>
   https://colab.research.google.com/drive/1AcfjIR24M1xhrg_bjjfrYb0TyzNbb8Iv?usp=drive_link
   
   Training  <br>
   https://colab.research.google.com/drive/1r09XhsShPOnnQVfskbtl08Rh7XEg7PLm?usp=drive_link
