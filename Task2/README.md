<B>#Task 2</B><br>
I used <B>tensorflows object detection api</B> for identifying fruits, mainly Apple, Banana & Orange from images(test images = 60 ).<br>
Tensorflows Object Detection Api:<br>
				<p>It is high level open source api, built on top of tensorflow framework for building powerful image recognization software, 
<br>
<br>
<b>problem Statement</b>: To train a object detection model using tensorflows object detection api, using 240 fruits images containing three different fruits(apple, banana & orange) & testing it over 60 images of fruits.<br>
<br>
<b>Following steps I performed to train object detection model </b><br>
<br>
<b>step 1:</b> Installing model:
1. clone github respo from "https://github.com/tensorflow/models" <br>
2. downloading all required lib like, Cython, lxml, jupyter, protocolbuffer<br>
3. Testing model using 'object_detection_model.ipynb' jupyter notebook.<br>
<br>
<b>step 2:</b>  Selecting a model: <br>
<br>
The default model in the notebook is the simplest (and fastest) pre-trained model offered by TensorFlow. You can see there are many other models available. mAP stands for mean average precision, which indicates how well the model performed on the COCO dataset. Generally models that take longer to compute perform better. However these models also have a number of subtle differences (such as performance on small objects)<br>
I have selected <b> faster_rcnn_inception_v2_pets </b> from tensorflows objec detection zoo for my object detection model, As it has low speed but higher accuracy. <br><br>
<b>step 3:</b> Coverting Existing database to Tensorflow records<br>
	TensorFlow provides us with a sample script in the file 'using_your_own_dataset.md' which by doing slight modification can convert our dataset in TF records also the given dataset of images is pre-labeled, so labeling is not required<br>
	next step is to create create a labelmap.pbtxt file which will save labels with a unique id <br>
<b>Training model:</b> I trained model for 5300 steps, where losssed were dropped to 0.0966
	<br>
	<br>
Following folders are attached:<br>
	1. Training checkpoints : folder conataining train.py sript, generate_tfrecord.py script <br>
	2. TensorBord : All tensorbord graph for loss <br>
	3. Inference graph: pipeline config, inference graph, model config file <br>
	4. graph.png: tensorboard graph


	

				
