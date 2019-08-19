# Predicting Pneumonia Using Deep Learning

I used the following dataset from kaggle.com to train, validate and test my model. 
https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia

## Model 
* Developed a feed forward classifier on top of Densenet161 and trained the classifier and Denselayer4 to acheive an accuracy of ~90.2% on   the TestSet
* Created custom weights for the optimizer to compensate for the data imbalance between the inputs and labels in the training data. 
* Used StepLR to implement Learning Rate decay during training of the model. 

## Hyperparameters
* Learning Rate: 0.0005, decayed by 0.1 every 2 epochs 
* Epochs: 5 
* Optimizer: Adam 
* Criterion: NLLLoss
