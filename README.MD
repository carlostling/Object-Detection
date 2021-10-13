# Project overview
This project aims to utilize Waymos open dataset in order to create a object detector that detects other vehicles, pedestrians and cyclists. 

# Dataset
The data contains images with different weather, time of day, blurriness and potentially different cameras. All images take the same shape. Some images, such as this one:
![image](https://user-images.githubusercontent.com/31474054/137139513-27acf0a5-5d7b-44db-b582-cf0fa21d8ae4.png)
Is annotated wrongly with the big box indicating a pedestrian where there is none. 

We also see a major skew in class distribution. We have plenty of vehicles, less pedestrians and a very low relative amount of cyclists.

# Cross validation
As we have a skewed distribution, I'd like to stratify the data at split - but this doesn't seem to be possible with the way this task is outlined (split into folders).
Instead, I've opted to randomly shuffle the dataset to reduce the skew in each sample. This should in theory ensure equal distribution of samples in the splits. 

Out of 100 files, I've opted to use 75 files for training, 10 files for testing and 15 files for validation. 

# Training

# Improve on the reference
This section should highlight the different strategies you adopted to improve your model. It should contain relevant figures and details of your findings.
