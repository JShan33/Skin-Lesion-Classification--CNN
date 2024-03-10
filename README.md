# Skin-Lesion-Classification--CNN
Skin Lesion Classification based on Convolutional Neural Network,using the Skin Cancer dataset by the International Skin Imaging Collaboration (ISIC).

In this experiment, the dataset which contains 10015 images containing 7 different skin lesion types is used, to train classifier models based on convolutional neural networks.
It should be noted that there is an obvious uneven distribution between the classes of the dataset,for example,there are 6705 data points in the class of 'Melanocytic nevi', but 115 data points in the class of 'Dermatofibroma'.
No doubt this will make model training more difficult and negatively impact the metrics of performance evaluation.  To address this situation, we adopt the following tuning strategies for the baseline model to improve its performance:
● Changing the hyperparameters
● Data Augmentation
● Category balancing strategies
● Transfer Learning.
I would like to make a note on the choice of metrics.After searching the literature，we found that accuracy is not always a good
metric,especially in multi-class classification with an imbalanced dataset. Accuracy is only a reasonable measure if the different classes in the dataset are approximately equally distributed. Accuracy is calculated by (TP + TN)/(TP + TN + FP + FN). It specifies the percentage of objects that have been correctly classified.The dataset we used has uneven distribution, so except accuracy, we also put a lot of focus on macro-F1 scores (unweighted mean of F1 scores).
Finally ,the difference between the performance of baseline model and the performance of tuned models as follows(PS:The chart is sorted in descending order by macro F1)

# Dataset
The dataset is available online and can be downloaded from:
https://challenge.isic-archive.com/data/#2018.
This dataset has many versions between 2016-2020. We used only the training data from 2018. This dataset is entitled as ’Training data’ under the section 2018 (10015 images (2.6 GB of size) and 1 ground truth response CSV file containing 1 header row and 10015 corresponding response rows). 

