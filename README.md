# Unsupervised-image-clustering
Using unsupervised learning to cluster 57k+ images.

•	AIM : To classify faces using unsupervised approach.


Face_encoding.ipynb:  In this file I have written the code to read every image one by one from all the three directories and also, I have used the trained dlib face detection model to detect the faces and encode them into 128-D vector. In the 5th shell, the code to eliminate no face images and encode the face images is written. And I have saved three csv files (f584_data.csv, dd40_data.csv, a055_data.csv)  each representing encodings of images(only face images) from the given three data sets.





Clustering.ipynb: In this notebook, I first imported the following csv files one by one: 
f584_data.csv
 dd40_data.csv
a055_data.csv
And cleaned it a bit(dropping unnecessary column), then I used the famous K-Means algorithm to cluster the rows in the csv files. I used the Sklearn library from that. After clustering, in the 7th shell, you can see I have stored the predicted IDs of each row(which basically represents a face) in a list. Then I put together the image name and predicted ID together and saved it as a csv file and stored it in the results folder. 


