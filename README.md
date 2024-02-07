# Project Name
 Problem statement: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)



## General Information
- The dataset provided consists images of 9 kinds of Skin Cancers . Hence making this a multi class classification problem
- Convulution Neural Networks (CNN) was used here in this case
- The classes were heavily imbalanced and there was little data too , preventing good results
- Augmentation techiniques were applied to tackle the problem mentioned in the above point
- Various models and Regularization techniques were tried (dropouts and batch normalization)


## Technologies Used - tp be installed
- Augmentor==0.2.12
- pandas==2.2.0
- seaborn==0.13.2
- tensorflow==2.10.0
- matplotlib==3.8.2


## Conclusions
- Minimal Dropout layers give better results
- Batch Normalization introduced a lot noise in the data
- 30 to 40 epochs was the optimal range for epoch
- While the problem of overfitting was addressed on the validation dataset , the accuracy on the test set wasn't as high expected 
- It might also be a good idea to look at other metrics like ROC , MCC ,f1-score 