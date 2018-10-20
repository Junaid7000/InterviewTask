<b>Task 1</b> is to classify images into  99 diferent classes(Species), Dataset contains 1584 images (990 for training),
a csv file containing 192 features of each 990 images. <br>
In this Task i used 192 preextracted features from the csv file <br>
My approch for this task<br>
(i used keras framework)<br>
<b>Model:</b> Sequential model from keras <br>
<b>layers:</b> input layer --> hidden layer1 --> hidden layer2 --> output layer <br>
<b>Input layer:</b> input dimension = 192 (no of features) <br>
<b>Hidden layer1:</b> keras Dense layer with 300 nodes, Activation function = RELU <br>
<b>Hidden layer2:</b> keras Dense layer with 300 nodes, Activation function = RELU <br>
<b>Output layer:</b> Keras Dense layer with 99(no of classification) o/p nodes, activation function = SOFTMAX <br>
<b>Optimizer:</b> Adams Optimizer
<b>Loss Function:</b> SPARS-CATEGORICAL-CROSSENTROPY 
<b>Metrics:</b> Accuracy metrix
