# Video-classification-using-CNN-LSTM

## Introduction
This project is on video classification in which I've used CNN-LSTM architecture which classifies video between ascending and descending order. This might be an easy task for humans but it's very complex for a machine because it has to firstly understand the images frame by frame then has to find information in those sequence of frames and then decide on what it is. My Laptop is not the best to do intensive training on so I've done training on Google Colab where they provide free GPUs for research purposes.

## Dataset
The dataset was created by shooting 100 videos of each ascending and descending and then augmenting it to make 1300 videos each. So total videos were 2600 which were converted to optical flow because optical flow stores the information of the motion in the image. Then it had to be converted to images and saved(Main reason for conveerting it to images is beacuse it has to be fed into Keras' ImageDataGenerator). There were total of 227,188 images(around 700MB) of dimension 224x224x1 so it's obviously not uploaded on this repository but you can download it from https://drive.google.com/open?id=1fa1sQuEyj1L49LAy-yiGQHl7HVBCgJT7. The main advantage of using optical flow is that it has information of motion which is really important in this usecase but apart from it there's no need of proper lighting at the time of realtime testing.

Sample optical flow video (which is later converted into grayscale images)



## Google Colab Notebook
This is the like of the Google Colab Notebook: https://colab.research.google.com/drive/1gYdk9jtr9XmCU-B02Ggx1_QRA4H8jAS7?usp=sharing
So after training the CNN-LSTM model and getting 98% Accuracy and loss of 0.060 
