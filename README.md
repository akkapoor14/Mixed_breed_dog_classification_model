For my Princeton Junior Project, I created the first public mixed breed dog dataset, and first mixed breed dog classification model. 

My approach: 
1. First, I created my own dataset
(https://www.kaggle.com/datasets/anjalikapoor14/mixed-breed-dog-dataset) consisting of
images of mixed breed dogs and their genetic breed breakdown; as there is no existing
public dataset of mixed breed dogs, I collected this data through a public Facebook group
where people have posted their dogs’ genetic breed breakdown results from Wisdom Panel.

2. Then, I utilized transfer learning to build on the Xception model to create a purebred
classification model and trained this model on the Stanford Dog Dataset.
(https://www.kaggle.com/datasets/jessicali9530/stanford-dogs-dataset) I evaluated how the
model performed at classifying mixed breed dogs at this step.

3. Finally, I fine-tuned the model on mixed breed dog data, and reevaluated its performance.

(The main reason for my approach is that the mixed breed dog dataset is currently only 100
images - in comparison, the Stanford Purebred Dog Dataset is 20,000 photos, and the
Xception model was trained on over a million images in the ImageNet database. The mixed
breed dog dataset is far too small to train a model specifically for the task of mixed breed dog
classification, especially when there are 339 dog breeds in the world, and thus approximately
2 possible combinations of mixed breed dogs. Thus, my approach tries to leverage these 339
larger datasets to help train our model for the ultimate task of classifying mixed breed dogs.)

Results: 
Prior to fine-tuning, the model was able to predict the top breed of a mixed breed dog 9.3% of the time, while after fine-tuning, the model was able to 
predict the top breed 29.2% of the time. The results would suggest that the
two classification tasks are quite different and that there is a need for a larger mixed breed dog
dataset to truly test whether a machine learning model can be used to classify mixed breed dogs.

Read my entire paper here: https://drive.google.com/file/d/1qX3NQBPTcbQwuKA_Mu8rmGB36o8y7zrO/view?usp=sharing
