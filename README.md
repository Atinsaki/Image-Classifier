# Image-Classifier
Retrain a pre-trained Neural Network to recognize Images

## Requirements:
* Python 3.6.2
* Numpy
* Tensorflow
* Keras

## Usage:
### Retraining for any Image:
* Create a folder in desktop, and extract all files to that folder. Create a folder tf_files inside the main folder.
Place all images in
```
tf_files/[any_name]/folders.
```
The folders must be name of the objects inside. 
  For eg. Folder names Cat will have images of cats

* Go to main folder and Run the following code in CMD:
```
 python -m scripts.retrain --image_dir=tf_files/[any_name]/ --how_many_training_steps=1000 --model_dir=tf_file/model/ --input_height=299 --input_width=299
```
### Testing the Classifier:
* Store the Image to Classify in the main folder

* In the main folder run the following in CMD:
```
python -m scripts.label_image --input_height=299 --input_width=299 --image=[file_to_classify].jpg
```

For more info on training an Image Classifier: 
https://codelabs.developers.google.com/codelabs/tensorflow-for-poets/#0
