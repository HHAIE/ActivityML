# Activity Tracker
## Introduction
In the past decade, there has been increased interest on fitness and health. People started to look for ways to be able to track their progress and their status. A suitable and easy to access methods to measure these statuses started to emerge as a good and practical idea instead of always having to go to a specialist to do it.
Hence, the fitness trackers was developed. They use different sensors to measure different variables and using an appropriate algorithm they detect the activity and give the corresponding feedback.

## Methodology

### Problem definition and Database Overview
This project is going to implement a small version of deep neural networks to develop an algorithm to predict a type of activity based on data from different sensors. This is going to be done using a public database that contains the data of 30 subjects. These data includes for each axis in the physical three dimensions (x, y, z), a recording for the values: gravitational acceleration, body acceleration, and body gyroscope. So, this dataset has a total of 9 features. They were recorded using the embedded accelerometer and gyroscope sensors in a Samsung Galaxy SII phone. The data were then sampled in a timesteps manner so as for each sample there are 128 readings for a total of 10299 samples. So, the shape of the dataset is 10299 sample, each has 128 timestep, each has 9 features readings. The data was already preprocessed to reduce the noise and has been normalized so the fall in the range of [-1, 1]. These records were recorded during different activities which are: three static postures (standing, sitting, lying), and three dynamic activities (walking, walking downstairs and walking upstairs). Each sample corresponds to one of the previous 6 activities. So, the problem is a single label multiclass classification.(1)(2)(3) 


## References

1) Anguita, D., Ghio, A., Oneto, L., Parra, X., Reyes-Ortiz, J.L., 2012. Human Activity Recognition on Smartphones Using a Multiclass Hardware-Friendly Support Vector Machine, in: Lecture Notes in Computer Science. Lecture Notes in Computer Science, pp. 216–223.. doi:10.1007/978-3-642-35395-6_30
2) Jorge-L. Reyes-Ortiz, Luca Oneto, Albert SamÃ , Xavier Parra, Davide Anguita. Transition-Aware Human Activity Recognition Using Smartphones. Neurocomputing. Springer 2015.
3) Brownlee, J. (September 17, 2018). "How to Model Human Activity From Smartphone Data." Retrieved August 29, 2022, from https://machinelearningmastery.com/how-to-model-human-activity-from-smartphone-data/