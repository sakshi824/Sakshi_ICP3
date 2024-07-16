# Sakshi_ICP3
Name: Sakshi Jadhav
ID:700757772
VIDEO-LINK:  https://drive.google.com/file/d/1T1QNPqfrkZajASzBEqd1qmGwVSGlJJta/view?usp=share_link

VIDEO-LINK: https://drive.google.com/file/d/1xyKfzf6QxDJY6mueZLu-ZMf1Bzxb2TV2/view?usp=share_link

--> First we have had modified the image classification code, we have changed the input shape which in previous code they had provided the wrong values(3,32,32) changed to (32,32,3). Then it executed succesfully.
<img width="452" alt="image" src="https://user-images.githubusercontent.com/122486644/227105002-d2305c9a-693f-42b5-91aa-933cea3b01a3.png">
<img width="605" alt="image" src="https://user-images.githubusercontent.com/122486644/227105063-3beb8c48-0b4f-4674-96f6-b0e4fd357de5.png">

1. Follow the instruction below and then report how the performance changed.(apply all at once)
  First we have fixed random seed for reproducibility, then load the data, then Normalize inputs from 0-255 to 0.0-1.0, then encode the outputs of one hot, then create the model.
• we have added this layer by using the add function "Convolutional input layer, 32 feature maps with a size of 3×3 and a rectifier activation function".
• Then Dropout layer at 20%.
• Convolutional layer, 32 feature maps with a size of 3×3 and a rectifier activation function.
• Max Pool layer with size 2×2.
• Convolutional layer, 64 feature maps with a size of 3×3 and a rectifier activation function.
• Dropout layer at 20%.
• Convolutional layer, 64 feature maps with a size of 3×3 and a rectifier activation function.
• Max Pool layer with size 2×2.
• Convolutional layer, 128 feature maps with a size of 3×3 and a rectifier activation function.
• Dropout layer at 20%.
• Convolutional layer,128 feature maps with a size of 3×3 and a rectifier activation function.
• Max Pool layer with size 2×2.
• Flatten layer.
• Dropout layer at 20%.
• Fully connected layer with 1024 units and a rectifier activation function.
• Dropout layer at 20%.
• Fully connected layer with 512 units and a rectifier activation function.
• Dropout layer at 20%.
• Fully connected output layer with 10 units and a Softmax activation function

Then we have have compiled the model then fit the model and then evaluated the model.
<img width="713" alt="image" src="https://user-images.githubusercontent.com/122486644/227106467-8689540e-3513-454b-b3ed-318ed731a047.png">

Did the performance change?
Yes we can see the change in performance. We can see the accuracy is changed as compared to the previous model.

2. Predict the first 4 images of the test data using the above model. Then, compare with the actual label for those 4
images to check whether or not the model has predicted correctly.

First we have predicted the first 4 images of the test data and then converted the predictions to class labels and then converted the actual labels to class labels and then printed the predicted and actual labels for the first four images.
<img width="338" alt="image" src="https://user-images.githubusercontent.com/122486644/227107221-16ccfa42-44b0-4163-97cf-c4fce4a32cf8.png">

3. Visualize Loss and Accuracy using the history object

Then here we are ploting the both training and validation loss along with it here we are also ploting the training and validation accuracy.
<img width="697" alt="image" src="https://user-images.githubusercontent.com/122486644/227107525-343f342b-6df3-4867-b1a0-6bbae6b65e14.png">


