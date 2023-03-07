In this reaserch we demonstrate different methods of size pruning and its effect on the learning process of deep learning models


files: 
 - README.txt
 - __init__.py
 - train.py: 
 	the model manager class:
 		- init the model with the scheduler, optimaizer and scheduler and load the model if needed
 		- train the model
 		- save the model is data and log on files when the model is finish to to train
 		- save the model state
 - utils.py:
 	   - function for plot examples and their prediction according to model's scores
 	   - function for get loader for the dataset according to indexes in dataset
 - veg.ipnyb:
 	   contain experiments on the original dataset:
 	   	- prune 10%-70% of the easiest examples
 	   	- prune sliding window of 40% from the easiest to the hardest
 	   	- prune 10%-90% of the hardest examples
 - veg2.ipynb:
 		contain experiment on dataset after we shuffle 10% of train labels:
 		- prune sliding window of 40% from the easiest to the hardest

run:
the dataset is from this link: https://www.kaggle.com/datasets/ahmadalqawasmeh/vegetables-images 
run veg.ipynb: 
 - download the dataset, rename the dataset file archive.zip to veg.zip and extract inside final/dataset/ folder 
 - run the notebook veg.ipynb
run veg2.ipynb:
 - download the dataset, rename the dataset file archive.zip to veg2.zip and extract inside final/dataset/ folder 
 - run the notebook veg2.ipynb
