A brain tumor is considered as one of the aggressive diseases, among both children and adults.
Brain tumors account for 85 to 90 percent of all primary CNS (central nervous system) tumors.
It is given that approximately 12000 people are diagnosed with a brain tumor every year. 
The best technique to detect brain tumors is Magnetic Resonance Imaging. The images produced are heavily examined
by a radiologist, however one thing to take into consideration, is that mistakes can often happen due to human error.
Therefore, with the use of artifical intelligence being more common, there are various machine learning techniques
that can be implemented to determine the health of a brain given by its MRI scan.

Using TensorFlow, I developed a deep-learning model consisting of various convolution 2D and dense layers with a total
number of trainable parameters of 171,394.

![brain-model](https://user-images.githubusercontent.com/106591496/223693315-39a8b82e-f193-4bac-9120-ff503f1edf7e.png)

I set the initial values of the image size, batch size and epoch number as (190,190), 32, 50 respectively. I intended to use
a higher value for the image size, however due to the limitations of my computer's capabilities, I deduced that (190,190)
was the ideal result. Since the original dataset was small, it would be quick to calculate that the neural network would
produce low accuracy results, therefore, some form of data augmentation was required. I added augmentations of random flip
and random rotation.

After carrying out the fitting of the model, the model produced an accuracy value of 92% for the training data. Applying the
model on the test data produced an accuracy value of 90.6%.

![brain-prediction](https://user-images.githubusercontent.com/106591496/223699570-55968536-4971-491c-b215-6ff2b7fabf4a.png)

![brain-pictures](https://user-images.githubusercontent.com/106591496/223699607-cf20e395-3d55-4e45-a300-83c6e6b2c66e.png)

