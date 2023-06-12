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

WASTE IMAGE RECOGNITION
Link Google Colab: https://colab.research.google.com/drive/1q6CrJMQdnEZgM_lyw4FgGJBHCNWOPMy_?usp=sharing

Link Google Drive DATASET.zip: https://drive.google.com/file/d/1LXjiQfwtL0ZUE93RMT_AeHlgul1I7MG0/view?usp=sharing
