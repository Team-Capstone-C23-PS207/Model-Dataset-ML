# Machine Learning

## Data Specification

The dataset is from [Drinking Waste ClassificationStructureRSMAS](https://www.kaggle.com/datasets/arkadiyhacks/drinking-waste-classification) that contains 4828 images separated by class and has 4 classes. But because the scope of this application is not very large, our team focuses on 3 classes (AluCan, Glass, and PET). We also decided to add one more class (Unknown) that contains 3 classes (Cardboard, Paper, Trash) from the dataset [Trashnet](https://github.com/garythung/trashnet). For our baseline and transfer learning model, we generate more images using data augmentation.
<br>
<br>

<div>
  <img src="https://github.com/Team-Capstone-C23-PS207/Model-Dataset-ML/blob/main/DATASET/TRAIN/AluCan/AluCan1%2C000.jpg" alt="AluCan1,000" width="256" height="256" style="display: inline-block;">
  <img src="https://github.com/Team-Capstone-C23-PS207/Model-Dataset-ML/blob/main/DATASET/TRAIN/Glass/Glass1%2C001.JPG" alt="Glass1,001" width="256" height="256" style="display: inline-block;">
  <img src="https://github.com/Team-Capstone-C23-PS207/Model-Dataset-ML/blob/main/DATASET/TRAIN/PET/PET1%2C000.jpg" alt="PET1,000" width="256" height="256" style="display: inline-block;">
</div>
<div>
  <img src="https://github.com/Team-Capstone-C23-PS207/Model-Dataset-ML/blob/main/DATASET/TRAIN/Unknown/cardboard384.jpg" alt="cardboard384" width="256" height="256" style="display: inline-block;">
  <img src="https://github.com/Team-Capstone-C23-PS207/Model-Dataset-ML/blob/main/DATASET/TRAIN/Unknown/paper188.jpg" alt="paper188" width="256" height="256" style="display: inline-block;">
  <img src="https://github.com/Team-Capstone-C23-PS207/Model-Dataset-ML/blob/main/DATASET/TRAIN/Unknown/trash50.jpg" alt="trash50" width="256" height="256" style="display: inline-block;">
</div>

## The Approach

In machine learning, we try three different scenarios for training models: baseline from CNN Coursera, transfer learning InceptionV3, and transfer learning Xception.
<br>
<br>
![Flow Diagram](https://user-images.githubusercontent.com/86770916/245032535-3efc4990-a892-4723-85a1-7f3d35cdc972.png)

And here’s the result of each model:
Algorithm | Loss | Accuracy | Val_Loss | Val_Accuracy
------------ | ------------ | ------------- | ------------- | -------------
Baseline CNN Coursera | 0.40 | 0.62 | 0.41 | 0.65
Transfer Learning InceptionV3 | 0.28 | 0.89 | 0.35 | 0.77
Transfer Learning Xception | **0.27** | **0.90** | **0.24** | **0.91**

The loss, accuracy, val_loss, and val_accuracy on the baseline model are really low and the transfer learning InceptionV3 has increased significantly but there are still fluctuations in val_loss and val_accuracy. Then with transfer learning Xception, we achieved 81% on precision, recall, and F-1 score and we think this is adequate for our model to run smoothly.

## References

- [Transfer Learning](https://www.coursera.org/learn/convolutional-neural-networks-tensorflow/home/week/3)
- [Converting Models to JSON Format](https://www.coursera.org/learn/browser-based-models-tensorflow/home/week/3)
- [InceptionV3](https://keras.io/api/applications/inceptionv3/)
- [Xception](https://keras.io/api/applications/xception/)

---

## Link Documentation

WASTE IMAGE RECOGNITION
Link Google Colab: https://colab.research.google.com/drive/1q6CrJMQdnEZgM_lyw4FgGJBHCNWOPMy_?usp=sharing

Link Google Drive DATASET.zip: https://drive.google.com/file/d/1xdWEBp1_R2zeJXl0CDTeiWewphRPEcqU/view?usp=sharing
