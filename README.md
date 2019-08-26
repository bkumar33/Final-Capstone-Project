# Final-Capstone-Project 

## Pneumonia Detection From Chest Radiograph (CXR) 

### Problem Statement :

Pnumonia is an infection that inflames the air sacs in one or both of the lungs. The air sacs may fill with fluid or pus(purulent material), causing cough with phlegm or pus, fever, chills, and difficult breathig. It can be found in kids, alults and seniors. In many cases it may cause a death. As a data scientist my job is to build a model that can detect Pneumonia at early state so it can treated propely.

### Approach

Approach I took on this project is building a Deep Learning Model which train on Pneumonia data that was provided by Kaggle competition. Link : <https://www.kaggle.com/c/rsna-pneumonia-detection-challenge/data> 

The dataset is 3.7 GB in size with over 30k CXR Images of patients. Images are labeled with 3 different classes: Normal, Lung opacity, No lung opacit/not normal. The goal is first identify correctly identify which the images that Pneumina. Medical Images can be very complicated and they are in this case. It holds alot of confidential information about patients which is encrypted. 


### Model Results

Binary Model - 81 % Accuracy

Multiclass Model - 68 % Accuracy 

### Obstacles 

My model did not score that great because original image was 1024 X 1024. Building a convolutional neural network takes in alot of computing power. Every time I ran a model on my local machine, it would crash. I tried resizing it to 512 X 512, 256 X 256, 128 X 128. All were crashing and killing the kernerl on jupyter notebook. I had to resize the images to 64 X 64, which took a a while to process but was able to the give me results of my model. 

### Next Step 

1. Run models on GPU, EC2 Instances on Amazon Machine Images (AMI) with Image size 1024 X 1024 on P2.xlarge or higher
2. Improve Accuracy score on correctly predicting the pnemonia 
3. Once predicted correctly build a boarder around the where possible signs of lung opacity (pnemonia)



