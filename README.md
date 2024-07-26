Gesture classification using muscle activity - Neural Networks
Prosthetic control systems enable prosthetic devices to have multiple degrees of freedom. The system is built of several components. It connects a muscle activity (EMG, Electromyography) sensor to a user Android/Android Things App. The app collects data, then a server builds a Tensorflow model specifically for this user. After that the model can be downloaded and executed on the device to control motors or other appendages.
This dataset can be used to map user residual muscle gestures to certain actions of a prosthetic such as an open/close hand or rotate wrist.
For a reference please watch a video on this topic : Living with a mind-controlled robot arm
Four classes of motion were written from MYO armband,
with the help of the nukleous app : https://github.com/cyber-punk-me/nukleos.
The MYO armband has 8 sensors placed on the skin surface, each measure electrical activity produced by muscles beneath.

We will build a gesture classification model using the gesture classification dataset
In the first step, I will be performing the below operations to check what the data set comprises of and will check the below things:

1.) head of the dataset
2.) shape of the dataset
3.) info of the dataset
4.) summary of the dataset
Often the variables of the data set are of different scales i.e. one variable is in millions and other in only 100. 
For e.g. in our data set 'muscle reading 1 sensor 1 is having values in single digit negative and 'muscle reading 8 sensor 7 in three digits positive numbers.
Since the data in these variables are of different scales, it is tough to compare these variables.
Feature scaling (also known as data normalization) is the method used to standardize the range of features of data. 
Since, the range of values of data may vary widely, it becomes a necessary step in data preprocessing while using machine learning algorithms

One-Hot-Encoding is used to create dummy variables to replace the categories in a categorical variable into features of each category and represent it using 1 or 0 based on the presence or absence of the categorical value in the record.**

**This is required to do since the machine learning algorithms only works on the numerical data. That is why there is a need to convert the categorical column into numerical one.**

**get_dummies is the method which creates dummy variable for each categorical variable.**

It is considered a good practice to set parameter `drop_first` as `True` whenever get_dummies is used. It reduces the chances of multicollinearity and the number of features are also less as compared to `drop_first=False

