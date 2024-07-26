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
